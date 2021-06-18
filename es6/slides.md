---
layout: cover
theme: seriph
background: none
class: text-center
highlighter: shiki
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
title: Welcome to Slidev
---

# es6入门

黄田阳

---
layout: cover
background: none
---

# What is es6?

ECMAScript 6.0（以下简称 ES6）是 JavaScript 语言的下一代标准

---

# 变量声明

- var
- const
- let

<!--
1. 变量提升，暂时性死区
2. 块级作用域
3. with的问题
-->

---

# 函数

1. function函数
2. 箭头函数
3. generator函数
4. async函数

---

# es6 模块

* import
* export

<!--
* import x from "./a.js" 引入模块中导出的默认值。
* import {a as x, modify} from "./a.js"; 引入模块中的变量。
* import * as x from "./a.js" 把模块中所有的变量以类似对象属性的方式引入
* export {a, b, c};
* export default a;
* export * from './a.js'
-->

---
layout: center
---

```javascript
// a.js
export var a = 1;
export function modify() { 
  a = 2;
}
```

```javascript
// b.js
import {a, modify} from "./a.js";
console.log(a);
modify();
console.log(a);
```

---

# 解构

* 数组
* 对象


<!--
# 数组
```javascript
let [a, [[b], c]] = [1, [[2], 3]];
let [a = 1, b = 2] = [, 3];
```
# 对象
```javascript
let { a, b, c } = { a: 'aaa', b: 'bbb' };
let { a: x, b: y } = { a: 'aaa', b: 'bbb' };
```
-->
---
class: text-left
---

# Promise


```javascript

new Promise((resolve, reject) => {
    console.log('初始化');
    resolve();
})
.then(() => {
    throw new Error('有哪里不对了');
    console.log('执行「这个」”');
}, () => {
  console.log(sth. wrong);
})
.catch(() => {
    console.log('执行「那个」');
})
.then(() => {
    console.log('执行「这个」，无论前面发生了什么');
});

```

---

![img](/promises.png)

---

# 数组的遍历

* forEach
* map
* some
* every
* filter
* reduce
* for...of

---
layout: center
class: text-center
---

# Learn More

[Documentations](https://es6.ruanyifeng.com/)
