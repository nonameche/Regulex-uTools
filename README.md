# Regulex

**[Regulex](https://jex.im/regulex/)是一个正则表达式解析和可视化工具**

> 本插件改编自开源项目 [Regulex](https://github.com/CJex/regulex)

### Features

![avatar](http://lmsworld.cn/img/1.png)

- 用纯 JavaScript 编写。无需后端。
- 详细的错误消息。在大多数情况下，它可以指出精确的语法错误位置。
- 不支持八进制转义。是的，这是一个功能！ ECMAScript 严格模式不允许在字符串中进行八进制转义，但是许多浏览器仍在正则表达式中允许八进制转义。在 regulex 中，DecimalEscape 将始终被视为反向引用。如果后向引用无效，例如`/ \ 1 /`，`/（\ 1）/`，`/（a）\ 2 /`或 DecimalEscape 出现在字符集中（因为在这种情况下，不能将其解释为反向引用，例如`/（ab）[\ 1] /`，Regulex 总是会抛出错误。
