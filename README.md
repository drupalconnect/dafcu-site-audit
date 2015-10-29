Introduction
=======

There is no doubt that the developers that have worked on this site know Drupal site building and development. Any site, of course, can be improved, and almost all custom modules have some rough edges or serve as a quick solution. With that, the point of this documentation is to identify the areas of the site that can be built and improved upon. This should help ease deeper understanding of the architecture of this Drupal instance.

The modules and themes and libraries are in "sites/default". The public files for the site are in "sites/default/files", although there is a "sites/default/files.old" directory that may be taking up unnecessary disk space.

Drupal core for this site is a couple versions behind and should be updated to the latest version. The most recent release is 7.41 (which will change) and should be applied to this or any other site to maintain a secure site.

Out-of-date modules should also be updated (see [Update Report](update_report.md)). Any patches will need to be reapplied, of course, as needed (see [Patches Report](patches_report.md). Note that some modules are a "dev" version or are not reporting a version. These should be updated to more current versions.