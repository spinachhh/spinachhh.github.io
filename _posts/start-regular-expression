---
layout: post
title: 正则表达式初入门
data: 2020-08-17
author: "zzw"
catalog: true
tags:
    - 随笔
---
#### 正则表达式初入门
正则表达式是用于匹配字符串中字符组合的模式，在javascript中也用于[replace()](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/String/replace "replace()"),[split()](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/String/split "split()")等方法。

------------

#### 创建正则表达式
1. 表达式包含在两个斜杠之间，如` /a+b/`
2. `RegExp("ab+c")`

#### 常见的特殊字符
- `\b`  匹配一个词的边界
- `\s`  匹配一个空白字符，包括空格、制表符、换页符和换行符
- `\d`  匹配一个数字
- `g`   正则表达式标识：全局搜索
- `i`   正则表达式标识：忽略大小写

示例：
`/\d\s/g`   全局匹配数字后带空格的部分，
```javascript
    var re = /\d\s/g;
    var str = "15000 5 666 2";
    console.log(str.match(re));
```
这段代码将输出` ["0 ", "5 ", "6 "]`

------------

详细更多常见的字符，可参考[正则表达式中各种字符的含义](https://www.cnblogs.com/afarmer/archive/2011/08/29/2158860.html "正则表达式中各种字符的含义")和[正则表达式](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Guide/Regular_Expressions "正则表达式")
