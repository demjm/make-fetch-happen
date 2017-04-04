# Change Log

All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.

<a name="1.3.1"></a>
## [1.3.1](https://github.com/zkat/make-fetch-happen/compare/v1.3.0...v1.3.1) (2017-04-04)


### Bug Fixes

* **cache:** pretend cache entry is missing on ENOENT ([9c2bb26](https://github.com/zkat/make-fetch-happen/commit/9c2bb26))



<a name="1.3.0"></a>
# [1.3.0](https://github.com/zkat/make-fetch-happen/compare/v1.2.1...v1.3.0) (2017-04-04)


### Bug Fixes

* **cache:** if metadata is missing for some odd reason, ignore the entry ([a021a6b](https://github.com/zkat/make-fetch-happen/commit/a021a6b))


### Features

* **cache:** add special headers when request was loaded straight from cache ([8a7dbd1](https://github.com/zkat/make-fetch-happen/commit/8a7dbd1))
* **cache:** allow configuring algorithms to be calculated on insertion ([bf4a0f2](https://github.com/zkat/make-fetch-happen/commit/bf4a0f2))



<a name="1.2.1"></a>
## [1.2.1](https://github.com/zkat/make-fetch-happen/compare/v1.2.0...v1.2.1) (2017-04-03)


### Bug Fixes

* **integrity:** update cacache and ssri and change EBADCHECKSUM -> EINTEGRITY ([b6cf6f6](https://github.com/zkat/make-fetch-happen/commit/b6cf6f6))



<a name="1.2.0"></a>
# [1.2.0](https://github.com/zkat/make-fetch-happen/compare/v1.1.0...v1.2.0) (2017-04-03)


### Features

* **integrity:** full Subresource Integrity support (#10) ([a590159](https://github.com/zkat/make-fetch-happen/commit/a590159))



<a name="1.1.0"></a>
# [1.1.0](https://github.com/zkat/make-fetch-happen/compare/v1.0.1...v1.1.0) (2017-04-01)


### Features

* **opts:** fetch.defaults() for default options ([522a65e](https://github.com/zkat/make-fetch-happen/commit/522a65e))



<a name="1.0.1"></a>
## [1.0.1](https://github.com/zkat/make-fetch-happen/compare/v1.0.0...v1.0.1) (2017-04-01)



<a name="1.0.0"></a>
# 1.0.0 (2017-04-01)


### Bug Fixes

* **cache:** default on cache-control header ([b872a2c](https://github.com/zkat/make-fetch-happen/commit/b872a2c))
* standard stuff and cache matching ([753f2c2](https://github.com/zkat/make-fetch-happen/commit/753f2c2))
* **agent:** nudge around things with opts.agent ([ed62b57](https://github.com/zkat/make-fetch-happen/commit/ed62b57))
* **agent:** {agent: false} has special behavior ([b8cc923](https://github.com/zkat/make-fetch-happen/commit/b8cc923))
* **cache:** invalidation on non-GET ([fe78fac](https://github.com/zkat/make-fetch-happen/commit/fe78fac))
* **cache:** make force-cache and only-if-cached work as expected ([f50e9df](https://github.com/zkat/make-fetch-happen/commit/f50e9df))
* **cache:** more spec compliance ([d5a56db](https://github.com/zkat/make-fetch-happen/commit/d5a56db))
* **cache:** only cache 200 gets ([0abb25a](https://github.com/zkat/make-fetch-happen/commit/0abb25a))
* **cache:** only load cache code if cache opt is a string ([250fcd5](https://github.com/zkat/make-fetch-happen/commit/250fcd5))
* **cache:** oops ([e3fa15a](https://github.com/zkat/make-fetch-happen/commit/e3fa15a))
* **cache:** refactored warning removal into main file ([5b0a9f9](https://github.com/zkat/make-fetch-happen/commit/5b0a9f9))
* **cache:** req constructor no longer needed in Cache ([5b74cbc](https://github.com/zkat/make-fetch-happen/commit/5b74cbc))
* **cache:** standard fetch api calls cacheMode "cache" ([6fba805](https://github.com/zkat/make-fetch-happen/commit/6fba805))
* **cache:** was using wrong method for non-GET/HEAD cache invalidation ([810763a](https://github.com/zkat/make-fetch-happen/commit/810763a))
* **caching:** a bunch of cache-related fixes ([8ebda1d](https://github.com/zkat/make-fetch-happen/commit/8ebda1d))
* **deps:** `cacache[@6](https://github.com/6).3.0` - race condition fixes ([9528442](https://github.com/zkat/make-fetch-happen/commit/9528442))
* **freshness:** fix regex for cacheControl matching ([070db86](https://github.com/zkat/make-fetch-happen/commit/070db86))
* **freshness:** fixed default freshness heuristic value ([5d29e88](https://github.com/zkat/make-fetch-happen/commit/5d29e88))
* **logging:** remove console.log calls ([a1d0a47](https://github.com/zkat/make-fetch-happen/commit/a1d0a47))
* **method:** node-fetch guarantees uppercase ([a1d68d6](https://github.com/zkat/make-fetch-happen/commit/a1d68d6))
* **opts:** simplified opts handling ([516fd6e](https://github.com/zkat/make-fetch-happen/commit/516fd6e))
* **proxy:** pass proxy option directly to ProxyAgent ([3398460](https://github.com/zkat/make-fetch-happen/commit/3398460))
* **retry:** false -> {retries: 0} ([297fbb6](https://github.com/zkat/make-fetch-happen/commit/297fbb6))
* **retry:** only retry put if body is not a stream ([a24e599](https://github.com/zkat/make-fetch-happen/commit/a24e599))
* **retry:** skip retries if body is a stream for ANY method ([780c0f8](https://github.com/zkat/make-fetch-happen/commit/780c0f8))


### Features

* **api:** initial implementation -- can make and cache requests ([7d55b49](https://github.com/zkat/make-fetch-happen/commit/7d55b49))
* **fetch:** injectable cache, and retry support ([87b84bf](https://github.com/zkat/make-fetch-happen/commit/87b84bf))


### BREAKING CHANGES

* **cache:** opts.cache -> opts.cacheManager; opts.cacheMode -> opts.cache
* **fetch:** opts.cache accepts a Cache-like obj or a path. Requests are now retried.
* **api:** actual api implemented