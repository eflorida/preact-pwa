# Preact Boilerplate - PWA, SSR

A `Super fast progressive web app` with a small footprint & minimal dependencies.  

Features universal rendering, redux, state-driven routing, preact, & service workers.  Crunched & optimized with rollup, buble, optimize-js, & purify-css.

## bundle sizes & performance
(These stats have not been updated since forking)
```
Bundle Size:            28.63 KB, 9.64 KB Gzipped
Webpage test:           A, A, A
pagespeed:              100
lighthouse:             100
```

## Getting Started

### Prerequisites

Make sure that [Node v8](https://nodejs.org/en/download/releases/) is installed.

### Instructions

First, clone the repo

```bash
$ git clone https://github.com/eflorida/preact-pwa.git
```

Then, install all dependencies:

```bash
$ npm install
```

Finally, to run the project for development:

```bash
$ npm run dev
```

Or, to run the project for production:

```bash
$ npm start
```

## Performance insights (note: incomplete)

### Lighthouse results

HTTP2 and HTTPS support are required for perfect scores, but typically not available on local server.

### manifest.json

Using 192x192 for minimum sized icon, omitting other sizes to reduce downloads for users
[reference](https://developers.google.com/web/updates/2015/10/splashscreen)

### libraries

- we can shave off ~10 KB, ~3kb Gzipped by pruning `preact-redux` & manually connecting

## Features

- Progressive Web App enabled with [service workers](https://developers.google.com/web/fundamentals/getting-started/primers/service-workers)
- Offline capable with [service workers](https://developers.google.com/web/fundamentals/getting-started/primers/service-workers)
- Universal JavaScript (isomorphic rendering)
- Asset Versioning, long term caching, & cache busting for browser that do not support service workers via [node-rev](https://www.npmjs.com/package/node-rev)
- Modern JavaScript syntax with [ES6](https://github.com/lukehoban/es6features) via [buble](https://buble.surge.sh/guide/).
- Performant bundles via [rollup](http://rollupjs.org/).
- Component-based UI architecture via [Preact](https://preactjs.com/).
- Application state management w/time-travel debugging via [Redux](https://github.com/gaearon/redux).
- CSS built with [Sass](http://sass-lang.com/) and optimized with [purify-css](https://github.com/purifycss/purifycss).
- Async actions handled with [redux-thunk](https://github.com/gaearon/redux-thunk), [isomorphic-fetch](https://github.com/matthew-andrews/isomorphic-fetch), and [promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).
- Node server is built with [express](http://expressjs.com/).
- Linting is handled with [Standard](http://standardjs.com/).

### Acknowledgement

Forked from the work started by [Ezekiel Chentnik](https://github.com/ezekielchentnik/preact-pwa)

Original demo (zeit): [https://preact-pwa-yfxiijbzit.now.sh/](https://preact-pwa-yfxiijbzit.now.sh/)

---

License

MIT
