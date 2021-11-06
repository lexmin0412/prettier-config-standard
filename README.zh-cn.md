# @youtils/prettier-config-standard

[中文](https://github.com/lexmin0412/youtils-prettier-config-standard/blob/main/README.zh-cn.md) | [English](https://github.com/lexmin0412/youtils-prettier-config-standard/blob/main/README.md)

前端项目通用基础 prettier 配置。

## 安装

```bash
yarn add @youtils/prettier-config-standard -D
```

## 使用

在你的项目根目录下新建 `.prettierrc.js` 文件并添加如下内容：

```js
module.exports = {
	...require('@youtils/prettier-config-standard'),
}
```

## 覆盖配置

```js
module.exports = {
	...require('@youtils/prettier-config-standard'),
	semi: true
}
```

在引入标准配置后将 `semi` 设为 `true` 将会覆盖标准配置。

## 默认配置

此配置中包含了以下配置:

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

标准配置详解：

- `"semi": false`

句尾不接分号。

- `"singleQuote": true`

使用单引号。

- `"useTabs": true`

使用 Tab 作为缩进方式。

- `"tabWidth": 2`

Tab 单级缩进为 2。

- `"jsxSingleQuote": true`

在 jsx 中使用单引号。

- `"bracketSameLine": false`

属性与标签**不**展示在同一行。

- `"printWidth": 80`

单行长度不超过80。

- `"arrowParens": "avoid"`

箭头函数只有单个参数时可省略括号。

点击 [这里](https://prettier.io/docs) 了解更多关于 Prettier 的详情。
