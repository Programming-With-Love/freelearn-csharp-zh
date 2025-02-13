# 前言

开发和维护游戏的过程在过去几年中发生了非常快速的变化。越来越普遍的是游戏开发者许可第三方游戏引擎，如 CryENGINE，以便完全专注于游戏本身。

作为第一个以纯**所见即所得**（**WYSIWYP**）理念出货的游戏引擎，CryENGINE 专注于通过允许开发人员直接进入他们的游戏，预览变化并且不等待级别和资产构建来提高生产力和迭代。

对于程序员来说，CryENGINE 是理想的工具集。可以使用慷慨的 API 在 C++中进行开发，使开发人员可以直接进入代码并编写性能优越的代码，而不受限于晦涩的脚本语言。有了想法？启动 Visual Studio，立即开始工作。

# 本书涵盖的内容

第一章，“介绍和设置”，涵盖了通过简要概述引擎，详细介绍其优势，提供的可能性，并逐步指南设置您的环境来加快速度的过程。

第二章，“使用 Flowgraph 进行可视化脚本编程”，向您介绍了可视化脚本工具，以便以一种易于访问的视觉方式创建游戏逻辑。

第三章，“创建和利用自定义实体”，涵盖了实体系统以及如何利用它来为您带来好处。用从简单的物理化对象到复杂的天气模拟管理器的实体填充您的游戏世界。

第四章，“游戏规则”，为您提供了对游戏规则系统的深入了解，为您提供了一个统一的模板，用于全面的游戏和会话逻辑。它还教授如何在各种语言中实现自定义游戏模式。

第五章，“创建自定义角色”，详细介绍了为玩家控制的实体和人工智能的基础创建自定义角色类的过程。

第六章，“人工智能”，涵盖了使用内置人工智能解决方案创建一个生动而有活力的世界的过程。

第七章，“用户界面”，详细介绍了使用 Flash 和 Autodesk Scaleform 来为您的界面增添色彩，从简单的屏幕位图到在游戏世界中呈现交互式 Flash 元素。

第八章，“多人游戏和网络”，涵盖了将引擎在线化的工作，并学习如何在网络上同步游戏世界的背后工作。

第九章，“物理编程”，涵盖了物理系统的内部工作原理，以及为从最大的车辆到最小的粒子效果的一切物理相互作用的创建过程。

第十章，“渲染编程”，帮助您了解渲染系统的工作原理，以及如何使用它来创建和扩展从渲染节点到多个视口的一切。

第十一章，“效果和声音”，详细介绍了 CryENGINE 使用的 FMod 声音引擎的工作原理，使您能够为您的项目实现令人信服的声音。

第十二章，“调试和性能分析”，涵盖了调试游戏的常见方法，以及使用控制台的基础知识。

# 您需要为本书做好的准备

+   CryENGINE 3 免费 SDK v3.5.4

+   CryMono v0.7 for CryENGINE 3.5.4

+   Visual Studio Express 2012

+   Notepad++

+   FMod

# 本书的受众

这本书是为具有基本 CryENGINE 和其编辑器使用知识的开发人员编写的，在某些情况下，会假设读者了解非常基本的功能，比如在编辑器中加载关卡和放置实体。如果您以前从未使用过 CryENGINE，我们建议您自己玩一下 CryENGINE Free SDK，或者购买 Sean Tracy 和 Paul Reindell 的《CryENGINE 3 游戏开发：初学者指南》。

# 约定

在这本书中，您将找到许多不同类型信息的文本样式。以下是这些样式的一些示例，以及它们的含义解释。

文本中的代码单词显示如下："`GFx`元素确定应加载哪个 Flash 文件用于该元素。"

代码块设置如下：

```cs
<events>
  <event name="OnBigButton" fscommand="onBigButton" desc="Triggered when a big button is pressed">    
    <param name="id" desc="Id of the button" type="string" />
  </event>
</events>
}
```

**新术语**和**重要单词**以粗体显示。您在屏幕上看到的单词，比如菜单或对话框中的单词，会以这种形式出现在文本中："一旦启动，UI 图将被激活，假设它包含一个**UI:Action:Start**节点，如下所示："

### 注意

警告或重要提示会以这样的方式出现在一个框中。

### 提示

提示和技巧会以这种形式出现。
