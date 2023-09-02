---
title: Step.4 主题特殊功能
date: 2020/08/13 21:45:48
categories:
- [计算机科学, 二进制杂谈, Theme Shoka Documentation]
tags:
- Hexo
- 教程
math: true
mermaid: true
quiz: true
valine:
  placeholder: "1. 提问前请先仔细阅读本文档⚡\n2. 页面显示问题💥，请提供控制台截图📸或者您的测试网址\n3. 其他任何报错💣，请提供详细描述和截图📸，祝食用愉快💪"
---

:::primary
[:rocket:快速开始](/computer-science/note/theme-shoka-doc/) - [:love_letter:依赖插件](/computer-science/note/theme-shoka-doc/dependents/) - [:pushpin:基本配置](/computer-science/note/theme-shoka-doc/config/) - [:rainbow:界面显示](/computer-science/note/theme-shoka-doc/display/) - [**:unicorn:特殊功能**](/computer-science/note/theme-shoka-doc/special/)
:::

:::info
以下介绍可以使用的markdown或者标签代码。
功能大部分基于`hexo-renderer-multi-markdown-it`渲染器，尤其是代码块的显示，与默认渲染器不兼容。
:::

# `links` 链接块
本功能参考NexT，基于Hexo Tag功能，用来建立友链或其他网址链接功能。

文章中的使用格式：

1. 使用`links`标签块，包围`yml`语法书写的内容，字段包括

--|--|--
`site`|站点名称|必填
`owner`|管理员名字|可选，默认为`site`的值
`url`|站点链接|必填
`desc`|站点描述|可选，默认为`url`的值
`image`|站点图片|可选，默认为`images/404.png`
`color`|方块颜色|可选，默认为`#666`

```raw 
&#123;% links %&#125;
- site: #站点名称
  owner: #管理员名字
  url: #站点网址
  desc: #简短描述
  image: #一张图片
  color: #颜色代码
&#123;% endlinks %&#125;
```
