# prettier-config [![NPM version](https://img.shields.io/npm/v/@stackbit/prettier-config.svg)](https://www.npmjs.com/package/@stackbit/prettier-config)

Stackbit's [shareable config](https://prettier.io/docs/en/configuration.html#sharing-configurations) for [Prettier](https://prettier.io/)

## Installation

Install Prettier and `@stackbit/prettier-config`:

```
npm install --save-dev prettier @stackbit/prettier-config
```

## Usage

Stackbit's Prettier rules come bundled in `@stackbit/prettier-config`. To enable these rules, add a `prettier` property in your `package.json`. See the [Prettier configuration docs](https://prettier.io/docs/en/configuration.html) for more details.

```json
"prettier": "@stackbit/prettier-config"
```

If you don't want to use `package.json`, you can use any of the supported extensions to export a string:

```jsonc
// `.prettierrc.json`
"@stackbit/prettier-config"
```

```javascript
// `prettier.config.js` or `.prettierrc.js`
module.exports = '@stackbit/prettier-config';
```

## Extending

This configuration is not intended to be changed, but if you have a setup where modification is required, it is possible. Prettier does not offer an "extends" mechanism as you might be familiar from tools such as ESLint.

To extend a configuration you will need to use a `prettier.config.js` or `.prettierrc.js` file that exports an object:

```javascript
module.exports = {
  ...require('@stackbit/prettier-config'),
  semi: false
};
```

## Changelog

Changes are recorded in [`CHANGELOG.md`](CHANGELOG.md).

## License

Distributed under the MIT License. See [`LICENSE`](LICENSE) for more information.
