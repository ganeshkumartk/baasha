# Baasha ![npm](https://img.shields.io/npm/v/baasha.svg) [![HitCount](http://hits.dwyl.io/coderganesh/baasha.svg)](http://hits.dwyl.io/coderganesh/baasha)

![Baasha](https://m.media-amazon.com/images/S/aplus-seller-content-images-us-east-1/ATVPDKIKX0DER/A1DQ4YPN2B87YV/959fae1b-5f1d-4c7e-8ddb-ac1a5d5c0459._CR120,0,360,180_PT0_SX350__.png) [![NPM](https://nodei.co/npm/baasha.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/baasha/)

[![forthebadge](https://forthebadge.com/images/badges/built-with-swag.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/its-not-a-lie-if-you-believe-it.svg)](https://forthebadge.com)[![forthebadge](https://forthebadge.com/images/badges/made-with-javascript.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/just-plain-nasty.svg)](https://forthebadge.com)[![forthebadge](https://forthebadge.com/images/badges/powered-by-netflix.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/makes-people-smile.svg)](https://forthebadge.com)
# Need a product name? Ask Baasha!

![baasha](https://pbs.twimg.com/media/B7PM45ZIYAA1bpN.jpg)

Coming up with good product names that are marketable, unique, and memorable is
hard. Let Baasha help!

Baasha has already done the grunt work of figuring out which words make the best
product names and will generate a magical combination from this curated set...
every time, guaranteed!

What are you waiting for? Put Baasha to the test!

## Install

As CLI:

```
npm install -g baasha
```

As module:

```
npm install --save baasha
```

```js
var baasha = require('baasha')
```

## Examples

### Ask Baasha for a product name

```console
$ baasha
We'll call it... ProGear
```

### Ask for 5 product names

```console
$ baasha --exactly 5
We'll call it... NexSpin... TaxThink... WatchWeb... TeamSlick... WorkSat
```

### Let baasha choose between 2 and 10 names

```console
$ baasha --min 2 --max 10
We'll call it... MapAlert... InstaFleet... PayTax... SafeAlert
```

### Have Baasha generate names until you find something specific you're looking for

Kill with Ctrl C

```console
$ baasha --forever --brief --interval 50 | grep Best
BestGear
DataBest
NexBest
```

### Get CLI help content

```console
$ baasha --help
```

## API

### baasha([options], [callback(error, results)])
### baasha.sync([options])

Generate product names.

The asynchronous version will call a given callback or, if not given, return a
[`Promise`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).

The synchronous version will return results immediately.

Each product name will be returned as either a string (default) or an object
(based on the `object` boolean option). If there are multiple generated names,
an array will be returned, unless the `join` string option is given, in which
case a string of joined names will be returned.

### options

Based on [random-words](https://www.npmjs.com/package/random-words).

- `exactly`: number

    Generate exactly this many product names.

- `min`: number

    Generate at least this many product names.

- `max`: number

    Generate at most this many product names.

- `join`: string

    Call join on the results array using this string.

- `object`: boolean

    Use an object for each result element instead of a string. The object will
    have a `left` property and `right` property as strings, representing the
    word combo that makes the name.

## License

MIT

## Disclaimer

This module was created for fun but should definitely be taken seriously. ✌
