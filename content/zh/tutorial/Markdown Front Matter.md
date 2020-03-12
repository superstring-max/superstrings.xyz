+++
title="Markdown Front Matters"
subtitle="Markdown头数据"
date = "2019-10-24T18:23:12+08:00"
tags=["markdown","front matter"]
slug="markdown-front-matters"
+++

| 名字                                     | 描述                                                         | 说明                                                         |
| ---------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| title                                    | 标题                                                         | string                                                       |
| linkTitle                                |                                                              | string                                                       |
| subtitle                                 | 副标题                                                       | string, Markdown supported, theme only                       |
| date                                     | 时间                                                         | string                                                       |
| lastmod                                  | 上次修改的时间                                               | string                                                       |
| publishDate                              | 发表时间                                                     | string                                                       |
| expiryDate                               | 到期时间                                                     | string                                                       |
| <taxonomies>eg: categories, tags, series | 分类                                                         | array                                                        |
| description                              | 描述                                                         | string, Markdown supported                                   |
| summary                                  | 摘要                                                         | string, Markdown supported                                   |
| keywords                                 | 关键词                                                       | array                                                        |
| images                                   | 图片                                                         | array                                                        |
| slug                                     | 强制指定文章路径                                                             | string                                                       |
| url                                      |  强制指定文章路径                                                            | string                                                       |
| draft                                    | 草案                                                         | boolean                                                      |
| isCJKLanguage                            |                                                              | boolean                                                      |
| weight                                   | 排序序号                                                     | integer                                                      |
| type                                     | 类型                                                         | string, if equal to "poetry", will use a special layout for it |
| layout                                   | 模板                                                         | string                                                       |
| outputs                                  | *                                                            | array                                                        |
| aliases                                  | *                                                            | array                                                        |
| markup                                   | *                                                            | string                                                       |
| meta                                     | set `false` to disable post-meta                             | boolean, theme only                                          |
| toc                                      | 是否目录显示                                                 | boolean, override `enableTOC` in `config.toml`, theme only   |
| displayCopyright                         | 是否显示版权                                                 | boolean, override `displayPostCopyright` in `config.toml`, theme only |
| badge                                    | 是否显示更新徽章                                             | boolean, override `displayUpdatedBadge` in `config.toml`, theme only |
| gitinfo                                  | 是否显示gitinfo                                              | boolean, override `displayPostGitInfo` in `config.toml`, theme only |
| related                                  | 是否显示相关帖子                                             | boolean, override `displayRelatedPosts` in `config.toml`, theme only |
| katex                                    | 是否添加KaTeX支持                                            | boolean, override `enableKaTeX` in `config.toml`, theme only |
| mathjax                                  | 是否添加MathJax支持                                          | boolean, override `enableMathJax` in `config.toml`, theme only |
| comments                                 | 设置`false`为禁用mainSections中的注释或设置`true`为启用非mainSections中的注释 | boolean, theme only                                          |
| smallCaps                                | small caps?                                                  | boolean, override `enableSmallCaps` in `config.toml`, theme only |
| dropCap                                  | drop cap?                                                    | boolean, override `enableDropCap` in `config.toml`, theme only |
| dropCapAfterHr                           | 在每个水平线标记之后放下大写字母？                           | boolean, override `enableDropCapAfterHr` in `config.toml`, theme only |
| deleteHrBeforeDropCap                    | 在删除上限之前删除水平规则标签？                             | boolean, override `deleteHrBeforeDropCap` in `config.toml`, theme only |
| indent                                   | indent instead of margin?                                    | boolean, override `paragraphStyle` in `config.toml`, theme only |
| align                                    | 对齐方式 normal, justify, center                             | srting, if euqal to "normal", will override `enableJustify` in `config.toml`, theme only |
| original                                 | 原版的？如果设置，则可以添加以下8个术语`false`。将`author`是必需的，其他可选 | boolean, override `original` in `config.toml`, theme only    |
| author                                   | 原始帖子的作者                                               | string, theme only                                           |
| link                                     | 原始帖子的链接                                               | string, URL, theme only                                      |
| copyright                                | 职位执照                                                     | string, Markdown supported, theme only                       |
| website                                  | 作者的网站                                                   | string, theme only                                           |
| email                                    | 作者的电子邮件                                               | string, theme only                                           |
| motto                                    | 作者的描述                                                   | string, theme only                                           |
| avatar                                   | 作者的头像                                                   | string, URL, theme only                                      |
| twitter                                  | 作者的推特ID                                                 | string, theme only                                           |
| disqus_url                               | *                                                            | string, if not set, will use `Permalink` as default          |
| disqus_identifier                        | *                                                            | string, if not set, will use `RelPermalink` as default       |
| disqus_title                             | *                                                            | string, if not set, will use `Title` as default              |