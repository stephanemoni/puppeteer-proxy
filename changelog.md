# Change log
### [1.2.8] - 2020-07-21
#### Changes
- Fixed silent failure when there was an invalid host in the cookies set by the server ([#32](https://github.com/Cuadrix/puppeteer-page-proxy/issues/32))
- Fixed Page URL not updating in Puppeteer when there was a server-side redirect (via location header)
### [1.2.7] - 2020-06-30
#### Changes
- Reimplement cookie handling to account for deletion and addition of browser cookies
- Changed default lookup fetch source to **api64.ipify.org**
- Update documentation
### [1.2.6] - 2020-06-18
#### Changes
- Updated for Puppeteer's v4.0.0 [breaking changes](https://github.com/puppeteer/puppeteer/releases/tag/v4.0.0) ([#22](https://github.com/Cuadrix/puppeteer-page-proxy/issues/22), [#23](https://github.com/Cuadrix/puppeteer-page-proxy/issues/23))
- Modified cookie handling to fix ([#20](https://github.com/Cuadrix/puppeteer-page-proxy/issues/20)) among other cookie related errors
### [1.2.5] - 2020-05-21
#### Changes
- Added ability to override requests
- Increase redirect restriction ([#17](https://github.com/Cuadrix/puppeteer-page-proxy/issues/17))
### [1.2.4] - 2020-05-18
#### Changes
- Fix 'net::ERR_FAILED' by updating package to work with latest Got ([#16](https://github.com/Cuadrix/puppeteer-page-proxy/issues/16), [#14](https://github.com/Cuadrix/puppeteer-page-proxy/issues/14))
- Added an explanation addressing site insecurity ([#9](https://github.com/Cuadrix/puppeteer-page-proxy/issues/9), [#12](https://github.com/Cuadrix/puppeteer-page-proxy/issues/12))
- Removed type enforcing
### [1.2.3] - 2020-02-14
#### Changes
- Added ability to remove page-wide proxy
- Changed static classes to object literals for compability with Node.js **10.16.x** ([#6](https://github.com/Cuadrix/puppeteer-page-proxy/issues/6))
- Removed `src\util\` folder along with proxy-validator
### [1.2.2] - 2020-02-09
#### Patches
- Fixed code indentation.
- Updated examples.
- Optimization.
### [1.2.0] - 2020-02-09
#### Major changes
- Added capability to change proxy per request.
- Added capability of changing the proxy if a page is already using one.
- Replaced [Request](https://github.com/request/request) with [Got](https://github.com/sindresorhus/got) for forwarding requests.
- Added [tough-cookie](https://github.com/salesforce/tough-cookie) for handling cookies
- Now communicates directly with Chrome DevTools Protocol when getting cookies
#### Minor changes
- Added a simple type enforcer and proxy validator.
- Removed some redundant code.
- Removed obsolete 'cache' parameter