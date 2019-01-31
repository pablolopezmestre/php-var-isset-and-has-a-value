# php-var-isset-and-has-a-value
Check if PHP var is set and has a certain value in one line


// Traditional way
if ( isset($my_var) ) {
    if ( true === $my_var ) {
        // do something
    }
}
 
// Same, but in one line
if ( true === ( isset( $my_var ) ? $my_var : null ) ) {
    // do something
}

// Using PHP 7 null coalesce operator
if ( true === ( $my_var ?? null ) ) {
    // do something
}
