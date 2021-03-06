# Event bus
[![NPM version](https://img.shields.io/npm/v/zax-eventbus.svg?style=flat)](https://www.npmjs.com/package/zax-eventbus)
[![Build Status](https://travis-ci.org/jsonchou/zax-eventbus.svg?branch=master)](https://travis-ci.org/jsonchou/zax-eventbus)
[![codecov](https://codecov.io/gh/jsonchou/zax-eventbus/branch/master/graph/badge.svg)](https://codecov.io/gh/jsonchou/zax-eventbus)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)

A subscribe & pubscribe module

## Browsers support

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="IE / Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>IE / Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Safari | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari-ios/safari-ios_48x48.png" alt="iOS Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>iOS Safari | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/opera/opera_48x48.png" alt="Opera" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Opera |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| IE8+ Edge+                                                                                                                                                                                                      | last 10 versions                                                                                                                                                                                                  | last 10 versions                                                                                                                                                                                              | last 2 versions                                                                                                                                                                                               | last 2 versions                                                                                                                                                                                                               | last 2 versions                                                                                                                                                                                           |

## Install

```bash
yarn add zax-eventbus --save
```

## Usage

```tsx
import EventBus, { EventHandler, EventHandlers, EventOptions, EventSource } from 'zax-eventbus'

const eventbus = new EventBus({
	channel: 'default',
	debug: false
})

eventbus.on('foo', handler)
eventbus.once('qux', handler)
eventbus.emit('foo', 'bar')
eventbus.off('foo')
eventbus.get('foo')
eventbus.has('foo')
eventbus.keys()
eventbus.values()
eventbus.remove('foo')
eventbus.removeAll()
```
