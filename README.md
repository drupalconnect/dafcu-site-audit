Introduction
=======

There is no doubt that the developers that have worked on this site know Drupal site building and development.  Any site, of course, can be improved, and almost all custom modules have some rough edges or only serve as a quick solution. Still, the point of this documentation is to identify areas in the site that can be built upon, areas of improvement, and help facilitate deeper understanding of the architecture of this Drupal instance.

The modules and themes for all sites are in "sites/default".  The public files for the parent site are in "sites/default/files", while the subsites all use their own multisite directory.  Several modules are a "dev" version or are not reporting a version.  These should be updated to more current versions.

Drupal core for this site is only 6.30, which is more than a year old and quite insecure.  The current version is 6.37 (which will change) and should be applied to this or any other site to maintain a secure site.  Out-of-date modules should also be updated.  Any patches will need to be reapplied, of course, as needed.

