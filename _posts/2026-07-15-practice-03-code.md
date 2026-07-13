---
title: "Markdown 练习3 -- 代码块和技术写作"
date: 2026-07-15
categories:
  - 学习笔记
tags:
  - Markdown
  - 练习
  - 代码
---

> 本练习覆盖：行内代码、代码块、语法高亮

## 一、行内代码

设置 Git 用户名用 `git config --global user.name "your name"`。
打印内容用 Python 的 `print()` 函数。
检查当前目录文件用 `ls` 命令。

## 二、代码块

### 2.1 不指定语言的通用代码块

```
def hello():
    print("Hello, World!")
```

### 2.2 带语法高亮的代码块

```python
def fibonacci(n):
    """计算斐波那契数列"""
    if n <= 1:
        return n
    return fibonacci(n-1) + fibonacci(n-2)

# 输出前 10 个数
for i in range(10):
    print(fibonacci(i))
```

```html
<!DOCTYPE html>
<html>
<head>
    <title>我的第一个网页</title>
</head>
<body>
    <h1>Hello World!</h1>
</body>
</html>
```

```css
body {
    font-family: sans-serif;
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
    background: #f5f5f5;
}
```

```javascript
function greet(name) {
    return `你好, ${name}!`;
}
console.log(greet("王梦越"));
```

```bash
# 创建项目目录
mkdir my-project
cd my-project
git init
echo "# My Project" > README.md
```

## 三、代码中嵌入链接和说明

学习 HTML 时首先要理解基本结构：

```html
<!-- 这是一个注释 -->
<p>这是一个 <strong>段落</strong></p>
```

更多 HTML 标签可以参考 [MDN 文档](https://developer.mozilla.org/zh-CN/docs/Web/HTML)。

## 四、今日收获

- 行内代码用单个反引号 `` `code` ``
- 代码块用三个反引号 ``` ``` `包裹`
- 在第一个反引号后加语言名（如 ` ```python`）即可高亮
- 支持的语言：`python`、`html`、`css`、`javascript`、`bash`、`yaml`、`json` 等
