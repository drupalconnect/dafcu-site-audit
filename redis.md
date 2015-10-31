# Redis

Redis can be used as a drop-in caching back-end for your Drupal website. Like Varnish, it requires basic sysadmin knowledge to install on the server, then the Drupal module handles the rest.

##Benefits of Redis
Most website frameworks like Drupal and WordPress use the database to cache internal application "objects" which can be expensive to generate (menu trees, filter results, etc), and to keep cached page content. Since the database also handles many queries for normal page requests, it is the most common bottleneck causing increase load-times.

Redis provides an alternative caching backend, taking that work off the database, which is vital for scaling to a larger number of logged-in users. It also provides a number of other nice features for developers looking to use it to manage queues, or do custom caching of their own.

* http://drupal.org/project/redis