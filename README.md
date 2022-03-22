# krypto.mn

## Table of Contents

-   [Install](#install)
-   [Usage](#usage)
-   [API](#api)
-   [License](#license)

## Install

```sh
$ npm install krypto-api-sdk
# OR
$ yarn add krypto-api-sdk
```

## Usage

```js
const Krypto = require('krypto-spi-sdk')

const apiKey = 'api key'
const client = new Krypto(apiKey)

client.getTags().then(console.log).catch(console.error)
client.getGainers(0, 100).then(console.log).catch(console.error)
```

## API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

-   [getQuotesLatest](#getQuoteLatest)
    -   [Parameters](#parameters-1)
    -   [Examples](#examples-1)
-   [getGainers](#getGainers)
    -   [Parameters](#parameters-2)
    -   [Examples](#examples-2)
-   [getRecent](#getRecent)
    -   [Parameters](#parameters-3)
    -   [Examples](#examples-3)
-   [getLatest](#getLatest)
    -   [Parameters](#parameters-4)
    -   [Examples](#examples-4)
-   [getTags](#getTags)
    -   [Parameters](#parameters-5)
    -   [Examples](#examples-5)
-   [getMetricsQuotes](#getMetricsQuotes)
    -   [Parameters](#parameters-6)
    -   [Examples](#examples-6)
-   [getNews](#getNews)
    -   [Parameters](#parameters-7)
    -   [Examples](#examples-7)
-   [getFearGreed](#getFearGreed)
    -   [Parameters](#parameters-8)
    -   [Examples](#examples-8)
-   [getInfo](#getInfo)
    -   [Parameters](#parameters-9)
    -   [Examples](#examples-9)
-   [getExchangeInfo](#getExchangeInfo)
    -   [Parameters](#parameters-10)
    -   [Examples](#examples-10)
-   [getMarketPairs](#getMarketPairs)
    -   [Parameters](#parameters-11)
    -   [Examples](#examples-11)
-   [getExchangeMarketPairs](#getExchangeMarketPairs)
    -   [Parameters](#parameters-12)
    -   [Examples](#examples-12)
-   [getExchangeListings](#getExchangeListings)
    -   [Parameters](#parameters-13)
    -   [Examples](#examples-13)
-   [getSingleNews](#getSingleNews)
    -   [Parameters](#parameters-14)
    -   [Examples](#examples-14)
-   [getFiatMap](#getFiatMap)
    -   [Parameters](#parameters-15)
    -   [Examples](#examples-15)
-   [getCryptoMap](#getCryptoMap)
    -   [Parameters](#parameters-16)
    -   [Examples](#examples-16)
-   [getTrending](#getTrending)
    -   [Parameters](#parameters-17)
    -   [Examples](#examples-17)
-   [getConvertion](#getConvertion)
    -   [Parameters](#parameters-18)
    -   [Examples](#examples-18)


### getQuoteLatest


#### Parameters

-   `url`   /cryptocurrency/quotes/latest
-   `options` (Object) Options for the request:
    -   `options.slug` (String)
    -   `options.symbol` (String)
    -   `options.id` (Array<Integer>)

#### Examples

```javascript
const client = new CoinMarketCap('api key')
client.getQuoteLatest(query).then(console.log).catch(console.error)
```

### getGainers


#### Parameters

-   `url`   /cryptocurrency/listings/gainers
-   `options` (Object) Options for the request:
    -   `options.start` (Integer)
    -   `options.end` (Integer)

#### Examples

```javascript
const client = new CoinMarketCap('api key')
client.getGainers(query).then(console.log).catch(console.error)
```
    
### getRecent


#### Parameters

-   `url`   /cryptocurrency/listings/recent
-   `options` (Object) Options for the request:
    -   `options.start` (Integer)
    -   `options.end` (Integer)

#### Examples

```javascript
const client = new CoinMarketCap('api key')
client.getRecent(query).then(console.log).catch(console.error)
```
    
### getLatest


#### Parameters

-   `url`   /cryptocurrency/listings/latest
-   `options` (Object) Options for the request:
    -   `options.start` (Integer)
    -   `options.end` (Integer)

#### Examples

```javascript
const client = new CoinMarketCap('api key')
client.getLatest(query).then(console.log).catch(console.error)
```
    
### getTags


#### Parameters

-   `url`   /cryptocurrency/listings/latest

#### Examples

```javascript
const client = new CoinMarketCap('api key')
client.getLatest().then(console.log).catch(console.error)
```
    
### getMetricsQuotes


#### Parameters

-   `url`   /cryptocurrency/listings/latest

#### Examples

```javascript
const client = new CoinMarketCap('api key')
client.getMetricsQuotes().then(console.log).catch(console.error)
```
    
    
## License

Licensed under the MIT License.
