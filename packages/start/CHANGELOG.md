# @solidjs/start

## 0.7.4

### Patch Changes

- 67a469f8: keep all entries as jsx to ensure treated as src

## 0.7.3

### Patch Changes

- 61381f1f: fix: remove dev overlay in prod
- 6c3eff5e: fix #1375 extensions for unprocess .js entries

## 0.7.2

### Patch Changes

- 480802f7: change to ts build
- 090df26b: fix import.meta.env resolution

## 0.7.1

### Patch Changes

- 1891af96: fix #1370 cannot resolve #start/app

## 0.7.0

### Minor Changes

- e33d506e: fix FS router circular dep by moving import
- 7b1c82be: add `.` notation to escape layouts in FS routes
- 28357e62: update config to anticipate Vite updates, clearer experimental features, routesDir
- d491fa8f: remove support for event symbol autoforwarding
- 113c5d53: add serverFunctionMeta
- b9b6eed8: transparent errors and support http status forwarding in server fns

### Patch Changes

- 30862af6: fix types for latest updates
- 32fc1f39: Fix dev overlay's CodeView not working with `mjs` or `cjs` files
- 29ffd16b: don't import app on server for SSR false when SingleFlight false
- 476b8ecf: add back different content type parsing in case middleware etc..
- ea53d37a: update Vinxi and Solid Router
- b19ff69f: revert vite alignment until we know more, add server option to types
- 256488b2: fix #1366 islands mode reference

## 0.6.1

### Patch Changes

- 29e4ec60: Fix refresh pragma
- cbcdde3c: update ts, fix #1346 flash types
- bb6d61ac: Update package.json to include license

## 0.6.0

### Minor Changes

- dbc0c685: Update to vinxi 0.3.3 (thus also Vite 4 -> 5)
- d1a4ec95: move server rendering options to handler
- 3bcfaf16: vite.config -> app.config

### Patch Changes

- eca781a7: configurable dev overlay
- 03a8d1f8: update vinxi, fix prerendering
- 44aa4c05: handler options as function, forward nonce to main scripts
- 516df5da: fix nojs flash update auth/prisma examples

## 0.5.10

### Patch Changes

- 2c503fd0: fix #1342 unintended early return in router < 12.4
- 688a643b: fix: resolve the import path correctly (@solidjs/start/server vs @solidjs/start/./server)
- 35dd4297: fix nojs return responses, fix throw single flight

## 0.5.9

### Patch Changes

- 15f497da: fix empty post bodies in server functions

## 0.5.8

### Patch Changes

- df779e9d: fix json returns from actions

## 0.5.7

### Patch Changes

- 59e8533a: lock vite-plugin-solid into 2.9.x

## 0.5.6

### Patch Changes

- dafdd97a: fix typescript
- b422f708: Fix: calling server functions without arguments, TS strict
- f73de3a6: fix: server functions router should put user plugins before server plugin
- 28691fc3: fix up single flight mutation

## 0.5.5

### Patch Changes

- f787f2b6: update router
- 77e57b2a: Fix #1299, Fix dev overlay logs
- 2cd7a3b3: Fixes incorrect, missing `type` import declarations.
- 2c193283: fix singleflight mutations in non-ALS envs
- 38ba8de8: fix singleflight eating response bodies

## 0.5.4

### Patch Changes

- 0b7eceeb: fix prerender/content-type, stupid copy-paste

## 0.5.3

### Patch Changes

- 4c32e85a: add base url to single flight redirect
- d8bcc5c5: add notes demo, fix redirects in single flight

## 0.5.2

### Patch Changes

- ebe9d0fb: fix up response iterables
- 4d66b4de: Fixed an issue with TypeScript based projects throwing client side errors regarding a type input in the `ErrorBoundary`.wq
- 20697edd: initial support for single flight mutations
- ae6dc628: update Solid to 1.8.14 to fix storage import

## 0.5.1

### Patch Changes

- a57b340f: update references to vinxi/http
- 733400fb: pull API routes back in
- 158f1090: fix storage import, update solid-js
- 11beebd6: fix unocss example
- 7dc792ca: fix tailwind typings

## 0.5.0

### Minor Changes

- 377635b8: move API out of main handler
- 97e0d62e: Add ssr "sync" render mode
- 63d09b0d: Remove old create-solid CLI
- 4311e830: Update to vinxi 0.2.x
- 30f8e521: use ALS for Http helpers
- d5e11006: split out solid event from native event
- 1e0542cf: Add ResponseSub wrapper to RequestEvent
- feb4a515: update entries, stop re-export of vinxi/server
- ca22cc81: update to router 0.11.0

### Patch Changes

- 7d7b073e: improve API route processing with Radix3
- 34c91747: vinxi - 0.1.10, automatic symbol based event discovery
- 6e8b2beb: update router again metadata -> info
- 54501ea6: fix #1278 wrong types for onBeforeResponse middleware
- e811c16a: fix up server function runtime typescript
- 18f2f71a: Add ability to type Locals, cleanup
- 3eb9ae8c: restore API routes to shared path
- 6ef9515f: improve API route passthrough

## 0.4.11

### Patch Changes

- 187acc55: update vinxi, fix #1247, fix #1261
- 92e8f8f8: fix formData and action issue for cloud runtimes
- 27d60cd2: better GET signature
- 24a4eb2e: GET server functions, response returns, cache to use GET
