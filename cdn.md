# CDN

In many cases, it's very advantageous to integrate your Drupal site with a CDN. A CDN reduces the latency between the end user and the server that serves files (resources) referenced by the HTML, such as CSS, JavaScript, fonts and images. The CDN achieves this by hosting and serving the content on servers that they manage that are often geographically close to the user.

CDNs can be populated either by physically uploading content to their network or by configuring an origin server that contains the content that should be served via a CDN. For Drupal sites, an origin server is the easiest approach.

Below are a few options for Content Delivery Networks. The pros and cons are detailed for each.

* [CloudFlare](cloudflare.md)
* [MaxCDN](maxcdn.md)
* [Amazon CloudFront](amazon_cloudfront.md)