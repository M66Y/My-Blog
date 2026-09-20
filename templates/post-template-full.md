---
# ===== 必填 =====
title: 文章标题                          # 必填
published: 2026-09-12T20:30:00+08:00      # 必填。纯日期 2026-09-12 或带时区 ISO 格式；不要用空格分隔
# ===== 常用可选 =====
description: 一句话简介，显示在首页卡片和 SEO
tags: [记录, 学习]                       # 必须是非空数组，不要写字符串
category: 记录                          # 分类，单个字符串
image: /posts/covers/cover.jpg          # 封面图。本地图放 public/posts/covers/ 下，路径必须带开头 /
draft: false                            # true = 草稿，不发布
pinned: false                           # true = 首页置顶
comment: true                           # false = 关闭这篇文章的评论
# ===== 进阶可选 =====
updated: 2026-09-13                      # 更新日期
lang: zh-CN                             # 语言标记
author: 钟毓林                           # 覆盖默认作者
password: ""                            # 设置后文章加密，访问需输入密码
passwordHint: ""                        # 密码提示语
sourceLink: ""                          # 转载原文链接
licenseName: ""                         # 单独指定许可证名
licenseUrl: ""
prevTitle: ""                           # 手动指定上一篇
prevSlug: ""
nextTitle: ""                           # 手动指定下一篇
nextSlug: ""
---

正文从这里开始。


<!-- ================= 常用语法速查（发布前删掉这段） ================= -->

## 二级标题

### 三级标题

**加粗**、*斜体*、`行内代码`、[链接](https://example.com)

## 图片

本地图放 src/content/assets/ 下，用相对路径：

![图片说明](../assets/图片名.png)

## 列表

- 无序项
- 无序项

1. 有序项
2. 有序项

## 提示框

:::note
这是提示内容，支持 note / tip / important / warning / caution 五种类型。
:::

## 代码块

```python
def hello():
    print("Hello")
```

## 代码组（Tab 切换）

:::code-group

```bash [pnpm]
pnpm add astro
```

```bash [npm]
npm i astro
```

:::

## 数学公式

行内公式 $E = mc^2$，块级公式：

$$
\int_{0}^{\infty} e^{-x^2} dx = \frac{\sqrt{\pi}}{2}
$$

## 表格

| 列一 | 列二 |
| --- | --- |
| 内容 | 内容 |

## 引用

> 引用内容

## 分隔线

---
