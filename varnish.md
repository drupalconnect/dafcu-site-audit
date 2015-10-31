# Varnish

* An HTTP accelerator that delivers a cached version of a page for a set amount of time without ever having to hit your back-end server, increasing the delivery of said page 300-1000x while reducing load on your server ten-fold. Each Varnish container can handle thousands of requests per second, much faster than a site's framework alone.

* The Drupal module allows for a user-friendly integration to Drupal requiring minimum system administration skills.

* Can also be used as a round-robin load balancer that directs traffic to proxy servers when volume grows beyond what one server can handle. This ensures that your site is always responding.

* http://drupal.org/project/varnish