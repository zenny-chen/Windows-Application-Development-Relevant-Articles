# Windows Application Development Relevant Articles
Windows应用开发相关

<br />

1. [Windows Presentation Foundation](https://docs.microsoft.com/en-us/dotnet/framework/wpf/)
1. [Windows Forms](https://docs.microsoft.com/en-us/dotnet/framework/winforms/)
1. [Detecting architecture at compile time from MASM/MASM64](https://stackoverflow.com/questions/2595550/detecting-architecture-at-compile-time-from-masm-masm64)
1. [How do I render my DirectX C++ engine to a C# Panel?](https://gamedev.stackexchange.com/questions/124249/how-do-i-render-my-directx-c-engine-to-a-c-panel)
1. [Calling Native Functions from Managed Code](https://docs.microsoft.com/en-us/cpp/dotnet/calling-native-functions-from-managed-code?view=vs-2019)（**Platform Invocation Services**, commonly referred to as **P/Invoke**, is a feature of Common Language Infrastructure implementations, like Microsoft's Common Language Runtime, that enables managed code to call native code.）
1. [C# – Calling Unmanaged DLL functions from Manage Code](https://codesteps.com/2018/10/13/c-sharp-calling-unmanaged-dll-functions-from-manage-code/)
1. [Is it possible to call a C function from C#.Net](https://stackoverflow.com/questions/11425202/is-it-possible-to-call-a-c-function-from-c-net)
1. [How to call native C# code from a C library](https://forums.xamarin.com/discussion/98337/how-to-call-native-c-code-from-a-c-library)
1. [Xamarin Part 4 - Dealing with Multiple Platforms](https://docs.microsoft.com/en-us/xamarin/cross-platform/app-fundamentals/building-cross-platform-applications/platform-divergence-abstraction-divergent-implementation)
1. [Func delegate with no return type](https://stackoverflow.com/questions/917551/func-delegate-with-no-return-type)
1. [怎么让IntPtr指向一个字符串](http://www.myexception.cn/c-sharp/73219.html)
1. [从C# String类理解Unicode（UTF8/UTF16)](https://www.cnblogs.com/zizifn/p/4734456.html)
1. [C#学习笔记 IEquatable 接口 IEqualityComparer 接口](https://blog.csdn.net/july_yeye/article/details/68951425)
1. [c#之lamda表达式的前世今生](https://www.toutiao.com/i6769386569053766157/)
1. [通用 Windows 平台文档](https://docs.microsoft.com/zh-cn/windows/uwp/)
1. [Visual Studio 2019中，用于调试的即时窗口](https://docs.microsoft.com/zh-cn/visualstudio/ide/reference/immediate-window?view=vs-2019)
1. [VC编译出现ITERATOR_DEBUG_LEVEL值不匹配异常](https://blog.csdn.net/crystalshaw/article/details/79961140)
1. [vs2012 error LNK2038 RuntimeLibrary 不匹配的解决](https://blog.csdn.net/wpc320/article/details/8496957)
1. [检测到“RuntimeLibrary”的不匹配项: 值“MT_StaticRelease”不匹配值“MD_DynamicRelease”](https://blog.csdn.net/hk121/article/details/80334481)
1. [VC使用CRT调试功能检测内存泄漏](https://blog.csdn.net/lvwx369/article/details/41776965)
1. [Visual Studio 2019之你还在手工清理代码吗？](https://www.toutiao.com/i6760478177031619075/)

<br />

#### Visual Studio 2019创建平台通用的DLL库项目

使用下图模板创建项目：

<br />

![1.jpg](https://github.com/zenny-chen/Windows-Application-Development-Relevant-Articles/blob/master/1.JPG)

<br />

请注意这个项目名与桌面DLL的区别：

<br />

![2.jpg](https://github.com/zenny-chen/Windows-Application-Development-Relevant-Articles/blob/master/2.JPG)

<br />

这样就能生成x86、x64、ARM以及ARM64这四种目标平台了。随后我们在项目属性中，将每个平台的“生成预编译头”选项设置为 **NO** 即可。


