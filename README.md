# `eslint-config-mailonline`

[![NPM version](http://img.shields.io/npm/v/eslint-config-mailonline.svg?style=flat-square)](https://www.npmjs.org/package/eslint-config-mailonline)

MailOnline ESLint configuration.

## Usage

Add `eslint-config-mailonline` as a development dependency:

```bash
npm install eslint-config-mailonline --save-dev
```

Create ESLint configuration file (`eslint.config.js`) that extends `eslint-config-mailonline`:

```js
// eslint.config.[m]js
import baseMailonlineConfig from "eslint-config-mailonline";

export default [{
  ...baseMailonlineConfig,
  // additional config here
];
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

### mocha

```js
module.exports = {
  "extends": "mailonline/mocha"
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
