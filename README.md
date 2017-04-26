[![Build Status](https://travis-ci.org/espebra/varnish-vcl-snippets.svg)](https://travis-ci.org/espebra/varnish-vcl-snippets)

# VCL snippets for Varnish Cache 4

The purpose of this repository is to gather a set of VCL snippets for specific use cases. The files should include comments and tests.

* [Edge Side Includes (ESI)](esi.vtc)
* [Grace mode and stale-while-revalidate](grace.vtc)
* [Serving stale content on slow backend responses](grace-if-slow-backend-request.vtc)
* [Lurker friendly bans](lurker-friendly-bans.vtc)
* [Regexp cache invalidation](regexp-cache-invalidation.vtc)
* [Range requests from clients](range.vtc)
* [Regular redirect](redirect.vtc)
* [HTTP to HTTPS redirect based on X-Forwarded-Proto](elb-http-to-https-redirect.vtc)
* [Retry a backend request when using a single backend](retry-single-backend.vtc)
* [Retry a backend request to a new backend when using a random director](retry-random-director.vtc)
* [Retry a backend request to a new backend when using a round-robin director](retry-round-robin-director.vtc)

Pull requests are welcome.

## Other similar sources

* [fgsch](https://github.com/fgsch/vcl-snippets)
* [Varnish Cache VCL examples](https://www.varnish-cache.org/trac/wiki/VCLExamples)

