# BEE TSLint 规则

此项目为所有的 BEE 项目提供一致的基础 [tslint](https://github.com/palantir/tslint) 规则。

## 使用方式

### 安装

安装包：

```shell
npm install @bee/tslint-rules --save-dev
```

### 配置

将 *@bee/tslint-rules* 作为您 `tslint.json` 的一个扩展：

```json
{
  "extends": "@bee/tslint-rules"
}
```

如果需要扩展多个规则集，您可以将 `extends` 定义为一个字符串数组：

```json
{
  "extends": [
    "@bee/tslint-rules",
    "another-tslint-ruleset"
  ]
}
```

访问 [configuring tslint](https://palantir.github.io/tslint/usage/configuration/) 以获取更多配置详情。
