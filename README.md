# Windows Application Development Relevant Articles
Windows应用开发相关

<br />

- [开发 Windows 10 应用程序](https://docs.microsoft.com/zh-cn/learn/paths/develop-windows10-apps/)
- [Windows Presentation Foundation](https://docs.microsoft.com/en-us/dotnet/framework/wpf/)
- [Windows Forms](https://docs.microsoft.com/en-us/dotnet/framework/winforms/)
- [获取WINDOWS下当前用户路径 USERPROFILE](https://blog.csdn.net/woodsp/article/details/51922920)（MS-DOS中回显变量值也是用echo）
- [Detecting architecture at compile time from MASM/MASM64](https://stackoverflow.com/questions/2595550/detecting-architecture-at-compile-time-from-masm-masm64)
- [How do I render my DirectX C++ engine to a C# Panel?](https://gamedev.stackexchange.com/questions/124249/how-do-i-render-my-directx-c-engine-to-a-c-panel)
- [Calling Native Functions from Managed Code](https://docs.microsoft.com/en-us/cpp/dotnet/calling-native-functions-from-managed-code?view=vs-2019)（**Platform Invocation Services**, commonly referred to as **P/Invoke**, is a feature of Common Language Infrastructure implementations, like Microsoft's Common Language Runtime, that enables managed code to call native code.）
- [C# – Calling Unmanaged DLL functions from Manage Code](https://codesteps.com/2018/10/13/c-sharp-calling-unmanaged-dll-functions-from-manage-code/)
- [Is it possible to call a C function from C#.Net](https://stackoverflow.com/questions/11425202/is-it-possible-to-call-a-c-function-from-c-net)
- [How to call native C# code from a C library](https://forums.xamarin.com/discussion/98337/how-to-call-native-c-code-from-a-c-library)
- [Xamarin Part 4 - Dealing with Multiple Platforms](https://docs.microsoft.com/en-us/xamarin/cross-platform/app-fundamentals/building-cross-platform-applications/platform-divergence-abstraction-divergent-implementation)
- [Func delegate with no return type](https://stackoverflow.com/questions/917551/func-delegate-with-no-return-type)
- [怎么让IntPtr指向一个字符串](http://www.myexception.cn/c-sharp/73219.html)
- [从C# String类理解Unicode（UTF8/UTF16)](https://www.cnblogs.com/zizifn/p/4734456.html)
- [C#学习笔记 IEquatable 接口 IEqualityComparer 接口](https://blog.csdn.net/july_yeye/article/details/68951425)
- [c#之lamda表达式的前世今生](https://www.toutiao.com/i6769386569053766157/)
- [通用 Windows 平台文档](https://docs.microsoft.com/zh-cn/windows/uwp/)
- [Visual Studio 2019中，用于调试的即时窗口](https://docs.microsoft.com/zh-cn/visualstudio/ide/reference/immediate-window?view=vs-2019)
- [VC编译出现ITERATOR_DEBUG_LEVEL值不匹配异常](https://blog.csdn.net/crystalshaw/article/details/79961140)
- [检测到“RuntimeLibrary”的不匹配项: 值“MT_StaticRelease”不匹配值“MD_DynamicRelease”](https://blog.csdn.net/hk121/article/details/80334481)
- [VC使用CRT调试功能检测内存泄漏](https://blog.csdn.net/lvwx369/article/details/41776965)
- MSVC中，Visual Studio 2019以前使用`__pragma`，比如：`__pragma(loop(hint_parallel(0)))`。Visual Studio 2019起可以使用`_Pragma`，比如：`_Pragma("loop( hint_parallel(0))")`。
- [MSVC loop pragma](https://docs.microsoft.com/en-us/cpp/preprocessor/loop?redirectedfrom=MSDN)
- [Visual Studio 2019之你还在手工清理代码吗？](https://www.toutiao.com/i6760478177031619075/)
- [visual studio如何查看全部断点](http://ask.zol.com.cn/x/9061922.html)
- [Visual Studio How to set two environment variable?](https://social.msdn.microsoft.com/Forums/vstudio/en-US/4665af21-19bf-442b-952f-7f08694b94ec/how-to-set-two-environment-variable)
- 如何利用Visual Studio通过打开指定的应用程序来调试当前的DLL项目：在当前DLL项目工程中，点击菜单栏的“项目”，选择“属性”，然后“配置属性”中的“调试”一栏中，右侧的“命令”中输入应用程序路径即可。应用程序路径最后必须是该应用文件名，当然也可以是一个批处理文件。
- [(Visual Studio) Set compiler and build properties](https://docs.microsoft.com/en-us/cpp/build/working-with-project-properties)
- MSVC忽略特定警告：使用`/wd[警告编号]`，多个警告用分号分隔。比如：`/wd4819`。
- [呕心整理Windows平台批处理脚本编程笔记之for语句](https://www.toutiao.com/a6798393017280496139)
- [C++ win32和linux获取系统剩余内存](https://blog.csdn.net/q1368232592/article/details/85157823)
- [Under windows, how to allocate a “write combining” memory block?](https://stackoverflow.com/questions/883622/under-windows-how-to-allocate-a-write-combining-memory-block)
- [Windows API笔记（五）管理虚拟内存](https://blog.csdn.net/lwwl12/article/details/89914275)
- [Window API （四）虚拟内存管理](https://blog.csdn.net/fansongy/article/details/7077605)

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

<br />

## Windows 10的日常使用

- [win10开启内置Ubuntu](https://www.jianshu.com/p/6d6e629df051)
- Windows 10 Edge浏览器中使用Ctrl+鼠标左键可直接在新标签页打开指定的链接。


