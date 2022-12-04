# @lexmin0412/prettier-config-standard

[中文](https://github.com/lexmin0412/youtils-prettier-config-standard/blob/main/README.zh-cn.md) | [English](https://github.com/lexmin0412/youtils-prettier-config-standard/blob/main/README.md)

前端项目通用基础 prettier 配置。

## 安装

```bash
pnpm add @lexmin0412/prettier-config-standard -D
```

## 使用

在你的项目根目录下新建 `.prettierrc.js` 文件并添加如下内容：

```js
module.exports = {
	...require('@lexmin0412/prettier-config-standard'),
}
```

## 覆盖配置

```js
module.exports = {
	...require('@lexmin0412/prettier-config-standard'),
	semi: true
}
```

在引入标准配置后将 `semi` 设为 `true` 将会覆盖标准配置。

## 默认配置

此配置中包含了以下配置项:

```json
{
	"printWidth": 100, // 单行最大长度
	"useTabs": true, // 使用tab
	"tabWidth": 2, // tab step
	"semi": false, // 禁用行尾分号
	"singleQuote": true, // 使用单引号
	"quoteProps": "as-needed", // 当从对象中解构属性时按需添加引号
	"jsxSingleQuote": false, // jsx使用双引号
	"trailingComma": "all", // 所有参数都允许尾逗号
	"bracketSpacing": true, // 括号两端是否需要空格
	"bracketSameLine": false, // jsx标签的闭合标签使用单独的一行（避免添加属性造成版本控制系统的多行冲突）
	"arrowParens": "avoid", // 箭头函数参数总是使用括号包裹（避免冲突）
	"proseWrap": "never", // 是否在markdown文件中根据printWidth来处理换行
	"htmlWhitespaceSensitivity": "css", // 去除html中的无用空格
	"vueIndentScriptAndStyle": false, // vue模版中的script和style标签内部代码是否需要默认缩进,
	"endOfLine": "lf", // linux风格的行尾结束符
	"embeddedLanguageFormatting": "auto", // 开启内嵌代码（如js中的html, vue中的js等）的自动格式化
	"singleAttributePerLine": true // 在HTML, Vue and JSX中单行只写一个属性
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
