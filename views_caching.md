# Views

As the Views module is the most popular contributed module, most of us are using it to display content is various ways. Views instances should be cached so that when accessed, a cached copy is returned instead of having to rebuild each view every time it's loaded. There are two (2) options here.

* Time-based caching for each view display (ships with Views)
* [Views Cache Bully](https://drupal.org/project/views_cache_bully): Enforces Views time-based caching for all uncached views.

Considering we want to apply the same caching strategy to all views the latter would probably be a more viable implementation.