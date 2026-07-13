---
title: "Markdown 语法速查与进阶"
date: 2026-07-13
categories:
  - 学习笔记
tags:
  - Markdown
  - 教程
---

> 这篇文章本身就是用 Markdown 写的。你在 GitHub 上打开 `.md` 源文件，对照着页面的渲染效果看，学得最快。
>
> 源文件位置：`_posts/2026-07-13-markdown-guide.md`

## 一、你已经会的基础语法

| 语法 | 写法 | 效果 |
|------|------|------|
| **标题** | `# H1` 到 `###### H6` | 6 级标题 |
| **粗体** | `**文字**` | **粗体** |
| **斜体** | `*文字*` | *斜体* |
| **链接** | `[文字](url)` | [GitHub](https://github.com) |
| **图片** | `![描述](url)` | 展示图片 |
| **无序列表** | `- 项目` 或 `* 项目` | 圆点列表 |
| **有序列表** | `1. 项目` | 数字列表 |
| **引用** | `> 引用内容` | 缩进引用块 |
| **分割线** | `---` | 水平线 |
| **行内代码** | `` `代码` `` | `代码` |
| **代码块** | 三个反引号包裹 | 带高亮的代码块 |

## 二、进阶语法

### 1. 表格

```
| 左对齐 | 居中 | 右对齐 |
| :----- | :--: | -----: |
| 苹果   | 香蕉 | 樱桃   |
| 1      | 2    | 3      |
```

渲染效果：

| 左对齐 | 居中 | 右对齐 |
| :----- | :--: | -----: |
| 苹果   | 香蕉 | 樱桃   |
| 1      | 2    | 3      |

### 2. 任务列表

```
- [x] 已完成的事
- [ ] 未完成的事
- [ ] 另一个待办
```

- [x] 学会基础 Markdown
- [x] 搭建个人网站
- [ ] 掌握进阶语法 ← 就是这篇
- [ ] 写 10 篇博客

### 3. 删除线

```
~~这行字被划掉了~~
```

~~这行字被划掉了~~

### 4. 代码块 + 语法高亮

````
```python
def hello():
    print("Hello, World!")
```
````

```python
def hello():
    print("Hello, World!")
```

支持的语言包括：`python`, `javascript`, `html`, `css`, `bash`, `yaml`, `json` 等。

### 5. 在 Markdown 里嵌入 HTML

Markdown 允许直接写 HTML 标签，所以你可以做更多事情：

```html
<details>
  <summary>点击展开</summary>
  这里是隐藏的内容，点击后才显示。
</details>
```

<details>
  <summary>点击展开</summary>
  这里是隐藏的内容，点击后才显示。
</details>

### 6. 行内 HTML 加样式

```html
<span style="color: red;">红色文字</span>
```

<span style="color: red;">红色文字</span>

<span style="color: blue; font-weight: bold;">蓝色加粗文字</span>

### 7. 锚点链接（页面内跳转）

```
[跳转到表格部分](#1-表格)
```

[跳转到表格部分](#1-表格)

### 8. Emoji

GitHub 支持用 `:emoji_code:` 插入表情：

```
:smile: :rocket: :+1: :fire:
```

:smile: :rocket: :+1: :fire:

完整列表：https://github.com/ikatyang/emoji-cheat-sheet

### 9. 自动链接

```
直接写网址：https://github.com
邮箱：example@example.com
```

直接写网址：https://github.com  
邮箱：example@example.com

## 三、Jekyll 特有的 Front Matter

你每篇文章顶部的 `---` 包裹的内容就是 Front Matter，它用 YAML 格式定义文章属性：

```yaml
---
title: "文章标题"
date: 2026-07-13
categories:
  - 分类1
  - 分类2
tags:
  - 标签A
  - 标签B
published: true
---
```

常用字段：

| 字段 | 作用 |
|------|------|
| `title` | 文章标题 |
| `date` | 发布日期 |
| `categories` | 分类（可多个） |
| `tags` | 标签（可多个） |
| `published` | 设为 `false` 可隐藏草稿 |

## 四、写新文章的标准流程

1. 在 `_posts` 文件夹新建文件，命名规则：`YYYY-MM-DD-英文标题.md`
2. 写上 Front Matter（标题、日期、分类）
3. 用 Markdown 写正文
4. 推送到 GitHub
5. 访问网站就能看到新文章了

---

> **进阶建议**：别一次性背完所有语法。每次写文章时想用一个新效果（比如表格），就去查这篇对照着写，写两三次就记住了。
