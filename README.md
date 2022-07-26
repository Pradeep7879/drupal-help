# drupal-help

Get value from path.

    $current_path = \Drupal::request()->getPathInfo();
    $path_args = explode('/', $current_path);
    $is_string_path = in_array('string', $path_args);
