# Caching

Since most of the site's traffic is unauthenticated, this is one of the easiest areas to address. This allows us to serve a cached (static/pre-built) page with no personal deviation. In this case, most of Drupal's out-of-the box mechanisms for caching are already utilized, which is great. Though in a world where [milliseconds of load time could cost you millions of users](http://www.nytimes.com/2012/03/01/technology/impatient-web-users-flee-slow-loading-sites.html?_r=0), sometimes putting in a little extra effort is necessary. In return, server load and therefore cost can be drastically reduced with the proper configuration.

Below are recommendations based on our findings:

Views, block and panels caching do not appear to be fully utilized please review the links below.

* [Views Caching](views_caching.md)
* [Blocks Caching](blocks_caching.md)
* [Panels Caching](panels_caching.md)

Drupal core caching methods are all utilized which is good, but the Minimum Cache Lifetime should be set to none at admin/config/development/performance.

For a significant increase in performance, consider the alternative caching back-ends below.

* [Caching Backends](caching_backends.md)