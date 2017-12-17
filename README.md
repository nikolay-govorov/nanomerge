# Nano Merge

[![Build Status](https://travis-ci.org/nikolay-govorov/nanomerge.svg?branch=master)](https://travis-ci.org/nikolay-govorov/nanomerge)
[![License](https://img.shields.io/npm/l/nanomerge.svg)](https://www.npmjs.com/package/nanomerge)
[![GitHub package version](https://img.shields.io/github/package-json/v/nikolay-govorov/nanomerge.svg)](https://github.com/nikolay-govorov/nanomerge)

Tiny universal isomorphic library for deep merging objects

### Install

```sh
npm install --save nanomerge
```

### Usage

```js
var nanomerge = require('nanomerge');

// Merge many objects
nanomerge({ a: 1, b: 2 }, { a: 2, c: 3 }, { b: 5, d: 7 }); // { a: 2, b: 5, c: 3, d: 7 }

// Custom configuration
nanomerge({ clone: true })({ a: 1 }, { b: 2 }) // { a: 1, b: 2 }
```

### Configuration
