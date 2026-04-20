---
title: Hexo 博客多格式元素指南-fix-t
date: 2026-04-20 23:33:00
tags: [Hexo, Butterfly, Markdown]
categories: 教程
description: 本文展示了如何在 Hexo 博客中优雅地呈现代码、数学公式、图片、链接以及其他常用格式。
---

欢迎来到自动化博客第一章！为了测试 Butterfly 主题的强大渲染能力，我准备了这篇包含多种常用排版格式的指南。

<!-- more -->

## 1. 代码块 (Code Blocks)

Hexo 支持多种语言的高亮显示。

```python
def say_hello(name):
    """一个简单的 Python 示例"""
    message = f"Hello, {name}! Welcome to Jane's Blog."
    print(message)
    return message

say_hello("World")
```

```bash
# 停止占用 4000 端口的进程
lsof -i :4000 | awk 'NR!=1 {print $2}' | xargs kill -9
```

## 2. 数学公式 (Math Formula)

Butterfly 主题支持 LaTeX 公式渲染（通常需要开启插件如 `hexo-renderer-kramed` 或 `hexo-math`）。

**行内公式**：例如质能方程 $E = mc^2$。

**块级公式**：

$$
\frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

$$
I = \int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}
$$

## 3. 图片展示 (Images)

你可以使用 Markdown 语法或 Butterfly 特有的标签。

**本地图片**：
![我的背景图](/img/my_bg.jpg)
*图：这是我们之前配置的首页背景图*

**外链图片**：
![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)

## 4. 链接与引用 (Links & Quotes)

**普通链接**：[访问 Jane-QX 的 GitHub](https://github.com/Jane-QX)

**引用块**：
> “Stay Hungry, Stay Foolish.” —— Steve Jobs

## 5. 列表与表格 (Lists & Tables)

**有序列表**：
1. 学习 Hexo 基础
2. 配置 Butterfly 主题
3. 部署到 GitHub Pages

**表格示例**：

| 工具 | 用途 | 状态 |
| :--- | :--- | :--- |
| Hexo | 静态博客框架 | 已安装 |
| Butterfly | 主题皮肤 | 已配置 |
| Actions | 自动部署 | 已开启 |

## 6. 特殊标签 (Butterfly Tags)

Butterfly 提供了许多漂亮的卡片标签：

{% note info %}
**提示**：这是一个蓝色信息通知框。
{% endnote %}

{% note success %}
**成功**：部署工作流已变绿！
{% endnote %}

---

希望这篇指南能帮助你快速上手博客写作！如果有任何格式显示不正常，请检查 `_config.yml` 中的渲染器配置。
