# Blockly 源码

## Blockly 和 Scratch

Blockly 是一款运行在网页客户端的 JavaScript 程式库，目的是用来打造视觉化程式设计语言，且同时附带编辑器。它是一项由谷歌根据 Apache2.0 许可的开放源码专案。常见被应用在网页浏览器中

目前而言, Blockly 依旧是值得学习的, 尽管在视觉化程式设计中, 目前更流行的 Scratch 3.0 的解决方法, 但是我们应该注意 [scratch-blocks](https://github.com/LLK/scratch-blocks) 中所说的这段话:

> Scratch Blocks is a fork of Google's Blockly project that provides a design specification and codebase for building creative computing interfaces. Together with the Scratch Virtual Machine (VM) this codebase allows for the rapid design and development of visual programming interfaces. Unlike Blockly, Scratch Blocks does not use code generators, but rather leverages the Scratch Virtual Machine to create highly dynamic, interactive programming environments.

This project is in active development and should be considered a "developer preview" at this time.

是的, Scratch 3.0 中的主要组成为: scratch-blocks, scratch-vm, scratch-gui, 其中 scratch-blocks 是基于 blockly 重新实现的解决方案, 换一种意思, Scratch 3.0 是作为 Blockly 的框架出现的. 如果我们需要完成编程之后的动态展示, 那么 Scratch 3.0 不失为一个优秀的解决方案

## 源码文档

## Blockly 中的基础实体 (Class)

- ToolBox
  - 路径：`core/toolbox.js`
- WorkSpace
  - 路径：`core/workspace_svg.js`
- WidgetDiv
  - 路径：`core/widgetdiv.js`
- Grid
  - 路径：`core/grid.js`

## 思考

其实如果只是语言层面的话，Blockly 已经足够出色，但在用户交互层面，Blockly 有着不足，因为使用可视化编程本身的，一定不是计算机专业，或者是一名即将成为工程师的人。更多的是，对此有着兴趣的人，希望通过此来完成某些作品或者成就。因此，以 Scratch 为例，卡通角色则代表了用户方面的交互，来以此帮助有着兴趣的人来达成他们的作品或者成就。当然，可以思考的方向并不只有 Scratch 这种形式。是的，如果你有足够的创意，你可以用 Blockly 来完成任意的项目，与硬件相关，与动画相关，等。只是目前存在一个问题，Blockly 定制仍然是困难的，当然我所指不是语言或者程序的生成，而是 UI 制作，事件合成，和交互反馈 等一系列的问题。

## 参考项目 (基于 Blockly 实现)

> [pxt-blockly](https://github.com/microsoft/pxt-blockly)

This is a fork of Blockly, an open source visual programming environment. The fork is maintained by the Microsoft MakeCode team, and is used to power the blocks environment in PXT.
