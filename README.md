# .NET Developer Roadmap 2026.

This is a step-by-step guide to becoming a .NET Engineer, featuring over 260 distinct tools, libraries, blogs, books, videos, frameworks, and concepts. 

## [Grab my .NET Ultimate Bundle (500+ pages and a course)](https://www.patreon.com/techworld_with_milan/shop/ultimate-net-bundle-for-2025-1519389)

* A brief walk through the .NET ecosystem 
* Modern C# v6‑14 features
* 200+ interview Q\&As that hiring managers ask
* 50+ real‑world design patterns in C#
* Clean code development in C# course
* ASP.NET Core auth  & middleware best practices
* Bonus: A complete C# Cheat Sheet

[Get the .NET Ultimate Bundle 🚀](https://www.patreon.com/techworld_with_milan/shop/ultimate-net-bundle-for-2025-1519389)

[![.NET Ultimate Bundle](Bundle.png)](https://www.patreon.com/techworld_with_milan/shop/ultimate-net-bundle-for-2025-1519389)

If you want to learn more about C# and .NET technologies, be sure to subscribe to **[my newsletter](https://newsletter.techworld-with-milan.com/)**. 

## Disclaimer

> This roadmap aims to give you an idea about the landscape. The road map will guide you if you need clarification about what to learn next rather than encouraging you to pick what is hype and trendy. It would help if you grew some understanding of why one tool would be better suited for some cases than the other and remember that hype and trendy only sometimes mean best suited for the job.

## Give a Star! :star:

If you like or are using this project to learn or start your solution, please give it a star. Thanks!

## Roadmap 

![Roadmap](NET%20Roadmap.png)

Download [PDF version](NET%20Roadmap.pdf).

## Minimalistic version

Below you can find a bare minimum version every junior .NET developer needs to know, with learning materials included and clickable in the PDF version.

![Roadmap](.NET%20Developer%20Roadmap%202026.%20Minimal.png)

Download [PDF version](NET%20Developer%20Roadmap%20Minimal.pdf).


## Table of Contents

- [Understanding the .NET ecosystem](#understanding-the-net-ecosystem)
  - [.NET runtimes](#net-runtimes)
    - [.NET Framework](#net-framework)
    - [.NET Core](#net-core)
    - [The One .NET - .NET 5](#the-one-net---net-5)
    - [The current - .NET 10](#the-current---net-10)
  - [.NET Standard](#net-standard)
- [Learning resources](#learning-resources)
  - [1. C#](#1-c)
  - [2. General Development Skills](#2-general-development-skills)
  - [3. ASP.NET Core](#3-aspnet-core)
  - [4. Client-Side .NET](#4-client-side-net)
  - [5. Databases](#5-databases)
  - [6. ORM](#6-orm)
  - [7. Testing](#7-testing)
  - [8. Logging](#8-logging)
  - [9. Communication](#9-communication)
  - [10. Background tasks](#10-background-tasks)
  - [11. Caching](#11-caching)
  - [12. Observability](#12-observability)
  - [13. Containerization](#13-containerization)
  - [14. Cloud](#14-cloud)
  - [15. Continuous Integration \& Delivery (CI/CD)](#15-continuous-integration--delivery-cicd)
  - [16. AI & Machine Learning](#16-ai--machine-learning)
  - [17. .NET Libraries](#17-net-libraries)
  - [Additional considerations](#additional-considerations)
    - [Performance best practices](#performance-best-practices)
    - [Profiling and diagnostics](#profiling-and-diagnostics)
    - [Performances 101](#performances-101)
    - [Security and Cryptography](#security-and-cryptography)
  - [Additional learning resources](#additional-learning-resources)
    - [Books](#books)
    - [YouTube Channels](#youtube-channels)
    - [Blogs](#blogs)
    - [Podcasts](#podcasts)
    - [Other .NET Content creators](#other-net-content-creators)
- [Tools](#tools)

## Understanding the .NET ecosystem

Before going into specifics, you need to have a solid understanding of the **.NET Ecosystem**. Here are a few that you should understand:

## .NET runtimes

In this section, we will look at the main .NET runtimes. We consider .NET runtime as anything that implements **[ECMA-335 Standard for .NET](https://github.com/dotnet/runtime/blob/main/docs/project/dotnet-standards.md)**.

### .NET Framework

[.NET Framework](https://dotnet.microsoft.com/en-us/download/dotnet-framework) is a software development framework for building and running applications on Windows. .NET Framework consists of Common Language Runtime (CLR), .NET Framework Class Library, and Application workloads (WPF, Windows Forms, and ASP.NET). CLR is part of a shared infrastructure that runs code, jit, does garbage collection (C#, VB.NET, F#), etc. The code that CLR manages is called managed code. Code is compiled into Common Intermediate Language (CIL) and stored in assemblies (with .exe or .dll extension). When an application runs, CLR takes an assembly and uses a just-in-time compiler (JIT) to transpile machine code into code that can run on specific computer architecture.

You can use it for both desktop and web development, but it is limited to Windows development, and it comes preinstalled on Windows.

### .NET Core

[.NET Core](https://dotnet.microsoft.com/en-us/download) is one of the runtimes in the .NET Ecosystem. It was released in 2016. and it's [open-sourced](https://github.com/dotnet/core). It was built from scratch as a cross-platform, modular runtime rather than as a new version of .NET Framework. Since .NET 5, it is the only line under active development: .NET Framework 4.8.1 is the final version and receives only security and reliability fixes. .NET Core consists of an App Host (dotnet.exe) that runs CLR and Library. It has a Common language runtime (CoreCLR) and .NET Core Class Library. It supports different application workloads, such as ASP.NET Core (MVC and API), console applications, and UWP.

.NET Core can run on different platforms: Windows Client, Server, IoT, Linux, Ubuntu, FreeBSD, Tizen, and Mac OSX, and can be installed side-by-side of different versions per machine or user.


### The One .NET - .NET 5

[.NET 5](https://dotnet.microsoft.com/en-us/download/dotnet/5.0) was released in November 2020 with the goal of unifying development for desktop, Web, cloud, mobile, gaming, IoT, and AI applications. The earlier setup goal was to produce a single .NET runtime and framework, cross-platform, integrating the best features of .NET Core, .NET Framework, Xamarin, and Mono. However, due to the global health pandemic, the unification was postponed to .NET 6. .NET 5 is a shared code base for .NET Core, Mono, Xamarin, and future .NET implementations. Also, target framework names (TFMs), which express which version of .NET targeting, are updated, so we now have net5.0. This is for code that runs everywhere. It combines and replaces the netcoreapp and netstandard names and net5.0-windows that represent OS-specific flavors of .NET 5 that include net5.0 plus OS-specific bindings.

### The current - .NET 10

[.NET 10](https://learn.microsoft.com/en-us/dotnet/core/whats-new/dotnet-10/overview) is the latest runtime in the .NET Ecosystem. It was released in November 2025, and it unifies development for desktop, Web, cloud, mobile, gaming, IoT, and AI applications. .NET 10 consists of an App Host (dotnet.exe) that runs CLR and Library. It has a Common language runtime (CoreCLR) and the .NET 10 Class Library. It also includes ASP.NET Core 10 and EF Core 10. .NET 10 brings runtime improvements (JIT inlining, devirtualization, stack allocations, AVX10.2, NativeAOT enhancements), new library APIs, and expanded post-quantum cryptography support.

.NET 10 is a **Long Term Support (LTS)** release, supported for three years (until November 2028).

.NET 9 was a **Standard Term Support (STS)** release, supported for two years after the initial release (until November 2026). STS releases are supported for 24 months; LTS releases for a minimum of three years. Releases alternate between LTS and STS.

**What's next:** [.NET 11](https://learn.microsoft.com/en-us/dotnet/core/whats-new/dotnet-11/overview) is in preview and ships in November 2026 as an STS release, together with [C# 15](https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-15) and [EF Core 11](https://learn.microsoft.com/en-us/ef/core/what-is-new/ef-core-11.0/whatsnew). Headline changes are runtime-native async, Zstandard compression in ASP.NET Core, vector search in EF Core, and union types in C#.

![C#/NET Timeline](CSharp-NET_Timeline.png)

## .NET Standard

Different runtimes use different class libraries, e.g., .NET Framework uses .NET Framework class library, while .NET Core contains its class library, as well as Xamarin with its class library. In this way, it's hard to share code between different runtimes, as they use different APIs. Microsoft's solution is the **.NET Standard library**, released in 2016. It represents a set of (formal) specifications that say which APIs you can use and all runtimes implement it. It is the evolution of Portable Class Libraries (PCL). Specific runtimes implement specific versions of .NET Standard (implementing specific APIs). E.g., .NET Framework 4.8.1 implements .NET Standard 2.0, and .NET 10 implements .NET Standard 2.1 ([link](https://learn.microsoft.com/en-us/dotnet/standard/net-standard?tabs=net-standard-1-0#net-implementation-support)). .NET Standard 2.1 is the final version; for code targeting modern .NET only, target the `net10.0` TFM directly instead.

To learn more about the .NET Ecosystem, check [this blog post](https://milan.milanovic.org/post/a-brief-walk-through-net-ecosystem/).

**.NET Release Schedule by Microsoft:**

![.NET Release schedule by Microsoft](release-schedule.png)

## Learning resources

### 1. C#

C# is a programming language developed by Microsoft. It's a language for building anything from desktop applications and games (using Unity) to cloud-based solutions and web services. With **strong support for object-oriented programming** and a rich library, it's designed to be easy and efficient. 

The latest version is **[C# 14](https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-14)**, released in November 2025 with .NET 10. Notable recent additions include [extension members](https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-14#extension-members), the [`field` keyword](https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-14#the-field-keyword), [null-conditional assignment](https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-14#null-conditional-assignment), first-class `Span<T>` conversions, and `partial` constructors/events. [C# 15](https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-15) is in preview and ships with .NET 11 in November 2026, bringing union types, closed hierarchies, extension indexers, and labeled `break`/`continue`.

Check the full C# timeline:

![C# Timeline](csharp-timeline.png)

You need to understand different **C# language features**, such as:

- Object-oriented programming (classes, objects, interfaces, inheritance, polymorphism)
- Variables, data types, and operators
- Reference and value types
- Control flow (conditionals, loops)
- Generics
- Exception handling
- Delegates and events
- Assemblies
- Collections
- LINQ (Language Integrated Query)
- Async and await for asynchronous programming
- Nullable reference types
- Records and pattern matching
- Primary constructors and collection expressions
- `Span<T>`, `Memory<T>`, and `ref struct` types
- Source generators
- File-based apps (`dotnet run app.cs`)

But also **.NET libraries and APIs** for:

- File I/O and serialization
- Collections and data structures
- Networking 
- Multithreading and task parallelism
- Security and cryptography

**Resources**:

- [C# Programming Cheat Sheet](https://github.com/milanm/csharp-cheatsheet) - This cheat sheet serves as a quick reference guide for C# developers at all skill levels.
- [Why C#](https://newsletter.techworld-with-milan.com/p/why-csharp) - A comprehensive overview of C# language features.
- [Microsoft Learn C#](https://dotnet.microsoft.com/en-us/learn/csharp).
- [Microsoft C# Fundamentals for Absolute Beginners](https://learn.microsoft.com/en-us/shows/c-fundamentals-for-absolute-beginners/).
- [Microsoft C# 101](https://learn.microsoft.com/en-us/shows/csharp-101/)
- [Udemy C# for Beginners - Coding From Scratch (.NET Core)](https://www.udemy.com/course/c-and-net-core-for-beginners/)
- [C# Basics for Beginners: Learn C# Fundamentals by Coding](https://www.udemy.com/course/csharp-tutorial-for-beginners/)
- [C# language specification - ECMA-334](https://www.ecma-international.org/publications-and-standards/standards/ecma-334/)
- Learn [dotnet CLI](https://docs.microsoft.com/dotnet/core/tools)
- [NuGet](https://learn.microsoft.com/en-us/nuget/what-is-nuget) package manager
- [Dot Net Perls](https://www.dotnetperls.com/s#c#) - Many code examples in C#
- Advanced concepts:
    - [Become a Full-stack .NET Developer - Advanced Topics](https://www.pluralsight.com/courses/full-stack-dot-net-developer)
    - [Async/Await](https://devblogs.microsoft.com/dotnet/how-async-await-really-works/) by Stephen Toub
    - [Threading in C#](https://www.albahari.com/threading/) by Joseph Albahari
    - [Concurrency](https://www.codeguru.com/csharp/thread-synchronization-c-sharp/) and [Locking](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/statements/lock)
    - [Pattern matching](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/functional/pattern-matching) and [Records](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/record)
    - [Nullable reference types](https://learn.microsoft.com/en-us/dotnet/csharp/nullable-references)
    - [Span<T> and Memory<T>](https://learn.microsoft.com/en-us/dotnet/standard/memory-and-spans/)
    - [Source generators](https://learn.microsoft.com/en-us/dotnet/csharp/roslyn-sdk/source-generators-overview)
    - [File-based apps](https://learn.microsoft.com/en-us/dotnet/core/sdk/file-based-apps) (`dotnet run app.cs`, .NET 10)
    - [Native AOT](https://learn.microsoft.com/en-us/dotnet/core/deploying/native-aot/) and trimming

### 2. General Development Skills

Mastering design patterns, clean code, and version control like Git enables you to write efficient, maintainable code that works and thrives in a team environment. It's the **difference between being a coder and a skilled software engineer**.

Here, you need to know different principles, such as:

**SOLID Principles**:
  - Single Responsibility Principle (SRP)
  - Open/Closed Principle (OCP)
  - Liskov Substitution Principle (LSP)
  - Interface Segregation Principle (ISP)
  - Dependency Inversion Principle (DIP)

But also:

- DRY (Don't Repeat Yourself)
- KISS (Keep It Simple, Stupid)
- YAGNI (You Ain't Gonna Need It)
- Law of Demeter (LoD) or Principle of least knowledge
- Composition over Inheritance
- The principle of least astonishment
- Software architecture styles and patterns (MVC, MVP)

**Resources**:

- Learn [Git](https://newsletter.techworld-with-milan.com/p/how-to-learn-git)
- Learn [Data Structures & Algorithms](https://amzn.to/3LTsZ6o)
- Learn [Clean Code](https://amzn.to/3Qdj91J)
- Learn [Refactoring](https://www.pluralsight.com/courses/refactoring-fundamentals) fundamentals
- Learn [Design Patterns from the book](https://amzn.to/3QcVQVS) or [video tutorials](https://www.pluralsight.com/paths/design-patterns-in-c) or download [cheat sheet](Patterns.png).
  - [Creational Design Patterns](https://refactoring.guru/design-patterns/creational-patterns)
  - [Structural Design Patterns](https://refactoring.guru/design-patterns/structural-patterns)
  - [Behavioral Design Patterns](https://refactoring.guru/design-patterns/behavioral-patterns)
  - [Repository pattern](https://learn.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/infrastructure-persistence-layer-design)
  - [Unit of Work pattern](https://learn.microsoft.com/en-us/aspnet/mvc/overview/older-versions/getting-started-with-ef-5-using-mvc-4/implementing-the-repository-and-unit-of-work-patterns-in-an-asp-net-mvc-application)
- Learn [Main software design](https://newsletter.techworld-with-milan.com/p/main-software-design-principles-you) principles
- Learn [SOLID](https://www.pluralsight.com/courses/principles-oo-design) principles of OO Design in depth.
- Learn [Clean Architecture](https://newsletter.techworld-with-milan.com/p/what-is-clean-architecture)
- Learn [Modular Monolith Architecture](https://newsletter.techworld-with-milan.com/p/what-is-a-modular-monolith)
- Learn [Vertical Slice Architecture](https://www.jimmybogard.com/vertical-slice-architecture/)
- Software Architecture Styles
    - Learn [Fundamentals of Software Architectures](https://amzn.to/3rEtJWh)
    - Learn [Layered](https://www.oreilly.com/library/view/software-architecture-patterns/9781491971437/ch01.html) architecture style
    - Learn [Microservices](https://microservices.io/) and [DAPR](https://dapr.io/)
      - Microservices Patterns
        - [Backend for Frontend](https://microservices.io/patterns/apigateway.html)
        - [CQRS](https://learn.microsoft.com/en-us/azure/architecture/patterns/cqrs)
        - [Event Sourcing](https://learn.microsoft.com/en-us/azure/architecture/patterns/event-sourcing)
        - [Saga](https://learn.microsoft.com/en-us/azure/architecture/patterns/saga)
        - [Actor Model](https://getakka.net/articles/intro/what-are-actors.html)
        - [Inbox pattern](https://learn.microsoft.com/en-us/azure/service-bus-messaging/duplicate-detection)
        - [Sidecar pattern](https://learn.microsoft.com/en-us/azure/architecture/patterns/sidecar)
        - [Outbox pattern](https://learn.microsoft.com/en-us/azure/architecture/databases/guide/transactional-outbox-cosmos)
      - [Data Consistency](https://daily.dev/blog/10-methods-to-ensure-data-consistency-in-microservices)
- Learn [Domain-Driven Design](https://learn.microsoft.com/en-us/archive/msdn-magazine/2009/february/best-practice-an-introduction-to-domain-driven-design) or from [the book](https://amzn.to/49jl0tm)

### 3. ASP.NET Core 

It is a cross-platform, high-performance framework developed by Microsoft for **building web apps, APIs, and microservices**. You can also run your apps on Windows, Linux, or macOS. It's engineered for flexibility and scalability with features like built-in dependency injection and a robust configuration system.

Here, you also need to know **web development fundamentals**, such as:

- HTML, CSS, and JavaScript for front-end development
- HTTP protocols, DNS, request/response model, and RESTful APIs
- Routing, middleware, authentication, and authorization

Note that **Minimal APIs** are now preferred for lightweight APIs, instead of controllers.

**Resources**:

- Web Basics:
    - [How Internet works](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work)
    - [What happens when you type a URL into your browser?](https://newsletter.techworld-with-milan.com/p/what-happens-when-you-type-a-url)
    - [How DNS works](https://newsletter.techworld-with-milan.com/i/135973327/how-dns-works)
    - [HTTP(S) protocol](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview) 
- [ASP.NET MVC](https://dotnet.microsoft.com/en-us/apps/aspnet/mvc)
- [ASP.NET Core Fundamentals by Scott Allen](https://www.pluralsight.com/courses/aspnet-core-fundamentals) course
- [Routing](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/routing)
- [Middlewares](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/middleware)
- [Health Checks](https://learn.microsoft.com/en-us/aspnet/core/host-and-deploy/health-checks)
- [Rate Limiting](https://learn.microsoft.com/en-us/aspnet/core/performance/rate-limit)
- APIs
    - [Web API](https://dotnet.microsoft.com/en-us/apps/aspnet/apis)
    - [Minimal APIs](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/minimal-apis?view=aspnetcore-10.0)
      - [FastEndpoints](https://fast-endpoints.com/)
      - [Built-in validation](https://learn.microsoft.com/en-us/aspnet/core/validation/overview?view=aspnetcore-10.0) (.NET 10)
    - Protocols
        - REST:
          - [REST API Design Best Practices](https://newsletter.techworld-with-milan.com/p/rest-api-design-best-practices)
          - [REST Constraints](https://www.webscrapingapi.com/rest-api-architecture-constraints)
          - [Understanding REST Headers](https://newsletter.techworld-with-milan.com/p/understanding-rest-headers)
          - [REST Maturity Model](https://martinfowler.com/articles/richardsonMaturityModel.html)
          - [HTTP Status Codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Status)
          - [HATEOAS](https://en.wikipedia.org/wiki/HATEOAS)
          - [Data Shaping](https://code-maze.com/data-shaping-aspnet-core-webapi/)
          - [Filtering, Sorting, Pagination](https://www.youtube.com/watch?v=X8zRvXbirMU)
        - GraphQL:
          - [Basics](https://graphql.org/)
          - [Queries](https://chillicream.com/docs/hotchocolate/v15/defining-a-schema/queries)
          - [Mutations](https://chillicream.com/docs/hotchocolate/v15/defining-a-schema/mutations)
          - [Subscriptions](https://chillicream.com/docs/hotchocolate/v15/defining-a-schema/subscriptions)
          - [Distributed Schemas](https://chillicream.com/docs/hotchocolate/v15/distributed-schema)
        - gRPC:
          - [gRPC Fundamentals](https://grpc.io/)
          - [Contracts and .proto files](https://learn.microsoft.com/en-us/aspnet/core/grpc/basics)
          - [Protobuf](https://learn.microsoft.com/en-us/aspnet/core/grpc/protobuf)
          - [Bidirectional communication](https://learn.microsoft.com/en-us/aspnet/core/grpc/client)
          - [Interceptors](https://learn.microsoft.com/en-us/aspnet/core/grpc/interceptors)
    - SDK Clients – Simplify calling external APIs or building resilient API integrations:
      - [IHttpClientFactory](https://learn.microsoft.com/en-us/dotnet/core/extensions/httpclient-factory) – The built-in way to create and pool `HttpClient` instances. -> Recommended
      - [Refit](https://github.com/reactiveui/refit) – Turns your REST API into a live interface via attributes. -> Recommended
      - [RestSharp](https://github.com/restsharp/RestSharp) – Low-level HTTP client wrapper, good for custom scenarios.
      - [Polly](https://github.com/App-vNext/Polly) – Fault-handling (retry, circuit breaker, timeout) for HTTP requests.
      - [Microsoft Resilience](https://learn.microsoft.com/en-us/dotnet/core/resilience/) – New resilience pipeline built into .NET.    
- Dependency Injection
    - [Life Cycles](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection)
    - [Microsoft Extensions Dependency Injection](https://learn.microsoft.com/en-us/dotnet/core/extensions/dependency-injection) -> Recommended
    - [Autofac](https://autofac.org/) -> Still maintained, but rarely needed now that built-in DI covers most cases
    - [Scrutor](https://github.com/khellang/Scrutor)
- [Application Settings & Configurations](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/configuration)
  - [Options pattern](https://learn.microsoft.com/en-us/dotnet/core/extensions/options)
  - [User Secrets](https://learn.microsoft.com/en-us/aspnet/core/security/app-secrets) for local development
- [Filters & Attributes](https://docs.microsoft.com/en-us/aspnet/core/mvc/controllers/filters)
- Security
    - [Identity on ASP.NET Core](https://learn.microsoft.com/en-us/aspnet/core/security/authentication/identity)
    - [Authentication](https://docs.microsoft.com/en-us/aspnet/core/security/authentication) or [this Reddit thread](https://www.reddit.com/r/dotnet/comments/we9qx8/a_comprehensive_overview_of_authentication_in/)
    - [Authorization](https://docs.microsoft.com/en-us/aspnet/core/security/authorization/introduction)
    - [Passkeys in ASP.NET Core Identity](https://learn.microsoft.com/en-us/aspnet/core/release-notes/aspnetcore-10.0) (.NET 10)
    - [Duende IdentityServer](https://duendesoftware.com/products/identityserver) (PAID for commercial use; IdentityServer4 is end of life)
    - [OpenIddict](https://documentation.openiddict.com/) (free OpenID Connect server)
    - [Auth0](https://auth0.com)
    - [OIDC](https://openid.net/connect)
    - [Mutual TLS](https://www.cloudflare.com/learning/access-management/what-is-mutual-tls/) 
    - [Keycloak](https://www.keycloak.org/)   

### 4. Client-Side .NET

If you want to build UIs in .NET, you will need these frameworks. **Razor** is a template engine for creating dynamic HTML, while **Blazor** takes it up a notch, letting you build interactive web UIs using C# instead of JavaScript. **MAUI** is a Xamarin successor made for building cross-platform mobile apps. **Windows Presentation Foundation (WPF)** is a UI framework that creates desktop client applications. **Uno Platform** is an open-source cross-platform UI framework that allows developers to build single-codebase applications for Windows, macOS, Linux, iOS, Android, and Web (via WebAssembly) using .NET.

**Resources**:

- [Razor](https://docs.microsoft.com/aspnet/core/mvc/views/razor)
- [Blazor](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)
  - [Render modes](https://learn.microsoft.com/en-us/aspnet/core/blazor/components/render-modes) (static SSR, Server, WebAssembly, Auto)
- [.NET MAUI](https://github.com/dotnet/maui)
- [WPF](https://learn.microsoft.com/en-us/dotnet/desktop/wpf/overview/?view=netdesktop-10.0)
- [WinUI](https://docs.microsoft.com/en-us/windows/apps/winui/winui3/)
- [Uno Platform](https://platform.uno/)
- [Avalonia](https://avaloniaui.net/)
- Note: [UWP](https://docs.microsoft.com/en-us/windows/uwp/get-started/universal-application-platform-guide) and [WinForms](https://docs.microsoft.com/en-us/dotnet/desktop/winforms/overview/?view=netdesktop-10.0) are also used client-side .NET technologies, though they are in maintenance mode (no major new investment).

### 5. Databases

Good database design ensures efficient data storage and quick retrieval, making your app run smoother and scale easier. **SQL**, the go-to language for database interaction, gives you the power to query, update, and manage the data you've so carefully designed to store.

Here, you need to know:

- SQL Syntax
- Basics of Database design (normal forms, keys, relationships)
- The Difference Between Inner, Left, Right, and Full Join
- SQL Queries Execution Order
- What is Query Optimizer

**Resources**:

- [Database design](https://www.youtube.com/watch?v=ztHopE5Wnpc)
- [Learn SQL](https://newsletter.techworld-with-milan.com/p/how-to-learn-sql)
  - [SELECT FROM](https://www.w3schools.com/sql/sql_select.asp)
  - [WHERE](https://www.w3schools.com/sql/sql_where.asp)
  - [ORDER BY](https://www.w3schools.com/sql/sql_orderby.asp)
  - [GROUP BY, HAVING](https://www.w3schools.com/sql/sql_groupby.asp)
  - [JOINs](http://www.w3schools.com/Sql/sql_join.asp)
  - [Database views](https://www.geeksforgeeks.org/sql-views/)
  - [Stored Procedures](https://www.w3schools.com/sql/sql_stored_procedures.asp)
  - [Functions](https://www.w3schools.com/sql/sql_ref_sqlserver.asp)
  - [Triggers](https://www.geeksforgeeks.org/sql-trigger-student-database/)
- Relational
  - [SQL Server](https://www.microsoft.com/en-us/sql-server)
  - [PostgreSQL](https://www.postgresql.org) - recommended for new projects
  - [SQLite](https://www.sqlite.org/) - embedded database, ideal for local development and tests
  - [MariaDB](https://mariadb.org)
  - [MySQL](https://www.mysql.com)
  - [Azure SQL](https://azure.microsoft.com/en-us/products/azure-sql/database)
- NoSQL
  - [MongoDB](https://docs.microsoft.com/aspnet/core/tutorials/first-mongo-app)
  - [RavenDB](https://github.com/ravendb/ravendb)
  - [Azure Cosmos DB](https://docs.microsoft.com/azure/cosmos-db) - recommended for new projects
  - [Marten](https://martendb.io/) -  (document DB and event store on PostgreSQL)
  - [Apache Cassandra](https://cassandra.apache.org/)
  - [DynamoDB](https://aws.amazon.com/dynamodb/)
- Vector search (for AI workloads):
  - [pgvector](https://github.com/pgvector/pgvector) for PostgreSQL
  - [Vector search in EF Core 11](https://learn.microsoft.com/en-us/ef/core/what-is-new/ef-core-11.0/whatsnew) with SQL Server 2025
- Tools:
  - [SQLFlow](https://sqlflow.gudusoft.com/#/) - a great tool to visualize SQL queries.
- Security:
  - [TLS](https://dev.to/scylladb/database-101-ssltls-for-beginners-4lmn)
  - [Transparent Data Encryption](https://learn.microsoft.com/en-us/sql/relational-databases/security/encryption/transparent-data-encryption)
  - [Always Encrypted](https://learn.microsoft.com/en-us/sql/relational-databases/security/encryption/always-encrypted-database-engine)
- [Consistency models](https://www.baeldung.com/cs/eventual-consistency-vs-strong-eventual-consistency-vs-strong-consistency)

### 6. ORM

Object-relational mapping (ORM) is like a translator between your object-oriented C# code and the relational database, eliminating the tedious task of writing SQL queries for basic CRUD operations. Using ORM frameworks like Entity Framework, you can **manipulate data as objects in your code, making it more readable and maintainable**. This speeds up development, minimizes errors, and lets you focus on complex business logic rather than wrestling with database syntax.

For **Entity Framework**, you need to know the following:

- DbContext and DbSet for managing database connections and querying data
- Code-First and Database-First approaches for defining data models
- Migrations for managing database schema changes
- Querying data using LINQ and raw SQL
- Tracking changes and saving data

**Resources**:

- [Entity Framework Core](https://learn.microsoft.com/en-us/ef/core)
    - [Code First Migrations](https://learn.microsoft.com/en-us/ef/core/managing-schemas/migrations/?tabs=dotnet-core-cli)
    - [Change Tracker API](https://learn.microsoft.com/en-us/ef/core/change-tracking/)
    - [Lazy Eager Explicit Loading](https://learn.microsoft.com/en-us/ef/core/querying/related-data/) 
    - Entity Relations:
      - [One-to-One](https://learn.microsoft.com/en-us/ef/core/modeling/relationships/one-to-one)
      - [One-to-Many](https://learn.microsoft.com/en-us/ef/core/modeling/relationships/one-to-many)
      - [Many-to-Many](https://learn.microsoft.com/en-us/ef/core/modeling/relationships/many-to-many)
    - Querying Data:
      - [Eager Loading](https://learn.microsoft.com/en-us/ef/core/querying/related-data/eager)
      - [Explicit Loading](https://learn.microsoft.com/en-us/ef/core/querying/related-data/explicit)
      - [Lazy Loading](https://learn.microsoft.com/en-us/ef/core/querying/related-data/lazy)
      - [AsNoTracking](https://learn.microsoft.com/en-us/ef/core/querying/tracking)
      - [Filtering](https://www.learnentityframeworkcore.com/dbset/querying-data)
      - [Sorting](https://code-maze.com/sorting-aspnet-core-webapi/)
      - [Paging](https://learn.microsoft.com/en-us/ef/core/querying/pagination)
      - [Projections](https://makolyte.com/ef-core-aggregate-select-queries/)
      - [Aggregations](https://www.csharptutorial.net/entity-framework-core-tutorial/ef-core-group-by/)
    - Advanced Querying:
      - [Compiled Queries](https://learn.microsoft.com/en-us/ef/core/performance/advanced-performance-topics#compiled-queries)
      - [Split Queries](https://learn.microsoft.com/en-us/ef/core/querying/single-split-queries)
      - [Functions](https://learn.microsoft.com/en-us/ef/core/querying/database-functions)
      - [Global Query Filters](https://learn.microsoft.com/en-us/ef/core/querying/filters)
    - Advanced Writing:
      - [Batch Update](https://learn.microsoft.com/en-us/ef/core/performance/efficient-updating)
      - [Transactions](https://learn.microsoft.com/en-us/ef/core/saving/transactions)
      - Concurrency: [Optimistic Locking](https://www.learnentityframeworkcore.com/concurrency) and [Pessimistic Locking](https://learn.microsoft.com/en-us/ef/core/saving/concurrency)
      - [Transaction Isolation Levels](https://www.bytehide.com/blog/transactions-ef-core)
    - Migrations:
      - [Add-Migration](https://learn.microsoft.com/en-us/ef/core/managing-schemas/migrations/?tabs=dotnet-core-cli#add-migration)
      - [Update-Database](https://www.learnentityframeworkcore.com/migrations/update-database)
      - [Scaffolding](https://learn.microsoft.com/en-us/ef/core/managing-schemas/scaffolding/)
      - [Applying Migrations](https://learn.microsoft.com/en-us/ef/core/managing-schemas/migrations/applying)
      - [Migrations with multiple providers](https://learn.microsoft.com/en-us/ef/core/managing-schemas/migrations/providers)
    - Advanced Modeling Techniques:
      - [Owned Entities](https://learn.microsoft.com/en-us/ef/core/modeling/owned-entities)
      - [Table per Hierarchy (TPH)](https://www.learnentityframeworkcore.com/inheritance/table-per-hierarchy)
      - [Table per Type (TPT)](https://www.learnentityframeworkcore.com/inheritance/table-per-type)
      - [Table per Concrete Class (TPC)](https://code-maze.com/efcore-how-and-when-to-use-tpc-inheritance-mapping/)
      - [Keyless Entities](https://learn.microsoft.com/en-us/ef/core/modeling/keyless-entity-types)
      - [Complex Types](https://www.learnentityframeworkcore.com/model/complex-type)
      - [Value Objects](https://learn.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/implement-value-objects)
    - Patterns:
      - [Repository Pattern](https://learn.microsoft.com/en-us/aspnet/core/data/ef-mvc/intro?view=aspnetcore-10.0#repository-pattern)
      - [Unit of Work Pattern](https://learn.microsoft.com/en-us/aspnet/core/data/ef-mvc/intro?view=aspnetcore-10.0#unit-of-work-pattern)      
    - Advanced topics:
      - [Temporal Tables](https://learn.microsoft.com/en-us/ef/core/providers/sql-server/temporal-tables)
      - [Shadow properties](https://learn.microsoft.com/en-us/ef/core/modeling/shadow-properties)
      - [DBContext pooling](https://learn.microsoft.com/en-us/ef/core/performance/advanced-performance-topics?tabs=with-di%2Cexpression-api-with-constant#dbcontext-pooling)
      - [JSON Mapping](https://learn.microsoft.com/en-us/ef/core/what-is-new/ef-core-10.0/whatsnew) (complex types mapped to JSON columns)
- [Dapper](https://github.com/StackExchange/Dapper)
- [LINQ](https://www.dotnetnakama.com/blog/understanding-the-dot-net-language-integrated-query-linq/)
     - [Index, CountBy, AggregateBy](https://timdeschryver.dev/blog/new-linq-methods-in-c-13-index-countby-aggregateby)
- [ADO.NET](https://learn.microsoft.com/en-us/dotnet/framework/data/adonet/)

### 7. Testing

**Unit tests** focus on isolated pieces of your code, **integration tests** ensure different parts play well together, and **end-to-end tests** validate the entire user journey within your application. Together, they form a safety net, catching bugs early, simplifying debugging, and making your codebase robust and maintainable.

Here you need to know:

- Test frameworks (xUnit, NUnit, MSTest, TUnit)
- Test runners and test explorers
- Asserts and test attributes
- Mocking libraries (NSubstitute, etc.)

**Resources**:

- [Unit Testing](https://www.pluralsight.com/courses/advanced-unit-testing)
    - Frameworks
      - [xUnit](https://xunit.net/) (v3) -> Recommended
      - [NUnit](https://nunit.org/)
      - [MSTest](https://docs.microsoft.com/dotnet/core/testing/unit-testing-with-mstest)
      - [TUnit](https://thomhurst.github.io/TUnit/)
    - [Microsoft.Testing.Platform](https://learn.microsoft.com/en-us/dotnet/core/testing/microsoft-testing-platform-intro) - the new test runner that replaces VSTest
    - Mocking
      - [NSubstitute](https://github.com/nsubstitute/NSubstitute) -> Recommended
      - [Moq](https://github.com/devlooped/moq)
    - Assertion
      - [Shouldly](https://github.com/shouldly/shouldly) -> Recommended
      - [xUnit Assert](https://xunit.net/)
      - [Fluent Assertions](https://fluentassertions.com/) (PAID)
      - [Awesome Assertions](https://awesomeassertions.org/)
- Integration Testing
    - [WebApplicationFactory](https://docs.microsoft.com/aspnet/core/test/integration-tests)
    - [TestServer](https://learn.microsoft.com/en-us/aspnet/core/test/integration-tests?view=aspnetcore-10.0)
    - [Testcontainers](https://dotnet.testcontainers.org/)
    - [Respawn](https://github.com/jbogard/Respawn)
- Snapshot Testing
     - [Verify](https://github.com/VerifyTests/Verify)
- Mutation Testing
     - [Stryker](https://stryker-mutator.io/)
- Behavior Testing
     - [Reqnroll](https://github.com/reqnroll/Reqnroll)
- End-to-End Testing
     - [Playwright](https://playwright.dev/)
     - [Selenium](https://www.selenium.dev/)
     - [Cypress](https://www.cypress.io/)
- Performance Testing
     - [K6](https://github.com/grafana/k6)
     - [JMeter](https://github.com/apache/jmeter)
     - [BenchmarkDotNet](https://benchmarkdotnet.org/)
- Load Testing
     - [NBomber](https://nbomber.com/)
- Test Data Generators
    - [Bogus](https://github.com/bchavez/Bogus) -> Recommended
    - [AutoFixture](https://github.com/AutoFixture/AutoFixture) 

### 8. Logging

Logging captures runtime information, errors, and other crucial data that can help you quickly identify and fix issues, making your application more reliable and secure. Logging frameworks like **NLog** or **Serilog** integrate seamlessly into .NET, giving you a real-time diagnostic tool indispensable for monitoring application health, troubleshooting problems, and even gathering insights for future development. 

**Resources**:

- [Serilog](https://github.com/serilog/serilog)
- [NLog](https://github.com/NLog/NLog)
- [Microsoft.Extensions.Logging](https://learn.microsoft.com/en-us/dotnet/core/extensions/logging)
  - [LoggerMessage source generator](https://learn.microsoft.com/en-us/dotnet/core/extensions/logger-message-generator) for high-performance logging
- [Seq](https://datalust.co/seq) - log server for structured logs

### 9. Communication

In .NET we have three types of communication: Real-time communication, Synchronous, and Asynchronous communication. **Real-time communication** technologies, like SignalR in the .NET ecosystem, enable these functionalities by maintaining a constant connection between server and client. **Synchronous communication** is mainly done by using through HTTP Client, while **asynchronous communication** is done through different messaging and event-based frameworks and libraries. Messaging systems act as a middleman between different parts of your system, allowing them to communicate without being directly connected. **Event handlers**, on the other side, are used for handling events within a single application. They facilitate a publisher-subscriber model where one part of the application can raise an event that other parts can react to.

**Resources**:

- Real time communication:
    - [SignalR Core](https://docs.microsoft.com/aspnet/core/signalr)
    - [WebSockets](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/websockets) 
    - [Server-Sent Events](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/minimal-apis/responses?view=aspnetcore-10.0) (built-in since .NET 10)
    - [Socket.IO](https://github.com/doghappy/socket.io-client-csharp)
- Synchronous communication: 
    - [HTTP Client](https://learn.microsoft.com/en-us/dotnet/api/system.net.http.httpclient?view=net-10.0) via [IHttpClientFactory](https://learn.microsoft.com/en-us/dotnet/core/extensions/httpclient-factory)
- Asynchronous communication: 
    - Message brokers:
         - [Azure Service Bus](https://docs.microsoft.com/azure/service-bus-messaging/service-bus-messaging-overview)
         - [RabbitMQ](https://www.rabbitmq.com/tutorials/tutorial-one-dotnet.html)
         - [ActiveMQ](https://activemq.apache.org/)
         - [NetMQ](https://netmq.readthedocs.io/en/latest/)
         - [Apache Kafka](https://kafka.apache.org/)
         - [Message Queues](https://www.geeksforgeeks.org/message-queues-system-design/)
         - [Message Queue vs Pub-Sub](https://systemdesignschool.io/blog/message-queue-vs-pub-sub)
         - [Dead Letter Exchange](https://medium.com/@shivanksingh01/rabbitmq-dead-letter-exchange-a-comprehensive-guide-node-js-b62967a76f10)
         - [Handling Duplicate Messages](https://codeopinion.com/handling-duplicate-messages-idempotent-consumers/)
     - Message bus:
         - [MassTransit](https://github.com/MassTransit/MassTransit) -> Recommended
         - [Rebus](https://github.com/rebus-org/Rebus)
         - [Azure Service Bus](https://docs.microsoft.com/azure/service-bus-messaging/service-bus-messaging-overview)
         - [NServiceBus](https://learn.microsoft.com/en-us/azure/service-bus-messaging/build-message-driven-apps-nservicebus?tabs=Sender) (PAID)
         - [EasyNetQ](https://easynetq.com/)
         - [Wolverine](https://wolverinefx.net/)
     - Event handlers:
         - [Azure Event Hub](https://docs.microsoft.com/azure/event-hubs/event-hubs-about)
         - [Azure Event Grid](https://docs.microsoft.com/azure/event-grid/overview)

### 10. Background tasks

These services run tasks in the background, freeing up your application to focus on user interactions. Whether **data processing, automated emails, or periodic clean-ups**, background services ensure these tasks don't slow down or interrupt the user experience. 

**Resources**:

- [Background Service](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/host/hosted-services)
- [HangFire](https://github.com/HangfireIO/Hangfire)
- [Quartz](https://github.com/quartznet/quartznet)
- [Coravel](https://docs.coravel.net/Scheduler/)
- [TickerQ](https://tickerq.net/)

### 11. Caching

Caching is like your app's personal short-term memory, storing frequently accessed data so it **can be quickly retrieved without accessing your database**. By reducing database load and speeding up data access, caching gives your app the competitive edge it needs to meet user demands for responsiveness and availability.

**Resources**:

- [Memory Cache](https://docs.microsoft.com/aspnet/core/performance/caching/memory)
  - [FusionCache](https://github.com/ZiggyCreatures/FusionCache)
- [Hybrid Cache](https://learn.microsoft.com/en-us/aspnet/core/performance/caching/hybrid?view=aspnetcore-10.0)
- [Redis](https://redis.io/)
  - [Valkey](https://valkey.io/) and [Garnet](https://microsoft.github.io/garnet/) - Redis-compatible alternatives
- Application-Level
   - [Built-in](https://learn.microsoft.com/en-us/aspnet/core/performance/caching/response)
   - [Output Caching](https://learn.microsoft.com/en-us/aspnet/core/performance/caching/output?source=recommendations)

### 12. Observability   

These tools provide **real-time insights into your application's performance**, user behavior, and error rates, enabling you to address issues before they escalate into full-blown problems proactively.

- **Monitoring** focuses on the health and availability of services and systems, often triggering alerts for predefined conditions.

- **Telemetry** collects, processes, and transmits data from systems, enabling analysis of patterns, trends, and anomalies.

**Resources**:

- [Prometheus](https://github.com/prometheus/prometheus)
- [Grafana](https://github.com/grafana/grafana)
- [Datadog](https://www.datadoghq.com)
- [ELK Stack](https://www.elastic.co/what-is/elk-stack)
- [OpenTelemetry](https://github.com/open-telemetry/opentelemetry-dotnet) - the standard for traces, metrics, and logs in .NET.
- [Aspire Dashboard](https://learn.microsoft.com/en-us/dotnet/aspire/fundamentals/dashboard/overview) - local OpenTelemetry viewer for logs, traces, and metrics.
- [Jaeger](https://www.jaegertracing.io/)
- [Azure Application Insights](https://docs.microsoft.com/azure/azure-monitor/app/app-insights-overview)
- [Azure Log Analytics](https://docs.microsoft.com/azure/azure-monitor/logs/log-analytics-overview)

### 13. Containerization

Container solutions encapsulate your .NET application, libraries, and runtime into isolated containers. This **enables consistency across multiple development and production environments**, resolving dependency issues. With features like layered file systems, you can easily manage container images for ASP.NET, .NET Core, or other .NET services, optimizing build times and resource utilization.

**Resources**:
- Containers
    - [Docker](https://www.docker.com)
      - [Networking](https://docs.docker.com/engine/network/)
      - [Env Variables](https://docs.docker.com/compose/how-tos/environment-variables/set-environment-variables/)
      - [Dockerfile](https://docs.docker.com/engine/reference/builder/)
      - [Docker CLI](https://docs.docker.com/engine/reference/commandline/cli/)
      - [Volumes](https://docs.docker.com/storage/volumes/)
    - [Docker Compose](https://docs.docker.com/compose/)
    - [Podman](https://podman.io/)
    - [.NET SDK container publish](https://learn.microsoft.com/en-us/dotnet/core/containers/sdk-publish) - build images with `dotnet publish`, no Dockerfile needed
    - [Chiseled images](https://devblogs.microsoft.com/dotnet/announcing-dotnet-chiseled-containers/) - minimal, hardened base images
    - [Docker Hub](https://hub.docker.com/)
    - [Azure Container Registry](https://learn.microsoft.com/en-us/azure/container-registry/container-registry-intro)
- Orchestration
    - [Kubernetes](https://kubernetes.io)
    - [Azure Kubernetes Service (AKS)](https://azure.microsoft.com/en-us/products/kubernetes-service)
    - [Helm](https://helm.sh/)
    - [Azure Container Apps](https://docs.microsoft.com/en-us/azure/container-apps/overview)

### 14. Cloud

Cloud providers provide a layer of APIs to abstract infrastructure and provision it based on security and billing boundaries. The cloud **runs on servers in data centers**, but the abstractions cleverly give the appearance of interacting with a single "platform" or large application. The ability to quickly provision, configure, and secure resources with cloud providers has been key to the tremendous success and complexity of modern DevOps.

The most popular cloud providers in the market are **AWS** and **Azure**, as well as **Google Cloud**.

Also, Microsoft offers **Aspire** (formerly .NET Aspire) to simplify cloud-native and microservices development with orchestration, service discovery, and a developer dashboard. It now ships on its own cadence (Aspire 13.x), decoupled from the .NET release schedule.

Here, you must know how to manage users and administration, networks, virtual servers, etc.

**Resources**:

- [AWS](https://aws.amazon.com/)
  - [AWS S3](https://aws.amazon.com/s3/)
  - [DynamoDB](https://aws.amazon.com/dynamodb/)
  - [SQS/SNS](https://aws.amazon.com/blogs/dotnet/event-driven-net-applications-with-aws-lambda-and-amazon-eventbridge/)
  - [AWS Kinesis](https://docs.aws.amazon.com/sdk-for-net/v3/developer-guide/csharp_kinesis_code_examples.html)
  - [Amazon EventBridge](https://aws.amazon.com/eventbridge/)
  - [AWS Secrets Manager](https://docs.aws.amazon.com/secretsmanager/latest/userguide/intro.html)
  - [AWS Lambda](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)
- [Azure](https://azure.microsoft.com/)
  - [Azure App Service](https://learn.microsoft.com/en-us/azure/app-service/overview)
  - [Managed Identity](https://learn.microsoft.com/en-us/entra/identity/managed-identities-azure-resources/overview)
  - [Azure Functions](https://learn.microsoft.com/en-us/azure/azure-functions/functions-overview)
  - [Azure Service Bus](https://learn.microsoft.com/en-us/azure/service-bus-messaging/service-bus-dotnet-get-started-with-queues)
  - [Azure Event Hubs](https://learn.microsoft.com/en-us/azure/event-hubs/event-hubs-dotnet-standard-getstarted-send)
  - [Application Insights](https://learn.microsoft.com/en-us/azure/azure-monitor/app/app-insights-overview)
  - [Azure Key Vault](https://azure.microsoft.com/en-us/products/key-vault)
  - [Azure Storage](https://learn.microsoft.com/en-us/azure/storage/common/storage-introduction)
  - [Azure CosmosDB](https://learn.microsoft.com/en-us/azure/cosmos-db/)
- [Google Cloud](https://cloud.google.com/)
- [Aspire](https://learn.microsoft.com/en-us/dotnet/aspire/get-started/aspire-overview/) *(cloud-native app model: orchestration, service discovery, and dashboard for microservices)*
- API Gateway:
  - [Envoy](https://www.envoyproxy.io/)
  - [YARP](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/servers/yarp/getting-started?view=aspnetcore-10.0)
  - [Nginx](https://nginx.org/)
  - [Service Discovery](https://learn.microsoft.com/en-us/dotnet/core/extensions/service-discovery?tabs=dotnet-cli)

### 15. Continuous Integration & Delivery (CI/CD)

CI/CD automates the building, testing, and deployment stages into a streamlined, error-resistant pipeline. This means **faster releases, bug fixes, and more time to focus on feature development**.

Here you need to know how to:

- Build and deployment tools (MSBuild, dotnet CLI)
- Version control systems (Git, Azure DevOps)
- CI/CD platforms (GitHub Actions, Azure Pipelines, Jenkins, TeamCity)

**Resources**:

- [DevOps concepts](https://newsletter.techworld-with-milan.com/p/devops-roadmap-2023)
- Services:
    - [GitHub Actions](https://github.com/features/actions)
    - [Gitlab CI](https://docs.gitlab.com/ee/ci)
    - [Azure Pipelines](https://azure.microsoft.com/en-us/services/devops/pipelines)
    - [AWS CodePipeline](https://aws.amazon.com/codepipeline/)
    - [Jenkins](https://www.jenkins.io)
    - [TeamCity](https://www.jetbrains.com/teamcity)
- Build hygiene:
  - [Central Package Management](https://learn.microsoft.com/en-us/nuget/consume-packages/central-package-management)
  - [NuGet Audit](https://learn.microsoft.com/en-us/nuget/concepts/auditing-packages) for vulnerable dependencies
  - [dotnet format](https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-format) and [code analyzers](https://learn.microsoft.com/en-us/dotnet/fundamentals/code-analysis/overview)
  - [Dependabot](https://docs.github.com/en/code-security/dependabot) or [Renovate](https://docs.renovatebot.com/) for dependency updates
- Infrastructure as code (IaC):
  - [Terraform](https://www.terraform.io/)
  - [Pulumi](https://www.pulumi.com/)
  - [Bicep](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/)

Check the full [DevOps Roadmap](https://github.com/milanm/DevOps-Roadmap). 

### 16. AI & Machine Learning

AI & Machine Learning enable software to learn from data, recognize patterns, and generate insights without explicit programming. In the .NET ecosystem, AI is increasingly used for automation, predictions, recommendations, and natural language processing.

While traditional machine learning relies on structured data and models, modern AI advances—such as large language models (LLMs)—enable applications to understand and generate human-like text, images, and code. The .NET ecosystem now has first-class abstractions for building LLM-powered apps, RAG pipelines, and agentic workflows that integrate with OpenAI, Azure, and local models.

For a .NET developer, key areas to understand include:

- Basic Machine Learning concepts – classification, regression, and neural networks
- AI-powered applications – using LLMs, chatbots, and intelligent search
- Retrieval-Augmented Generation (RAG) – embeddings, vector search, and grounding LLMs on your data
- Agents & tool calling – function/tool calling, orchestration, and the Model Context Protocol (MCP)
- Cloud AI Services – leveraging Azure AI Foundry and OpenAI APIs

**Resources**:

- Building blocks
  - [Microsoft.Extensions.AI (MEAI)](https://learn.microsoft.com/en-us/dotnet/ai/microsoft-extensions-ai) – Unified `IChatClient`/`IEmbeddingGenerator` abstractions over any provider. -> Recommended foundation
  - [Microsoft Agent Framework](https://learn.microsoft.com/en-us/agent-framework/overview/agent-framework-overview) – Unified successor to Semantic Kernel + AutoGen for building agents and workflows. 1.0 shipped in April 2026. -> Recommended for agents
  - [Semantic Kernel](https://github.com/microsoft/semantic-kernel) – Now in maintenance mode (bug and security fixes only); new development happens in the Agent Framework.
  - [Microsoft.Extensions.VectorData](https://www.nuget.org/packages/Microsoft.Extensions.VectorData.Abstractions) – Unified abstractions over vector stores for RAG.
  - [Model Context Protocol (C# SDK)](https://github.com/modelcontextprotocol/csharp-sdk) – Build MCP servers/clients to expose tools and data to AI models.
- Models & inference
  - [ML.NET](https://dotnet.microsoft.com/en-us/apps/machinelearning-ai/ml-dotnet) – Classic ML (classification, regression, recommendation) in .NET.
  - [ONNX Runtime](https://onnxruntime.ai/) – Run pretrained models locally for inference.
  - [OllamaSharp](https://github.com/awaescher/OllamaSharp) – Run and consume local LLMs via Ollama.
  - [Foundry Local](https://learn.microsoft.com/en-us/azure/foundry-local/) – Run Azure AI Foundry models on-device.
- Vector stores
  - [pgvector](https://github.com/pgvector/pgvector), [Qdrant](https://qdrant.tech/), [Azure AI Search](https://learn.microsoft.com/en-us/azure/search/)
- Provider SDKs
  - [OpenAI .NET SDK](https://github.com/openai/openai-dotnet) – Official `OpenAI` NuGet package.
  - [Azure AI Foundry](https://learn.microsoft.com/en-us/azure/ai-foundry/) – Azure's unified platform for models, agents, and AI services.
- AI Tools:
  - Chat-based
    - [ChatGPT](https://openai.com/chatgpt)
    - [Claude](https://www.anthropic.com/claude)
    - [Gemini](https://gemini.google.com/)
  - Web-based
    - [Bolt](https://bolt.new/)
    - [Replit](https://replit.com/)
    - [Lovable](https://lovable.dev/)
  - Agentic / coding
    - [GitHub Copilot](https://github.com/features/copilot) (+[Customizations](https://github.com/github/awesome-copilot))
    - [Claude Code](https://www.anthropic.com/claude-code)
    - [OpenAI Codex CLI](https://github.com/openai/codex)
    - [Gemini CLI](https://github.com/google-gemini/gemini-cli)
    - [Aider](https://aider.chat/)
  - IDE
    - [Visual Studio / VS Code Copilot](https://visualstudio.microsoft.com/github-copilot/)
    - [Cursor](https://www.cursor.com/)
    - [Windsurf](https://windsurf.com/)

### 17. .NET Libraries

Some useful .NET libraries. Note that not all libraries will be used by everyone, it mainly depends on a project you work on.

- **[MediatR](https://github.com/jbogard/MediatR)** – Mediator pattern implementation in .NET. (Now under a **commercial license** for most production use; not recommended -> manual handlers are better)
  - **[Mediator](https://github.com/martinothamar/Mediator)** – Source-generated, MIT-licensed alternative to MediatR.
  - **[Relevox](https://github.com/tunahanaliozturk/relevox)** – Source-generated, MIT-licensed alternative that keeps MediatR 12's handler signatures, with a code fix for migrating.
- **[Polly](https://github.com/App-vNext/Polly)** – Fault-handling library that allows expressing policies such as Retry and Circuit Breaker.
- **[Benchmark.NET](https://github.com/dotnet/BenchmarkDotNet)** – .NET library for benchmarking.
- **[YARP](https://microsoft.github.io/reverse-proxy/)** – Reverse proxy server.
- **OpenAPI / API documentation** – ASP.NET Core ships [built-in OpenAPI document generation](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/openapi/overview) (`Microsoft.AspNetCore.OpenApi`); Swashbuckle is no longer in the default .NET 9+ templates.
  - **[Scalar](https://github.com/scalar/scalar)** – Modern, interactive API reference UI (a popular Swagger UI replacement). -> Recommended
  - **[NSwag](https://github.com/RicoSuter/NSwag)** – OpenAPI/Swagger toolchain with client code generation.
  - **[Swashbuckle](https://github.com/domaindrivendev/Swashbuckle.AspNetCore)** – Classic Swagger tooling for ASP.NET Core (community-maintained).
- **[FluentValidation](https://github.com/JeremySkinner/FluentValidation)** – The most popular library for building strongly-typed validation rules with fluent syntax.
- **Object Mapping** – Libraries for transforming between domain models, DTOs, and view models:
  - **[AutoMapper](https://github.com/AutoMapper/AutoMapper)** – Convention-based mapping using profiles. (Now under a **commercial license** for most production use; not recommended -> use manual mapping)
  - **[Mapster](https://github.com/MapsterMapper/Mapster)** – Lightweight, fast, and flexible.
  - **[Mapperly](https://github.com/riok/mapperly)** – Compile-time, source generator-based mapper for performance and type safety. (better alternative to AutoMapper)
- **[Humanizer](https://github.com/Humanizr/Humanizer)** – Turns strings, enums, dates, and numbers into human-readable text.
- **[CsvHelper](https://github.com/JoshClose/CsvHelper)** – Read and write CSV files.

## Additional considerations

In addition to this, you also need to know the following:

### Performance best practices

Performances play an essential role in .NET applications. Here you need to know:

#### Profiling and diagnostics

These tools can help you identify and debug different performance bottlenecks you have in your code. For this, you can use other tools, such as:

- [PerfView](https://joshthecoder.com/2023/10/23/using-perfview-to-diagnose-high-cpu-in-an-aspnet-app.html)
- [Visual Studio Profiler](https://learn.microsoft.com/en-us/visualstudio/profiling/profiling-feature-tour?view=vs-2022)
- [dotTrace](https://www.jetbrains.com/profiler/) and [dotMemory](https://www.jetbrains.com/dotmemory/)
- [dotnet-counters, dotnet-trace, and dotnet-dump](https://learn.microsoft.com/en-us/dotnet/core/diagnostics/tools-overview) - cross-platform CLI diagnostics

#### Performances 101

Along with tools, you should be aware of different performance best practices for .NET:

- **Caching** (in-mem Memory Cache or Redis)

- **Database Optimization** (optimize queries, proper indexing, connection pooling)

- **Async Programming** (offload all CPU extensive or I/O bound operations to DB, file systems, ext. systems)

- **Use Entity Framework wisely** (use eager loading, projections, and optimizations like compiled queries)

- **Memory management** (use value types and be cautious with large object graphs. Use dispose pattern to db connections or streams. Avoid boxing/unboxing. Use StringBuilder instead of String for a large number of concatenations.)

- **HTTP Caching** (use ETags, Last-Modified headers)

- **Minimize Round-Trips** (reduce the number of HTTP requests and database round-trips)

- **Content Delivery Networks (CDNs)** (Offload static assets (CSS, JavaScript, images) to CDNs for faster delivery to users)

- **Compression** (Enable GZIP or Brotli compression for HTTP responses to reduce data transfer size)

- **Logging and Tracing** (Avoid excessive logging in production. Use distributed tracing across microservices.)

- **Parallelism and Concurrency** (Utilize parallelism and multithreading for CPU-bound tasks using Parallel class or Task Parallel Library (TPL))

- **Resource Optimization** (Optimize images and assets for the Web to reduce load times)

- **HTTP2 over SSL** (now make intelligent decisions about the page content)

- **Measure and Monitor Performance** (use VS Diagnostic Tools, App Insights, or BenchmarkDotNet)

- **Use Span<> instead of collections** (spans can represent a contiguous section of memory; this means we can use them to operate over arrays)

- **Native AOT and trimming** (publish ahead-of-time compiled, self-contained apps for faster startup and a smaller footprint)

Check more about performances in the [Awesome .NET Performance](https://github.com/adamsitnik/awesome-dot-net-performance) repo.

### Security and Cryptography

Security plays an essential role in application development. The most critical aspects of security in the .NET world are:

- [**Authentication and Authorization**](https://learn.microsoft.com/en-us/aspnet/web-api/overview/security/authentication-and-authorization-in-aspnet-web-api) concepts:
  - Cookies
  - ASP.NET Core Identity for user management
  - .NET OIDC middleware
  - OAuth and OpenID Connect for 3rd-party authentication
  - JWT (JSON Web Tokens) for token-based authentication
  - Role-based and claims-based authorization

- [**Cryptography and Data Protection**](https://learn.microsoft.com/en-us/dotnet/standard/security/cross-platform-cryptography) concepts:
  - Symmetric and asymmetric encryption algorithms
  - .NET Core Data Protection APIs
  - Hashing and digital signatures
  - Secure random number generation

- **Web hardening** concepts:
  - [OWASP Top 10](https://owasp.org/www-project-top-ten/)
  - [CORS](https://learn.microsoft.com/en-us/aspnet/core/security/cors)
  - [CSRF protection](https://learn.microsoft.com/en-us/aspnet/core/security/anti-request-forgery)
  - [HTTPS and HSTS](https://learn.microsoft.com/en-us/aspnet/core/security/enforcing-ssl)
  - Secrets management ([User Secrets](https://learn.microsoft.com/en-us/aspnet/core/security/app-secrets) locally, [Azure Key Vault](https://azure.microsoft.com/en-us/products/key-vault) in production)
  - Dependency auditing ([NuGet Audit](https://learn.microsoft.com/en-us/nuget/concepts/auditing-packages))

## Additional learning resources

- [Pluralsight learning platform](https://www.pluralsight.com/browse?q=C%20sharp&type=all&sort=highest) - Learn C#/.NET mostly from Microsoft MVPs.
- [Awesome .NET!](https://github.com/quozd/awesome-dotnet) - A collection of awesome .NET libraries, tools, frameworks, and software.
- [Microsoft .NET Architecture Guides](https://dotnet.microsoft.com/en-us/learn/dotnet/architecture-guides) - Learn how to build production-ready .NET apps with free application architecture guidance.

### Books

#### Beginners
- [Learn C# in One Day and Learn It Well](https://amzn.to/3Qld3fT), Jamie Chan - the best for beginners (Rating: 4.4/5)
- [C#: Programming Basics for Absolute Beginners](https://amzn.to/4kbSNcC), Nathan Clark (Rating: 4/5)
- [Starting out with Visual C#](https://amzn.to/4jULLsY), Tony Gaddis (Rating: 4.7/5)
- [The C# Yellow book](http://www.csharpcourse.com/) (free) - the best book overall (Rating: 4.4/5)

#### Intermediate

- [C# in Depth: Fourth Edition](https://amzn.to/3ZPcZbq) by Jon Skeet - the best for intermediate (Rating: 4.6/5)
- [Agile Principles, Patterns, and Practices in C#](https://amzn.to/43gXwDd) by Robert Martin, Micah Martin (Rating: 4.5/5)
- [Adaptive Code via C#: Agile coding with design patterns and SOLID principles](https://amzn.to/43f4E2W) by Gary McLean Hall (Rating: 4.5/5)
- [Head First C#: A Learner’s Guide to Real-World Programming with C# and .NET Core](https://amzn.to/3S3sB85) by Andrew Stellman, Jennifer Greene (Rating: 4.5/5)
- [C# 12 in a Nutshell: The Definitive Reference](https://amzn.to/43f4LeS) by Joseph Albahari (Rating: 4.6/5)
- [C# 14 and .NET 10 – Modern Cross-Platform Development Fundamentals](https://amzn.to/49W9V3k) by Mark J. Price (Rating: 4.6/5)
- [Dependency Injection Principles, Practices, and Patterns](https://amzn.to/43MStur) by Mark Seemann, Steven van Deursen (Rating: 4.7/5)

#### Advanced
- [Concurrency in C# Cookbook: Asynchronous, Parallel, and Multithreaded Programming](https://amzn.to/490EMtu) - the best for advanced (Rating: 4.6/5)
- [Professional C# and .NET](https://amzn.to/458YHHb) by Christian Nagel (Rating: 4.3/5)
- [CLR via C#](https://amzn.to/4j3AyFp) by Jeffrey Richter (Rating: 4.6/5)
- [Functional Programming in C#: How to write better C# code](https://amzn.to/4mgURSr) (Rating: 4.6/5)

![Roadmap](Books.jpg)

### YouTube Channels

- [IAmTimCorey](https://www.youtube.com/user/IAmTimCorey) 
- [Programming with Mosh](https://www.youtube.com/user/programmingwithmosh) 
- [Nick Chapsas](https://www.youtube.com/channel/UCrkPsvLGln62OMZRO6K-llg) 
- [Milan Jovanovic](https://www.youtube.com/@MilanJovanovicTech) 
- [Zoran Horvat](https://www.youtube.com/@zoran-horvat) 
- [CodeOpinion](https://www.youtube.com/@CodeOpinion), by Derek Comartin
- freeCodeCamp
  - [C# Tutorial - Full Course for Beginners](https://www.youtube.com/watch?v=GhQdlIFylQ8) (3h)
  - [Advanced C# Programming Course](https://www.youtube.com/watch?v=YT8s-90oDC0) (15h)
- [Raw Coding](https://www.youtube.com/@RawCoding)
- [Gui Ferreira](https://www.youtube.com/@gui.ferreira)

### Blogs

- Official [.NET Blog](https://devblogs.microsoft.com/dotnet/)
- [The Morning Dew](https://www.alvinashcraft.com/), aggregator of different info about .NET world, by Alvin Ashcraft.
- [You’ve Been Haacked](https://haacked.com/), by Phil Haack.
- [Eric Lippert's blog](https://ericlippert.com/), who worked on C# compiler team.
- [Steve Smith](https://ardalis.com/), who focuses on code quality and DDD.
- [Andrew Lock](https://andrewlock.net/), Senior Engineer at Datadog
- [Scott Hanselman](https://www.hanselman.com/blog/), Partner Program Manager at Microsoft
- [Rick Strahl's Web Log](https://weblog.west-wind.com/), focus on web and desktop apps in .NET.
- [Adam Sitnik](https://adamsitnik.com/), an expert on .NET Performance and Reliability.
- [Jimmy Bogard](https://www.jimmybogard.com/), creator of AutoMapper.
- [Vladimir Khorikov](https://enterprisecraftsmanship.com/), and expert in Testing.
- [Ayende @ Rahien](https://ayende.com/blog/), written by Oren Eini, creator of RavenDB.
- [Maarten Balliauw](https://blog.maartenballiauw.be/), Developer Advocate at JetBrains.
- [Khalid Abuhakmeh’s Blog](https://khalidabuhakmeh.com/), Developer Advocate at JetBrains.
- [Stephen Cleary](https://blog.stephencleary.com/), the author of "Concurrency in C# Cookbook"
- [Scott Brady](https://www.scottbrady91.com/articles), an expert on OAuth and web security.
- [Jiří Činčura](https://www.tabsoverspaces.com/), a project lead for ADO.NET provider for Firebird DB.
- [Coding Militia](https://blog.codingmilitia.com/), by João Antunes (Microsoft MVP).
- [Michael Shpilt](https://michaelscodingspot.com/), a software developer working at Microsoft
- [Mark Seemann](https://blog.ploeh.dk/), explains concepts that are not commonly blogged about with C#.
- [Steven Giesel](https://steven-giesel.com/), Microsoft MVP
- [Code Maze Weekly](https://code-maze.com/), articles on .NET, weekly.

### Podcasts

  - [.NET Rocks!](https://www.dotnetrocks.com/)
  - [Rockin' the Code World with Dot Net Dave](https://www.c-sharpcorner.com/live/rockin-the-code-world-with-dotnetdave)
  - [The Modern .NET Show](https://dotnetcore.show/)
    
### Other [.NET Content creators](https://www.wearedotnet.io/)

## Tools

- [Git](https://github.com/git-guides/install-git) and some [GUI clients](https://www.hostinger.com/tutorials/best-git-gui-clients/) - Distributed source control system.
- [Visual Studio 2026](https://visualstudio.microsoft.com/) - Main IDE for .NET projects.
- [Visual Studio Code](https://code.visualstudio.com/) - Lightweight code editor for different tech stacks, including .NET.
- [Rider](https://www.jetbrains.com/rider/) - Cross-Platform .NET IDE from JetBrains.
- [SQL Server Management Studio](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms) / [MSSQL extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-mssql.mssql) - tools for managing SQL Server and Azure SQL (Azure Data Studio was retired in February 2026).
- [LINQPad](https://www.linqpad.net/) - interactively query databases with LINQ.
- [ReSharper](https://www.jetbrains.com/resharper/) - rapid refactoring.
- [ILSpy](https://github.com/icsharpcode/ILSpy) / [dotPeek](https://www.jetbrains.com/decompiler/) / [.NET Reflector](https://www.red-gate.com/products/reflector/) - .NET decompilers.
- [Postman](https://www.postman.com/), [Bruno](https://www.usebruno.com/), or [.http files](https://learn.microsoft.com/en-us/aspnet/core/test/http-files) - tools for testing APIs.
- [NDepend](https://www.ndepend.com/) - static code analyzer.
- [NCrunch for Visual Studio](https://www.ncrunch.net/) - enables developers to run tests in the background as they write code.

## Wrap Up

If you think the roadmap can be improved, please open a PR with any updates and submit any issues. Also, I will continue to improve this, so you should star this repository, too.

## Contribution

- Open a pull request with improvements
- Discuss ideas in issues
- Spread the word

## License

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Author

[Dr. Milan Milanović](https://milan.milanovic.org) -  CTO at [3MD](https://3mdinc.com) and Microsoft MVP for Developer Technologies.
