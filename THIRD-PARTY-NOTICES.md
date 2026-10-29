# 来源、许可与贡献说明

本候选针对Watchmen: The End Is Nigh第一部，游戏内容权利属于原权利人。需要玩家已有正版游戏；不含游戏可执行文件、Steam客户端、存档或完整原始资源。

项目文本由gpt-6-luna/max初译、gpt-6.1-sol/high校对，主代理执行格式、来源及抽样整合；原有312条初稿保留既有来源后进入指定模型校对。原文、任务及完整校对记录保留在开发项目。未补写未经确认的人工作者署名。

资源结构研究参考thurask/watchmen-toolkit（MIT）：https://github.com/thurask/watchmen-toolkit 。本项目使用自行实现的有限解析与构建脚本，包内不含其程序或NumPy。

xdelta3 3.2.2用于开发生成VCDIFF差分，Copyright Joshua MacDonald，Apache-2.0：https://github.com/jmacd/xdelta/releases/tag/v3.2.2 。官方Windows x86_64归档SHA-256 d48f7651d86b78fdca397057b46601f89131f37219675df736db70af44ec3379。其许可证和上游BLAKE3/XZ说明保留用于溯源，玩家包不携带或执行xdelta3原生程序及其VC++依赖。

玩家使用本项目自行实现的WatchmenDelta默认表解码器（源码app/VcdiffDecoder.cs），依据RFC3284 https://www.rfc-editor.org/rfc/rfc3284.html ，支持本包无二次压缩的固定格式和Adler32窗口校验，另由安装入口校验完整SHA-256。不作为通用格式工具。运行时为Windows自带.NET Framework4.x，无第三方DLL。

字体来自Adobe Source Han Sans SC 2.005 Regular，OFL-1.1：https://github.com/adobe-fonts/source-han-sans/releases/tag/2.005R 。派生位图字形称为Watchmen SC Bitmap，生成参数和原字体指纹在font-info/；原始保留字体名Source不用于派生物命名。字形嵌入资源差分中，许可完整保留。

开发阶段使用CPython、Pillow与FontTools；玩家入口不调用它们，因此不携带这些运行时。界面使用Windows自带PowerShell5.1、.NET Framework和原生目录选择器；游戏内使用思源黑体，管理窗口使用系统界面字体。没有从本补丁安装或修改系统组件。

## 中文译文许可与声明

中文译文采用 CC BY-NC-SA4.0；游戏原始内容、思源黑体及第三方组件分别遵循原权利与随附许可。使用前请阅读同目录《版权与免责声明.md》。
