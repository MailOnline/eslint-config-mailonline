# `eslint-config-mailonline`

[![NPM version](http://img.shields.io/npm/v/eslint-config-mailonline.svg?style=flat-square)](https://www.npmjs.org/package/eslint-config-mailonline)

`eslint-config-mailonline` is a shared ESLint configuration used by MailOnline. This configuration includes rules for ES6, React, Jest, Lodash, and Webpack.

## Prerequisites

- Node.js v18.18 or higher

## Installation

Add `eslint-config-mailonline` as a development dependency:

For *npm* users:
```bash
npm install eslint-config-mailonline --save-dev
```

For *Yarn* users:
```bash
yarn add eslint-config-mailonline --dev
```

Please note that there is no requirement to install stylelint independently in the parent package. This is because it is included as a dependency within this library and will be hoisted to the parent package.

## Usage

Create ESLint configuration file (`eslint.json`) that extends `eslint-config-mailonline`:

```js
{
  "extends": "mailonline",
}
```

## Extended configs

The package also has separate entry points for some environments. Simply extend from the entry point as described below,
either in a folder-specific eslint config, or additionally to the root config, e.g.:

```js
module.exports = {
  "extends": [
    "mailonline",
    "mailonline/jest",
    "mailonline/react"
  ]
};
```

### jest

```js
module.exports = {
  "extends": "mailonline/jest"
};
```

### react

```js
module.exports = {
  "extends": "mailonline/react"
};
```

### lodash

```js
module.exports = {
  "extends": "mailonline/lodash"
};
```

### webpack

```js
module.exports = {
  "extends": "mailonline/webpack"
};
```

## Breaking changes

Any changes to this package that might cause code using it to not validate anymore, will be a semver-major change.
