# .NET Terms


## .NET Core
.NET Core is open-sourced, cross-platform version of .NET Framework, free of Windows-related components.

## CoreCLR
CoreCLR is .NET Core's complete runtime implementation of CLR - the virtual machine that manages the execution of programs. CoreCLR comes with RyuJIT and CoreFX.

## RyuJIT
RyuJIT is the just-in-time compiler included in CoreCLR.

## CoreFX
CoreFX is a partial fork of FCL.

## .NET Framework
.NET Framework is Microsoft's original Windows-only framework, a superset of the slimmed-down .NET Core. It includes a large class library, FCL, and provides interoperability across supported programming languages.

## Framework Class Library - FCL
FCL is the class library included in .NET Framework and .NET Core.

## .NET Micro Framework - NETMF
.NET Micro Framework (NETMF) is a .NET Framework platform for resource-constrained devices with at least 256 KB of flash and 64 KB of random-access memory (RAM). It includes a small version of the .NET Common Language Runtime (CLR) and supports development in C#, Visual Basic .NET, and debugging using Visual Studio.

## .NET Compiler Platform - Roslyn
.NET Compiler Platform, better known as *Roslyn*, is a set of open-source compilers and code analysis APIs for C# and VB .NET languages.

## Common Language Runtime - CLR
CLR is the VM that manages the execution of .NET programs. A process known as JIT compilation converts compiled code into machine instructions which the computer's CPU then executes. The CLR provides language services: memory management, type safety, exception handling, garbage collection, security, thread management. All programs written for the .NET framework, regardless of programming language, are executed by the CLR. CLR implements VES as defined by the CLI public standard.

## Virtual Execution System - VES
The Virtual Execution System (VES) is a run-time system of the CLI which provides an environment for executing managed code. It provides direct support for a set of built-in data types, defines a hypothetical machine with an associated machine model and state, a set of control flow constructs and an exception handling model. To a large extent, the purpose of the VES is to provide the support required to execute CIL instruction set.

## Common Intermediate Language - CIL
Common Intermediate Language (CIL), formerly Microsoft Intermediate Language (MSIL), is the lowest-level human-readable language defined by the CLI specification, used by the .NET Framework, .NET Core, and Mono. Languages which target a CLI-compatible runtime environment compile to CIL, which is assembled into an object code that has a bytecode-style format. CIL is an object-oriented assembly language, and is entirely stack-based. Its bytecode is translated into native code or executed by VM.

## Entity Framework - EF
EF is an open source object-relational mapping (ORM) framework for ADO.NET. It was a part of .NET Framework, but since Entity framework version 6 it is separated from .NET framework.

## ASP.NET
is an open-source server-side web application framework designed for web development to produce dynamic web pages. It was developed by Microsoft to allow programmers to build dynamic web sites, web applications and web services.

## ASP.NET Core
is a free and open-source web framework, and higher performance than ASP.NET, developed by Microsoft and the community. It is a modular framework that runs on both the full .NET Framework, on Windows, and the cross-platform .NET Core.

## ASP.NET MVC
is a web application framework developed by Microsoft, which implements the Model–View–Controller pattern. It is open-source software, apart from the ASP.NET Web Forms component which is proprietary.

## ASP.NET Web Forms
is a web application framework and one of several programming models supported by the Microsoft ASP.NET technology. Web Forms applications can be written in any programming language which supports the Common Language Runtime, such as C# or Visual Basic. Main building blocks of Web Forms pages are server controls, which are reusable components responsible for rendering HTML markup and responding to events.

## F#
is a strongly typed, multi-paradigm programming language that encompasses functional, imperative, and object-oriented programming methods. F# is most often used as a cross-platform Common Language Infrastructure (CLI) language, but it can also generate JavaScript and graphics processing unit (GPU) code.

## ML.NET
is a free software machine learning library for the C#, F# and VB.NET programming languages. It also supports Python models when used together with NimbusML. The preview release of ML.NET included transforms for feature engineering like n-gram creation, and learners to handle binary classification, multi-class classification, and regression tasks.

## MSBuild
Microsoft Build Engine is a free and open-source build tool set for managed code as well as native C++ code and was part of .NET Framework. Visual Studio depends on MSBuild, but not the vice versa. Visual Studio Application Lifecycle Management depends on MSBuild to perform team builds via the Team Foundation Server.

## NuGet
is a free and open-source package manager designed for the Microsoft development platform (formerly known as NuPack). Since its introduction in 2010, NuGet has evolved into a larger ecosystem of tools and services.

## PowerShell
is a task automation and configuration management framework from Microsoft, consisting of a command-line shell and associated scripting language. Initially a Windows component only, known as Windows PowerShell, it was made open-source and cross-platform on 18 August 2016 with the introduction of PowerShell Core. The former is built on .NET Framework while the latter on .NET Core.

## Windows Communication Foundation
WCF, previously known as *Indigo*, is a runtime and a set of APIs in the .NET Framework for building connected, service-oriented applications.

## ADO.NET
ADO.NET is Microsoft's data access technology, a part of framework's BCL, that enables communication between relational databases through a common set of components. It provides access to the data and services to programmers, allowing them to modify data stored in relational, but also non-relational, database systems.

## Microsoft Sync Framework
Microsoft Sync Framework is a data synchronization platform used to synchronize data across multiple data stores.
Sync Framework includes a transport-agnostic architecture, into which data store-specific synchronization providers, modelled on the ADO.NET data provider API, can be plugged in.
Sync Framework can be used for offline access to data, by working against a cached set of data and submitting the changes to a master database in a batch, as well as to synchronize changes to a data source across all consumers (publish/subscribe sync) and peer-to-peer synchronization of multiple data sources.
Sync Framework features built-in capabilities for conflict detection – whether data to be changed has already been updated – and can flag them for manual inspection or use defined policies to try to resolve the conflict.
Sync Services includes an embedded SQL Server Compact database to store metadata about the synchronization relationships as well as about each sync attempt.
Sync Framework API is surfaced both in managed code, for use with .NET Framework applications, as well as unmanaged code, for use with COM applications.

## Chakra
is a JavaScript engine developed by Microsoft for its Microsoft Edge web browser. It is a fork of the JScript engine used in Internet Explorer. Like the Edge layout engine and unlike previous versions in Internet Explorer the declared intention is that it will reflect the "Living Web". On December 5, 2015, it was announced that core components of Chakra will be open-sourced as ChakraCore.

## SignalR is a software library for Microsoft ASP.NET that allows server code to send asynchronous notifications to client-side web applications. The library includes server-side and client-side JavaScript components.

## WinJS
is the Windows Library for JavaScript, an open-source JS library developed by Microsoft.


