# prettier-config

Stackbit's [shareable config](https://prettier.io/docs/en/configuration.html#sharing-configurations) for prettier

## Installation

Install [prettier](https://prettier.io/) and `@stackbit/prettier-config`:

```
npm install --save-dev prettier @stackbit/prettier-config
```

## Usage
Stackbit's prettier rules come bundled in `@stackbit/prettier-config`. To enable these rules, add a `prettier` property in your `package.json`. See the [prettier configuration docs](https://prettier.io/docs/en/configuration.html) for more details.

```
"prettier": "@stackbit/prettier-config"
```

If you don't want to use `package.json`, you can use any of the supported extensions to export a string:

```
// `.prettierrc.json`
"@stackbit/prettier-config"
```

```
// `prettier.config.js` or `.prettierrc.js`
module.exports = '@stackbit/prettier-config'
```

## [CHANGELOG](CHANGELOG.md)

## [LICENSE](LICENSE)
