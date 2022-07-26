# drupal-help

Get value from path.

    $current_path = \Drupal::request()->getPathInfo();
    $path_args = explode('/', $current_path);
    $is_string_path = in_array('string', $path_args);

Set Page Title

    $node_details = Node::load($nid);
    $page_title = $node_details->getTitle();
    $request = \Drupal::request();
    if ($route = $request->attributes->get(\Symfony\Cmf\Component\Routing\RouteObjectInterface::ROUTE_OBJECT)) {
      $route->setDefault('_title', $page_title);
    }
