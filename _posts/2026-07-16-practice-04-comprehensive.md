---
title: "Markdown 练习4 -- HTML 基础学习笔记"
date: 2026-07-13
categories:
  - 学习笔记
tags:
  - HTML
  - Markdown
  - 练习
---

> 这是一篇真实的编程笔记，用到了之前练习过的所有 Markdown 语法。

## 一、什么是 HTML

HTML（HyperText Markup Language）是**网页的结构语言**。它不是编程语言，而是**标记语言**，用标签来描述内容的含义。

我的理解：如果把网页比作一栋房子，HTML 就是**钢筋骨架**，CSS 是**装修**，JavaScript 是**水电系统**。

## 二、常用标签

| 标签 | 作用 | 示例 |
| :--- | :--- | :--- |
| `<h1>` ~ `<h6>` | 标题 | 最大到最小 |
| `<p>` | 段落 | 一段文字 |
| `<a>` | 链接 | `<a href="url">文字</a>` |
| `<img>` | 图片 | 自闭合标签 |
| `<ul>`、`<ol>` | 列表 | 无序和有序 |
| `<div>` | 块级容器 | 布局用 |

## 三、一个完整页面

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>我的页面</title>
</head>
<body>
    <h1>欢迎来到我的网站</h1>
    <p>这是我的第一个网页。</p>
    <ul>
        <li>正在学习 HTML</li>
        <li>下一步学习 CSS</li>
    </ul>
</body>
</html>
```

## 四、学习进度

- [x] HTML 是什么
- [x] 常用标签
- [x] 写一个完整页面
- [ ] CSS 入门
- [ ] 用 CSS 美化这个页面

## 五、推荐资源

- [MDN HTML 教程](https://developer.mozilla.org/zh-CN/docs/Web/HTML) -- 最权威的文档
- [W3Schools](https://www.w3schools.com/) -- 在线练习平台
- [freeCodeCamp](https://www.freecodecamp.org/) -- 免费互动课程

> 学 HTML 最快的方法就是打开编辑器直接写，遇到不会的标签上网查。

## 六、常用快捷键（VS Code）

| 快捷键 | 作用 |
| :--- | :--- |
| `!` + Tab | 生成 HTML 骨架 |
| `Ctrl + /` | 注释/取消注释 |
| `Alt + Shift + F` | 格式化代码 |
| `Ctrl + D` | 选中相同词 |

## 七、小结

通过这四篇 Markdown 练习，我学会了：

1. 基础语法 -- 标题、粗体、列表、链接、引用
2. 表格和任务列表 -- 结构化数据和待办事项
3. 代码块 -- 展示代码示例，带语法高亮
4. 综合写作 -- 用 Markdown 写一篇完整的博客

以后写每篇新文章，都是在复制这篇的框架，然后填充自己的内容。
