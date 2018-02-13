##thirdparty 增加 poppler_win 用于编译工程cairo curl freetype jpeglib libopenjpeg nspr pixman poppler-qt4 zlib
  其中poppler-qt4依赖工程cairo curl freetype jpeglib libopenjpeg nspr pixman zlib
##include 增加  poppler头文件
windows 打开宏定义 USE_PDF
add library poppler-qt4.lib 


Debug版本 库是/MD 使用库的生成方式也必须是/MD
Release版本 库是/MT 使用库的生成方式也必须是/MT 我们程序用的是/MT 所以生成的库也必须是/MT的模式


增加文件freetype6.dll libz.dll QtXml4.dll QtXmld4.dll
poppler_debug poppler_release poppler poppler_win.zip



可以用dumpbin.exe 查看导出信息



错误: 无法解析参考 Microsoft.VC90.DebugCRT,processorArchitecture="x86",publicKeyToken="1fc8b3b9a1e18e3b",type="win32",version="9.0.21022.8"。 引用了VC90.DebugCRT 