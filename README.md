# Obsidian Weread Plugin

[![](https://github.com/zhaohongxuan/obsidian-weread-plugin/actions/workflows/CI.yml/badge.svg)](https://github.com/zhaohongxuan/obsidian-weread-plugin/actions/workflows/CI.yml)
[![Release Obsidian plugin](https://github.com/zhaohongxuan/obsidian-weread-plugin/actions/workflows/release.yml/badge.svg)](https://github.com/zhaohongxuan/obsidian-weread-plugin/actions/workflows/release.yml)
[![GitHub license](https://badgen.net/github/license/Naereen/Strapdown.js)](https://github.com/zhaohongxuan/obsidian-weread-plugin/blob/main/LICENSE)
[![Github all releases](https://img.shields.io/github/downloads/zhaohongxuan/obsidian-weread-plugin/total.svg)](https://GitHub.com/zhaohongxuan/obsidian-weread-plugin/releases/)
[![GitLab latest release](https://badgen.net/github/release/zhaohongxuan/obsidian-weread-plugin/)](https://github.com/zhaohongxuan/obsidian-weread-plugin/releases)

> 从 [obsidian-weread-plugin](https://github.com/zhaohongxuan/obsidian-weread-plugin) Fork而来



Obsidian微信读书插件是一个社区插件，用来同步微信读书中书籍`元信息`、`高亮标注`，`划线感想`、`书评`等，并将这些信息转换为markdown格式保存到Obsidian的文件夹中，初次使用，如果笔记数量较多，更新会比较慢，后面再去更新的时候只会更新`划线数量`或者`笔记数量`有变化的书籍，一般速度很快。

## 更新功能
- 主要修改了将读书笔记同步至日历的部分，自定义推送格式，用于适配[Thino](https://pkmer.cn/products/thino/)的Memos；
- 如果你是Thino的Pro会员，可以参考[这个例子](https://github.com/Quorafind/Obsidian-Thino/discussions/532)直接进行修改，不用单独使用此插件。

## 新增功能：自定义标签支持

插件现已支持为所有导出的笔记和日历推送内容添加"自定义标签"。

- 你可以在插件设置页中填写自定义标签内容（如 `#微信读书`）。
- 支持动态模板变量（如 `#{{metaData.title}}`），可自动渲染为书名、作者等信息。
- 标签会自动添加到每条日历推送（Thino/Memos格式）引用行的前面，便于分类、自动化处理。

**示例：**

- 设置自定义标签为 `#微信读书`，则每条推送内容会自动带上 `#微信读书`。
- 设置为 `#{{metaData.title}}`，则每条推送内容会自动带上当前书名作为标签。

你可以根据自己的需求自由组合标签和模板变量，实现更灵活的内容管理。

**实际效果：**
- 日记显示
![日记显示](https://pics.shineee.site/2025/06/a2b5a2e0e7186a883ff87a08df913e6e.png)

- Thino显示
![Thino显示](https://pics.shineee.site/2025/06/4a5cc6b8e50f8584bb85503eb23baf71.png)