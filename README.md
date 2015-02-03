# custom
&lt;?php global $post; $args = array( 'posts_per_page' => 10, 'post_type'=> 'custom-post-type' ); $myposts = get_posts( $args ); foreach( $myposts as $post ) : setup_postdata($post); ?>  &lt;?php  $job_link= get_post_meta($post->ID, 'job_instructions', true);  ?>   &lt;h2>&lt;?php the_title(); ?>&lt;/h2>  &lt;?php the_content(); ?>  &lt;p>&lt;?php echo $job_link; ?>&lt;/p>
