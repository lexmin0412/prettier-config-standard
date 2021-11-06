# @youtils/prettier-config-standard

[English](https://github.com/lexmin0412/youtils-prettier-config-standard/blob/main/README.md) | [中文](https://github.com/lexmin0412/youtils-prettier-config-standard/blob/main/README.zh-cn.md)

Universal and common prettier configuration for your frontend projects.

## Install

```bash
yarn add @youtils/prettier-config-standard -D
```

## Usage

Add `.prettierrc.js` in you project's root directory:

```js
module.exports = {
	...require('@youtils/prettier-config-standard'),
}
```

## Override

```js
module.exports = {
	...require('@youtils/prettier-config-standard'),
	semi: true
}
```

set `semi` to `true` after require `@youtils/prettier-config-standard` will override standard configurations.

## Default Configuration

there are some configuration items defined:

```json
{
	"semi": false,
	"singleQuote": true,
	"useTabs": true,
	"tabWidth": 2,
	"jsxSingleQuote": true,
	"bracketSpacing": true,
	"bracketSameLine": false,
	"printWidth": 80,
	"arrowParens": "avoid"
}
```

Click [Here](https://prettier.io/docs) to get more details about Prettier.
