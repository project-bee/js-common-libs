# SLIME Prettier 规则

此项目为所有的 SLIME 项目提供一致的基础 [Prettier](https://prettier.io) 规则。

## 使用方式

### 安装

安装包：

```shell
npm install slime-prettier-rules --save-dev
```

### 配置

您可以选择以下方式来使用我们提供的 Prettier 规则：

#### package.json

您可以直接在项目根目录中的 `package.json` 文件里完成配置：

```json
{
  "name": "my-cool-library",
  "version": "9000.0.1",
  "prettier": "slime-prettier-rules"
  ...
}
```

#### Prettier 配置文件

如果您不愿意使用 `package.json` 文件，您还可以使用独立的 Prettier 配置文件，比如 `.prettierrc.json`：

```json
"slime-prettier-rules"
```

但是以上的方法都没有提供规则的改写，如您需要改写部分规则，请在 `.prettierrc.js` 或 `prettier.config.js` 文件中改写部分规则并导出最终的修改：

```js
module.exports = {
  ...require('slime-prettier-rules'),
  semi: false
};
```

访问 [Prettier Options](https://prettier.io/docs/en/options.html) 以获取更多规则详情。
