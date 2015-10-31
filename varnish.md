# Varnish

Varnish is an HTTP accelerator that quickly serves both static content and anonymous pages. By serving data from virtual memory, a response is returned without needing to access the application server, which in turns frees application container workers to build more dynamic requests.. Each Varnish container can handle thousands of requests per second, much faster than a site's framework alone.

Varnish can also improve the availability of your site. For example, if a PHP fatal error breaks your site, anonymous page requests can still be served by Varnish and end-users won't realize anything is wrong.

The Drupal module allows for a user-friendly integration to Drupal requiring minimum system administration skills.

* http://drupal.org/project/varnish