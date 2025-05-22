# 🍻 贡献小手册

多人开发维护的项目，代码规范是必须有的，有利于项目的维护管理，前端有很多工具帮助我们完成这项任务例如 eslint、prettier 等。

## 🧋 代码规范

实际项目中一般采用 npm 或者其它的包管理器安装依赖的方式，确保多人合作时保证最终代码格式的统一。

本项目使用了以下工具：

- [Eslint](https://eslint.org/)： ECMAScript/JavaScript 代码格式审查，兼有部分修复功能
- [Stylelint](https://stylelint.io/)： CSS 代码检查
- [eslint-config-prettier](https://github.com/prettier/eslint-config-prettier)：关闭所有可能干扰 Prettier 规则的 ESLint 规则。
- [eslint-plugin-prettier](https://github.com/prettier/eslint-plugin-prettier)：将 Prettier 规则转换为 ESLint 规则。
- [eslint-plugin-vue](https://github.com/vuejs/eslint-plugin-vue)： Eslint 针对 Vue 的模版语法检查
- [Prettier](https://prettier.io/)： 代码格式化/代码美化

:::tip 说明

- VSCode 中安装的相关插件只是为了 **个人使用方便**，因为不是所有人开发都会使用 VSCode；即便使用，也不一定人人都安装这些插件。
- `xxxlint` 的工具一般都是检查规范的，出现语法问题时，会得到类似波浪线的提示，从而引起开发人员注意并修改。比如 markdownlint、scss-lint 等等。Linting 是一种静态分析，用于发现不符合某些样式准则的问题模式和代码。
- Prettier 格式化时主观性很强（有自己的格式化方式，我们无法配置某些样式和风格），可能和我们个人或者团队的某些方面 “意见不合”。
- 由于同时使用 Eslint + Prettier 时会出现部分配置或者说风格上的差异，会出现冲突。我们会使用一些像 `eslint-config-prettier`、`eslint-plugin-prettier` 的 npm 包，前者帮助我们关闭冲突配置，后者将 Prettier 作为 lint 的插件使用。但是使用这些插件有一个副作用，你可能会在项目中看到一些红波浪线，即便代码本身并没有错。
- ESLint、Prettier 流畅配合不是一件容易的事情，如果向往足够简单，使用 `eslint-config-prettier` 或者 [prettier-eslint](https://github.com/prettier/prettier-eslint) 就好。

:::

## PR

![PR](/pr-workflow.png)

:::tip

使用最新版的 Edge 浏览器把鼠标光标置于图像之上，按下两次 Ctrl 有惊喜！😜

:::
