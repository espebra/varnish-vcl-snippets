[![Build Status](https://travis-ci.org/espebra/varnish-vcl-snippets.svg)](https://travis-ci.org/espebra/varnish-vcl-snippets)

# VCL snippets for Varnish Cache 4

The purpose of this repository is to gather a set of VCL snippets for specific use cases. The files should include comments and tests.

* [Grace mode and stale-while-revalidate](grace.vtc)
* [Edge Side Includes (ESI)](esi.vtc)
* [Retry a backend request when using a single backend](retry-single-backend.vtc)
* [Retry a backend request to a new backend when using a round-robin director](retry-round-robin-director.vtc)
* [Retry a backend request to a new backend when using a random director](retry-random-director.vtc)

Pull requests are welcome.

## Other similar sources

* [fgsch](https://github.com/fgsch/vcl-snippets)
* [Varnish Cache VCL examples](https://www.varnish-cache.org/trac/wiki/VCLExamples)

