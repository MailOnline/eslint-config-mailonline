# `eslint-config-mailonline`

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

## Breaking changes

Any changes to this package that might cause code using it to not validate anymore, will be a semver-major change.
