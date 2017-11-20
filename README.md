# `eslint-config-mailonline`

[![Greenkeeper badge](https://badges.greenkeeper.io/MailOnline/eslint-config-mailonline.svg)](https://greenkeeper.io/)

[![NPM version](http://img.shields.io/npm/v/eslint-config-mailonline.svg?style=flat-square)](https://www.npmjs.org/package/eslint-config-mailonline)
[![Travis build status](http://img.shields.io/travis/MailOnline/eslint-config-mailonline/master.svg?style=flat-square)](https://travis-ci.org/MailOnline/eslint-config-mailonline)

MailOnline ESLint configuration.

## Usage

Add `eslint-config-mailonline` as a development dependency:

```bash
npm install eslint-config-mailonline --save-dev
```

Create ESLint configuration file (`.eslintrc`) that extends `eslint-config-mailonline`:

```json
{
  "extends": "mailonline"
}
```

## Extended configs

The package also has separate entry points for some environments. Simply extend from the entry point as described below,
either in a folder-specific eslint config, or additionally to the root config, e.g.:

```json
{
  "extends": [
    "mailonline",
    "mailonline/jest",
    "mailonline/react"
  ]
}
```

### jest

```json
{
  "extends": "mailonline/jest"
}
```

### mocha

```json
{
  "extends": "mailonline/mocha"
}
```

### react

```json
{
  "extends": "mailonline/react"
}
```

### flowtype

```json
{
  "extends": "mailonline/flowtype"
}
```

### lodash

```json
{
  "extends": "mailonline/lodash"
}
```

### webpack

```json
{
  "extends": "mailonline/webpack"
}
```

## Breaking changes

Any changes to this package that might cause code using it to not validate anymore, will be a semver-major change.
