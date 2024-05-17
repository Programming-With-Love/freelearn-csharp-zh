# 前言

我们中的一些人可能习惯于使用面向对象编程技术开发应用程序，不关心函数式编程技术。然而，使用函数式编程是有好处的。其中一个好处是，我们将从新的角度看待我们的编程代码，因为函数式编程中的函数与数学函数相同。因为它与数学函数相同，函数式编程中的函数不包含副作用，这意味着函数调用不会对类中的其他函数产生影响。我们将在本书中讨论有关函数式编程的好处和其他相关事项的更多细节。

# 本书涵盖的内容

第一章 ，*品味 C#中的函数式风格*，通过讨论其概念和函数式与命令式编程的比较，介绍了函数式编程方法。我们还尝试将简单的命令式代码重构为函数式方法。

第二章 ，*委托演练*，涵盖了委托的定义、语法和用法。我们还讨论了委托的变化和内置委托。

第三章 ，*用 Lambda 表达式表达匿名方法*，引导我们了解委托的概念，并使用它来创建和使用匿名方法。在深入研究匿名方法之后，我们可以将其转换为 Lambda 表达式，然后应用于函数式编程。

第四章 ，*使用扩展方法扩展对象功能*，详细说明了在函数式编程中使用扩展方法的好处。在此之前，我们讨论了扩展方法的用法，还讨论了如何在 IntelliSense 中获取这个新方法。此外，我们尝试从其他程序集调用扩展方法。

第五章 ，*使用 LINQ 轻松查询任何集合*，列举了 C#提供的 LINQ 运算符，并比较了两种 LINQ 语法：流畅语法和查询表达式语法。我们还讨论了 LINQ 过程中的延迟执行。

第六章 ，*使用异步编程增强函数式程序的响应性*，涵盖了函数式方法的异步编程。它将解释异步编程模型和基于任务的异步模式。

第七章 ，*学习递归*，解释了递归在循环序列上的优势。我们还在本章讨论了直接递归和间接递归。

第八章 ，*使用惰性和缓存技术优化代码*，涵盖了函数式方法中用于优化代码的技术。我们讨论了惰性思维和缓存技术，以优化我们的代码。

第九章 ，*使用模式*，涵盖了使用模式与传统的 switch-case 操作相比的优势。我们在本章讨论了模式匹配和单子。我们使用模式匹配功能，这是 C# 7 提供的新功能。

第十章 ，*在 C#函数式编程中采取行动*，引导我们通过基于给定命令式代码开发函数式代码。我们利用上一章的学习成果，使用函数式方法创建一个应用程序。

第十一章 ，*编码最佳实践和测试功能代码*，解释了功能方法的最佳实践，包括创建诚实的签名和处理副作用。我们还将代码分为领域逻辑和可变外壳，然后使用单元测试进行测试。

# 您需要为本书做好准备

要阅读本书并成功编译所有源代码，我们需要一台运行 Microsoft Windows 10（或更高版本）的个人电脑，并安装 Visual Studio Community 2015 Update 3 以运行第 1-8 章、10、11 章的代码，以及安装 Visual Studio Community 2017 RC（Release Candidate）以运行第九章的代码。我们还需要.NET Framework 4.6.2，除非您需要重新编写所有源代码以在当前版本的.NET Framework 中运行。如果您想在其他平台上编译所有代码，则还需要.NET Core 1.0，因为所有代码都与.NET Core 1.0 兼容。

# 本书适合对象

本书适合具有 C#基础知识但没有功能性编程经验的 C#开发人员。

# 惯例

在本书中，您将找到许多文本样式，用于区分不同类型的信息。以下是这些样式的一些示例及其含义的解释。

文本中的代码词、数据库表名、文件夹名、文件名、文件扩展名、路径名、虚拟 URL、用户输入和 Twitter 句柄显示如下：“我们可以通过使用`include`指令包含其他上下文。”

代码块设置如下：

```cs
namespace ActionFuncDelegates
{
  public partial class Program
  {
    static void Main(string[] args)
    {
      //ActionDelegateInvoke();
      FuncDelegateInvoke();
    }
  } 

```

当我们希望引起您对代码块的特定部分的注意时，相关行或项目将以粗体显示：

```cs
Console.WriteLine("Prime Number from 0 - 49 are:"); 

foreach (int i in extractedData)

Console.Write("{0} \t", i)

; 
Console.WriteLine();
```

任何命令行输入或输出都以以下方式编写：

```cs

C:\>dir | more

```

**新术语**和**重要单词**以粗体显示。例如，屏幕上看到的单词，例如菜单或对话框中的单词，会以这种方式出现在文本中：“我们有一个包含**{(a * b)}**的**Body**属性，包含**Lambda**的**NodeType**，包含具有三个模板的**Func**委托的**Type**。”

### 注意

警告或重要提示会以以下方式显示。

### 提示

提示和技巧看起来像这样。