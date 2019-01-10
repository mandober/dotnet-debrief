# Comparison with .NET Framework

https://docs.microsoft.com/en-us/dotnet/core/about

.NET was first announced by Microsoft in 2000 and then evolved from there. The .NET Framework has been the primary .NET implementation produced by Microsoft during that nearly two decade period.

The major differences between .NET Core and the .NET Framework:

- App-models: 
.NET Core does not support all the .NET Framework app-models. In particular, it doesn't support ASP.NET Web Forms and MVC. It was announced that .NET Core 3 will support WPF and Windows Forms.

- APIs: 
.NET Core contains a large subset of .NET Framework Base Class Library, with a different factoring (assembly names are different; members exposed on types differ in key cases). These differences require changes to port source to .NET Core in some cases (see microsoft/dotnet-apiport). .NET Core implements the .NET Standard API specification.

- Subsystems: 
.NET Core implements a subset of the subsystems in the .NET Framework, with the goal of a simpler implementation and programming model. For example, Code Access Security (CAS) is not supported, while reflection is supported.

- Platforms: 
The .NET Framework supports Windows and Windows Server while .NET Core also supports macOS and Linux.

- Open Source: 
.NET Core is open source, while a read-only subset of the .NET Framework is open source.
While .NET Core is unique and has significant differences to the .NET Framework and other .NET implementations, it is straightforward to share code between these implementations, using either source or binary sharing techniques.