# Views

As the Views module is the most popular contributed module, most of us are using it to display content is various ways. Views instances should be cached so that when accessed, a cached copy is returned instead of having to rebuild each view every time it's loaded. There are two (2) options here.

* Time-based caching for each view display (ships with Views)
* Views Content Cache: Update each view only when its constituent element have been updated.
 
If you've got a lot of content and are using Views paging, you may want to consider using Views Litepager. It will work around slow COUNT queries on InnoDB tables, those using the default table-engine type in MySQL.