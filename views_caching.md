# Views

As the Views module is the most popular contributed module, most of us are using it to display content is various ways. Views instances should be cached so that when accessed, a cached copy is returned instead of having to rebuild each view every time it's loaded. There are two (2) options here.

* Time-based caching for each view display (ships with Views)
* [Views Content Cache](https://drupal.org/project/views_content_cache): Update each view only when its constituent element have been updated.