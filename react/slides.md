---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: "text-center"
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
---

# React

黄田阳

---
layout: cover
---

# What is React?

### React 是一个声明式，高效且灵活的用于构建用户界面的 JavaScript 库。使用 React 可以将一些简短、独立的代码片段组合成复杂的 UI 界面，这些代码片段被称作“组件”。

### 以下我们先用 create-react-app 创建一个 react app。

<!--
1. npm install yarn -g --registry https://registry.npm.taobao.org
2. npm install yrm -g --registry https://registry.npm.taobao.org
3. yarn create react-app my-app
4. yarn enject
5. yarn start
-->

---

# 核心概念

- 📝 **JSX**
- 🎨 **元素渲染**
- 🧑‍💻 **组件和 props**
- 🤹 **state 和声明周期**
- 🎥 **事件处理**
- 📤 **条件渲染**
- 🛠 **列表 & Key**
- ⬆️ **状态提升**

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent; 
  -moz-text-fill-color: transparent;
}
</style>

---
layout: cover
---

# JSX

<style>
h1 {
  color: white
}
</style>

<!--
# 什么是JSX
# 在 JSX 中嵌入表达式
# JSX 也是一个表达式
# JSX属性
-->

---
layout: cover
---

# 元素渲染

<!--
# 将一个元素渲染为 DOM
# 更新已渲染的元素
-->

---
layout: cover
---

# 组件和props

---

## 函数组件与 class 组件

* 函数组件

```javascript
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```

* class组件

```javascript
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

---
layout: cover
---

## 渲染组件

<!--
# 组件名首字母必须大写
# 组合组件
# 提取组件
-->

---

# state和生命周期

1. 向 class 组件中添加局部的 state
2. 添加声明周期
3. state的注意事项
4. 数据的流动

---
layout: cover
---

# 事件处理

<!--
# 添加点击事件
# 添加参数
-->

---
layout: cover
---

# 条件渲染

<!--
# 元素变量
# &&
# 三目表达式
# 组织渲染
-->

---
layout: cover
---

# 列表和key

<!--
# 列表
# key
-->

---
layout: cover
---

# 状态提升

---

# 课后作业

* 阅读 [https://zh-hans.reactjs.org/docs/thinking-in-react.html](https://zh-hans.reactjs.org/docs/thinking-in-react.html)
* 自行开发一个待办事项应用
