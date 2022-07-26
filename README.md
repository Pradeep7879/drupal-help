# drupal-help

Get value from path.

      $current_path = \Drupal::request()->getPathInfo();
      $path_args = explode('/', $current_path);
      $is_discussion_path = in_array('discussion', $path_args);
