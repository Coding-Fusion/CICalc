# CICalc
Build a web app with Blazor WebAssembly and Visual Studio Code

What is Blazor?
Blazor is a web technology that lets you build client web applications using C#. Blazor is a feature of the ASP.NET Core framework that allows developers to use .NET tools and libraries to build web apps.
Blazor apps are composed of reusable web UI components built using C#, HTML, and CSS. It enables developers to build both client and server code with C#, allowing you to share code and libraries with both the front-end client code and back-end logic. Using C# for both can simplify sharing data between the front-end and backend, enable code reuse to accelerate development and simplify maintenance.
Blazor can be used to generate server-side code that handles UI interactions over a WebSocket connection, or a client-side web app that runs directly in the browser via WebAssembly.

What is WebAssembly?
WebAssembly (WASM) is an open binary standard that defines a portable code format for executable programs designed to run in web browsers. It is a textual assembly language with a compact binary format built for fast downloads and near-native performance.
WebAssembly provides a compilation target for languages such as C/C++ and Rust. It is designed to run alongside JavaScript, allowing both to work together. It can also be used to generate Progressive Web Applications that can be downloaded and run offline.

What is Blazor WebAssembly?
Blazor WebAssembly allows developers to run .NET code in a browser. It's a single-page app framework and uses the WebAssembly open standards without requiring plugins or code generation.
.NET code executed via WebAssembly in the browser runs in the browser's JavaScript sandbox. It includes all the security and protection that the sandbox provides to help prevent malicious actions on the client machine.
Under the hood, Blazor uses a .NET runtime compiled to a WebAssembly module that is downloaded with the app. The module is able execute .NET Standard code included in your Blazor application.
Blazor WebAssembly apps are restricted to the capabilities of the browser that is executing the application but can access full browser functionality via JavaScript interop.
Blazor WebAssembly supported browsers

Blazor WebAssembly requires a modern desktop or mobile browser. The following browsers are currently supported:
Microsoft Edge
Mozilla Firefox
Google Chrome
Safari
Blazor WebAssembly development requirements
Blazor WebAssembly applications can be built using the latest versions of Visual Studio 2019, Visual Studio for Mac or Visual Studio Code. In this module, we'll be focusing on Visual Studio code.
Regardless of your development environment, you'll need to install the .NET Core 3.1 SDK. With the SDK installed, you'll have everything you need to start building Blazor apps. You'll install all of the requirements to build Blazor WebAssembly app with Visual Studio Code in the next exercise.


Install tools and templates
We'll start by downloading the .NET Core 3.1 SDK, it includes the .NET Core SDK, the .NET Core Runtime, and the ASP.NET Core runtime.
Install .NET Core 3.1 by downloading the latest version from https://dotnet.microsoft.com/download/dotnet-core/3.1 for your operating system
Install Visual Studio Code extensions
We need to install two Visual Studio Code extensions to develop Blazor WebAssembly applications: the Microsoft C# extension and the JavaScript debugger extension.
Install the C# for Visual Studio Code extension

Open Visual Studio Code on your local machine
Open the Extension browser by clicking on the Extension left navigation button (or press ctrl-shift-X on Windows)
Search for C# for Visual Studio Code
Install the C# for Visual Studio Code (powered by OmniSharp) extension by pressing the install button
Install the JavaScript debugger extension

The JavaScript debugger extension is currently in preview, we'll install the latest build.
Open the Extension browser in Visual Studio Code by clicking on the Extension left navigation button (or press ctrl-shift-X on Windows)
Search for JavaScript debugger
Install the JavaScript Debugger (Nightly) extension by pressing the install button


Configure the JavaScript debugger extension

Open the Extension browser in Visual Studio Code by clicking on the Extension left navigation button (or press ctrl-shift-X on Windows)
Find the JavaScript Debugger (Nightly) in the list of Enabled extensions

Open the extensions settings by right-clicking on JavaScript Debugger (Nightly) and select Extension Settings
Scroll and find the Debug > JavaScript Use Preview setting
Check Use the new in-preview JavaScript debugger for Node.js and Chrome.

Create a new Blazor WebAssembly app
To validate our setup, we'll make a new Blazor WebAssembly client web app using the installed template.
Open a terminal or command prompt on your local development machine
In the command prompt or terminal dotnet new blazorwasm -o CICalc
Navigate to the CICalc sub folder


Run the app
From the command prompt or terminal dotnet run to launch the app
Open a web browser to https://localhost:5001





