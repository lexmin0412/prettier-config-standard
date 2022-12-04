# @lexmin0412/prettier-config-standard

[English](https://github.com/lexmin0412/youtils-prettier-config-standard/blob/main/README.md) | [中文](https://github.com/lexmin0412/youtils-prettier-config-standard/blob/main/README.zh-cn.md)

Universal and common prettier configuration for your frontend projects.

## Install

```bash
yarn add @lexmin0412/prettier-config-standard -D
```

## Usage

Add `.prettierrc.js` in you project's root directory:

```js
module.exports = {
	...require('@lexmin0412/prettier-config-standard'),
}
```

## Override

```js
module.exports = {
	...require('@lexmin0412/prettier-config-standard'),
	semi: true
}
```

set `semi` to `true` after require `@lexmin0412/prettier-config-standard` will override standard configurations.

## Default Configuration

there are some configuration items defined:

```json
{
	"printWidth": 100,
	"useTabs": true,
	"tabWidth": 2,
	"semi": false,
	"singleQuote": true,
	"quoteProps": "as-needed",
	"jsxSingleQuote": false,
	"trailingComma": "all",
	"bracketSpacing": true,
	"bracketSameLine": false,
	"arrowParens": "avoid",
	"proseWrap": "never",
	"htmlWhitespaceSensitivity": "css",
	"vueIndentScriptAndStyle": false,
	"endOfLine": "lf",
	"embeddedLanguageFormatting": "auto",
	"singleAttributePerLine": true
}
```

Click [Here](https://prettier.io/docs) to get more details about Prettier.
