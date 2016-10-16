---
title: "Building on the Command Line"
ms.custom: na
ms.date: "10/14/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-cpp"
ms.tgt_pltfrm: na
ms.topic: "get-started-article"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "command-line builds [C++]"
  - "compiling source code [C++], command line"
  - "builds [C++], command-line"
  - "command line [C++], building from"
  - "command line [C++], compilers"
ms.assetid: 7ca9daed-a003-4162-842d-908f79058365
caps.latest.revision: 22
ms.author: "corob"
manager: "ghogen"
translation.priority.ht: 
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "ru-ru"
  - "zh-cn"
  - "zh-tw"
translation.priority.mt: 
  - "cs-cz"
  - "pl-pl"
  - "pt-br"
  - "tr-tr"
---
# Building on the Command Line
You can build C and C++ applications on the command line by using tools that are included in [!INCLUDE[vsprvs](../build/includes/vsprvs_md.md)]. Every edition of [!INCLUDE[vsprvs](../build/includes/vsprvs_md.md)] installs a command-line toolset that includes a compiler, linker, and other build tools, and a command file that sets the required build environment. By default, these tools are installed in *drive*:\Program Files (x86)\Microsoft Visual Studio *version*\VC\bin\\. (The actual directory on your computer depends on the system, the [!INCLUDE[vsprvs](../build/includes/vsprvs_md.md)] version, and your installation choices.)  
  
 To work correctly, the [!INCLUDE[vcprvc](../build/includes/vcprvc_md.md)] command-line tools require several environment variables that are customized for your installation. When [!INCLUDE[vsprvs](../build/includes/vsprvs_md.md)] is installed, it creates a vcvarsall.bat command file that you can run to set the required environment variables. It also creates a shortcut that starts a Developer Command Prompt window in which these variables are already set. These environment variables are specific to your installation, and might be changed by product updates or upgrades. Therefore, we recommend that you use vcvarsall.bat or a Developer Command Prompt shortcut instead of setting them yourself. For more information, see [Setting the Path and Environment Variables for Command-Line Builds](../build/setting-the-path-and-environment-variables-for-command-line-builds.md).  
  
### To open a Developer Command Prompt window  
  
1.  On the Windows **Start** menu, open **All apps** and then open the **Visual Studio** folder for your version of Visual Studio. In some versions of Visual Studio, the folder is called  **Visual Studio Tools**.  
  
2.  In the **Visual Studio** folder, choose the **Developer Command Prompt** for your version of [!INCLUDE[vsprvs](../build/includes/vsprvs_md.md)]. If you've installed the Visual C++ Build Tools edition, choose the **x86 Native Tools Command Prompt**.  
  
 To build a C/C++ project on the command line, you can use these [!INCLUDE[vcprvc](../build/includes/vcprvc_md.md)] command-line tools:  
  
 [CL](../buildref/compiling-a-c-c---program.md)  
 Use the compiler (cl.exe) to compile and link source code files into apps, libraries, and DLLs.  
  
 [Link](../buildref/linking.md)  
 Use the linker (link.exe) to link compiled object files and libraries into apps and DLLs.  
  
 [MSBuild (Visual C++)](../build/msbuild--visual-c---.md)  
 Use MSBuild (msbuild.exe) to build [!INCLUDE[vcprvc](../build/includes/vcprvc_md.md)] projects and [!INCLUDE[vsprvs](../build/includes/vsprvs_md.md)] solutions. This is equivalent to running the **Build** project or **Build Solution** command in the [!INCLUDE[vsprvs](../build/includes/vsprvs_md.md)] IDE.  
  
 [DEVENV](../Topic/Devenv%20Command%20Line%20Switches.md)  
 Use DEVENV (devenv.exe) combined with a command-line switch—for example, **/Build** or **/Clean**—to perform certain build commands without displaying the [!INCLUDE[vsprvs](../build/includes/vsprvs_md.md)] IDE.  
  
 [NMAKE](../build/nmake-reference.md)  
 Use NMAKE (nmake.exe) to automate tasks that build [!INCLUDE[vcprvc](../build/includes/vcprvc_md.md)] projects by using a traditional makefile.  
  
 When you build on the command line, you can get information about warnings, errors, and messages by starting [!INCLUDE[vsprvs](../build/includes/vsprvs_md.md)] and then on the menu bar, choosing **Help**, **Search**.  
  
## In This Section  
 The articles in this section of the documentation show how to build apps on the command line, describe how to customize the command-line build environment to use 64-bit toolsets and target x86, x64, and ARM platforms, and demonstrate how to use the command-line build tools MSBuild and NMAKE.  
  
 [Walkthrough: Compiling a Native C++ Program on the Command Line](../build/walkthrough--compiling-a-native-c---program-on-the-command-line.md)  
 Gives an example that shows how to create and compile a simple C++ program on the command line.  
  
 [Walkthrough: Compiling a C Program on the Command Line](../build/walkthrough--compiling-a-c-program-on-the-command-line.md)  
 Describes how to compile a program written in the C programming language.  
  
 [Walkthrough: Compiling a C++/CLI Program on the Command Line](../build/walkthrough--compiling-a-c---cli-program-on-the-command-line.md)  
 Describes how to create and compile a C++/CLI program that uses the .NET Framework.  
  
 [Walkthrough: Compiling a C++/CX Program on the Command Line](../build/walkthrough--compiling-a-c---cx-program-on-the-command-line.md)  
 Describes how to create and compile a C++/CX program that uses the Windows Runtime.  
  
 [Setting the Path and Environment Variables for Command-Line Builds](../build/setting-the-path-and-environment-variables-for-command-line-builds.md)  
 Describes how to start a Command Prompt window that has the required environment variables set for command-line builds that target x86, x64, and ARM platforms by using a 32-bit or 64-bit toolset.  
  
 [NMAKE Reference](../build/nmake-reference.md)  
 Provides links to articles that describe the Microsoft Program Maintenance Utility (NMAKE.EXE).  
  
 [MSBuild (Visual C++)](../build/msbuild--visual-c---.md)  
 Provides links to articles that discuss how to use MSBuild.EXE.  
  
## Related Sections  
 [/MD, /MT, /LD (Use Run-Time Library)](../buildref/-md---mt---ld--use-run-time-library-.md)  
 Describes how to use these compiler options to use a Debug or Release run-time library.  
  
 [C/C++ Compiler Options](../buildref/compiler-options.md)  
 Provides links to articles that discuss the C and C++ compiler options and CL.exe.  
  
 [Linker Options](../buildref/linker-options.md)  
 Provides links to articles that discuss the linker options and LINK.exe.  
  
 [C/C++ Build Tools](../buildref/c-c---build-tools.md)  
 Provides links to the C/C++ build tools that are included in [!INCLUDE[vsprvs](../build/includes/vsprvs_md.md)].  
  
## See Also  
 [Building C/C++ Programs](../Topic/Building%20C-C++%20Programs.md)