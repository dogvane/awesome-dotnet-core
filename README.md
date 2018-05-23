# Awesome .NET Core [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A collection of awesome [.NET Core](#frameworks-libraries-and-tools) frameworks, libraries, tools, resources and software.

Inspired by [awesome](https://github.com/sindresorhus/awesome), [awesome-dotnet](https://github.com/quozd/awesome-dotnet),  [awesome-nodejs](https://github.com/sindresorhus/awesome-nodejs), [frontend-dev-bookmarks](https://github.com/dypsilon/frontend-dev-bookmarks).

Contributions are always welcome! Please take a look at the [contribution guidelines](https://github.com/thangchung/awesome-dotnet-core/blob/master/contributing.md) pages first. We accept proprietary and commercial software too.

Thanks to all [contributors](https://github.com/thangchung/awesome-dotnet-core/graphs/contributors), you're awesome and wouldn't be possible without you! The goal is to build a categorized community-driven collection of very well-known resources.

## Contents

* [General](#general)
* [框架，类库与工具](#框架，类库与工具)
  * [API](#api)
  * [应用程序框架](#应用程序框架)
  * [Application Templates](#application-templates)
  * [认证和授权](#authentication-and-authorization)
  * [区块链](#区块链)
  * [机器人](#bot)
  * [Build Automation](#build-automation)
  * [Bundling and Minification](#bundling-and-minification)
  * [Caching](#caching)
  * [CMS](#cms)
  * [Code Analysis and Metrics](#code-analysis-and-metrics)  
  * [Compression](#compression)
  * [Compilers, Transpilers and Languages](#compilers-transpilers-and-languages)
  * [Cryptography](#cryptography)
  * [Database](#database)
  * [Database Drivers](#database-drivers)
  * [Database Tools and Utilities](#database-tools-and-utilities)
  * [Date and Time](#date-and-time)
  * [Distributed Computing](#distributed-computing)
  * [E-Commerce and Payments](#e-commerce-and-payments)
  * [Exceptions](#exceptions)
  * [Functional Programming](#functional-programming)
  * [Graphics](#graphics)
  * [GUI](#gui)
  * [IDE](#ide)
  * [Internationalization](#internationalization)
  * [IOC](#ioc)
  * [Logging](#logging)
  * [Machine Learning and Data Science](#machine-learning-and-data-science)
  * [Mail](#mail)
  * [Mathematics](#mathematics)
  * [Networking](#networking)
  * [Misc](#misc)
  * [ORM](#orm)
  * [Profiling](#profiling)
  * [Queue and Messaging](#queue-and-messaging)
  * [Query Builders](#query-builders)
  * [Scheduler and Job](#scheduler-and-job)
  * [SDKs](#sdks)
  * [Security](#security)
  * [Searching](#searching)
  * [Serialization](#serialization)
  * [Template Engine](#template-engine)
  * [Testing](#testing)
  * [Tools](#tools)
  * [Web Framework](#web-framework)
  * [Web Socket](#web-socket)
  * [Windows Service](#windows-service)
  * [Workflow](#workflow)
* [Starter Kits](#starter-kits)
* [Sample Projects](#sample-projects)
* [Articles](#articles)
* [Books](#books)
* [Videos](#videos)
* [Podcasts](#podcasts)
* [Community](#community)

## 通用

* [ASP.NET Core Documentation](https://docs.asp.net/en/latest/) - 这个是 ASP.NET Core 官方文档的网站。
* [.NET Core Documentation](https://docs.microsoft.com/en-us/dotnet/articles/welcome) - .net Core 官方入门文档，和例子。包含c# F# VB。
* [.NET Core SDK](https://www.microsoft.com/net/core) - .NET Core SDK 的说明以及开源社区  [GitHub](https://github.com/dotnet/core).
* [.NET Platform Standard](https://github.com/dotnet/corefx/blob/master/Documentation/architecture/net-platform-standard.md) - .NET 跨平台标准的说明以及版本之间的差别。
* [Introducing .NET Standard 2.0](https://blogs.msdn.microsoft.com/dotnet/2016/09/26/introducing-net-standard) - .NET 标准 2.0 的介绍

## 框架，类库与工具

### API
* [autorest](https://github.com/Azure/autorest) - 一个生成OpenAPI访问客户端的工具（本体使用nodejs来运行）。输出格式包含C#, Java, Node.js, TypeScript, Python， Ruby.
* [aspnet-api-versioning](https://github.com/Microsoft/aspnet-api-versioning) - 给 ASP.NET Web API, OData with ASP.NET Web API, ASP.NET Core，写的REST API接口增加版本控制。（简化 http://api.xxx.com/v1.0，http://api.xxx.com/v2.0 这样的API格式的实现）
* [AspNetCoreRateLimit](https://github.com/stefanprodan/AspNetCoreRateLimit) - 一个针对 ASP.NET Core 访问控制的中间件。可以对IP或者客户端ID增加每秒，每分钟或者每小时访问次数的限制。
* [CondenserDotNet](https://github.com/Drawaes/CondenserDotNet) - 使用Kestrel和Consul构建的轻量级微服务框架。（文档不多，start也少，国内和国外基本没相关介绍，建议养肥了再关注吧）
* [Flurl](https://github.com/tmenier/Flurl) - 以 Fluent 方式构建 URL 并进行HTTP请求测试。[http://tmenier.github.io/Flurl](http://tmenier.github.io/Flurl).
* GraphQL - （GraphQL 是一个用于 API 的查询语言，是一个使用基于类型系统来执行查询的服务端运行时（类型系统由你的数据定义）。GraphQL 并没有和任何特定数据库或者存储引擎绑定，而是依靠你现有的代码和数据支撑。以上来自：[http://graphql.cn/](http://graphql.cn/learn/)）
  * [graphql-aspnetcore](https://github.com/JuergenGutsch/graphql-aspnetcore) - GraphQL在 ASP.NET Core 的中间件。（start:69 @ 2018/5/9）
  * [graphql-convention](https://github.com/graphql-dotnet/conventions) - 一个类库可以根据对象的属性及方法定义自动生成 GraphQL 的 Schema。
  * [graphiql-dotnet](https://github.com/JosephWoodward/graphiql-dotnet) - GraphiQL在 ASP.NET Core 下的中间件（start:63 @ 2018/5/9）
  * [graphql-dotnetcore](https://github.com/mkmarek/graphql-dotnetcore) - GraphiQL在 ASP.NET Core 下的中间件，基于[https://github.com/graphql/graphql-js](https://github.com/graphql/graphql-js).（start:80 @ 2018/5/9） 
  * [graphql-dotnet](https://github.com/graphql-dotnet/graphql-dotnet) - GraphiQL在 .Net 下的实现。（start:1957 @2018/5/9) 这个项目是.Net下的项目，暂时不支持.net core，但可以用Mono在Linux下运行。独立运行不依赖web服务器。
  * [FSharp.Data.GraphQL](https://github.com/fsprojects/FSharp.Data.GraphQL) - GraphQL在F#下的实现 [https://fsprojects.github.io/FSharp.Data.GraphQL](https://fsprojects.github.io/FSharp.Data.GraphQL).
  * [parser](https://github.com/graphql-dotnet/parser) - .net下为GraphQL提供的词法分析与解析器。
* [halcyon](https://github.com/visualeyes/halcyon) - halcyon 是 HAL(Hypertext Application Language) 在 asp.net 下的实现，支持 asp.net 和 asp.net core。HAL是一种简单的数据格式，它能以一种简单、统一的形式，在API中引入超链接特性，使得API的可发现性（discoverable）更强，并具有自描述的特点。更详细的介绍常见[度娘](https://www.baidu.com/s?wd=HAL%20json)
* [JSON API .NET Core](https://github.com/Research-Institute/json-api-dotnet-core) - 用来构建一个兼容[json:api](http://jsonapi.org/)样式的webapi框架。它有点类似HAL。
* [LightNode](https://github.com/neuecc/LightNode) - 一个实现[OWIN](https://www.baidu.com/s?wd=OWIN)的微型 RPC/REST 框架。[http://neuecc.github.io/LightNode](http://neuecc.github.io/LightNode).
* [NetCoreStack.Proxy](https://github.com/NetCoreStack/Proxy) - 一个类型安全的，用.NET Standard 2.0标准实现的REST代理库。
* [NSwag](https://github.com/NSwag/NSwag) - NSwag 是 Swagger/OpenAPIThe 在.Net，Web API, TypeScript 下的工具链。详细内容访问：[http://NSwag.org](http://NSwag.org).工具链简单说就是提供了一个[NSwagStudio](https://github.com/NSwag/NSwag/wiki/NSwagStudio)，或者的[命令行工具](https://github.com/RSuter/NSwag/wiki/CommandLine)，甚至直接引用相关的代码生成OpenAPI的客户端访问代理类，输出类型包括c#,TypeScrip(包含但不仅限于：jQuery, AngularJS, Angular 2+, Aurelia, KnockoutJS )
* [OData](https://github.com/OData/WebApi/tree/feature/netcore) - [OData](https://www.baidu.com/s?wd=odata) = Open Data Protocol（是一个设计和使用RESTful API的标准）。OData项目就是帮你在 .net 和 .net core 下帮你实现这套标准的库。
* [refit](https://github.com/paulcbetts/refit) - 帮你自动构建一个访问 REST 的类库，支持.NET全版本和Xamarin。[http://paulcbetts.github.io/refit/](http://paulcbetts.github.io/refit/).（这个和上面的NSwag实现的功能类似，但是它更灵活一些，访问的代理类不会像代码生成那样，根据接口的名称和产生的名称生成固定的代理类。而是可以按照自己的医院写一个接口，然后用标签（Attribute)的方式在的方法上注明要访问REST下的那个API）
* [RESTClient .NET](https://bitbucket.org/MelbourneDeveloper/restclient-.net) - 一个简单的 REST 客户端，支持所有.NET平台
* [RestEase](https://github.com/canton7/RestEase) - 一个简单易用的 REST API 客户端，从[refit](https://github.com/paulcbetts/refit)改造过来的版本。（start有300多个，refit有2500个@2018/5/20，但首页的文档详细程度比refit要多很多，可以做入门介绍。）
* [RestLess](https://github.com/letsar/RestLess) - 也是一个 REST API 客户端，作者灵感来自于[refit](https://github.com/paulcbetts/refit)，介绍里重点介绍了和refit的性能比较，简单说就是比refit快了一倍（在安卓端测试）。
* [Swashbuckle](https://github.com/domaindrivendev/Swashbuckle.AspNetCore) - 我觉得不需要介绍了，每次写web api需要配置swagger是都会用，重点是，谁还能再把对它的配置再简化一下。
* [WebAPIContrib for ASP.NET CORE](https://github.com/WebApiContrib/WebAPIContrib.Core) - 对于asp.net和asp.net core下的web api项目的一些社区代码做收集，形成的一个辅助性质的类库。.net版和.net core版的实现的功能模块还不完全一样。但都实现了帮助你的web api 以 Bson,CSV,PlainText,Jsopn,MessagePack,Protobuf,Yaml，这几种协议进行返回。

### 应用程序框架
* [ABP](https://github.com/aspnetboilerplate/aspnetboilerplate) - 一个基于asp.net的应用程序框架，.net圈里应该都听过的，没听过可以上[cnblogs.com](http://zzk.cnblogs.com/s?t=b&w=abp)看看相关介绍。简单说，当你新开一个要比简单的三层架构要复杂很多的项目时，建议看看它，首次使用可以直接按照框架来，熟悉之后再按照实际项目情况进行优化和改进。
* [Aeron.NET](https://github.com/AdaptiveConsulting/Aeron.NET) - 一个实现了高效可靠的UDP单播，组播和IPC消息协议的组件库。它是[Aeron](https://github.com/real-logic/Aeron)在.NET下的实现。Aeron则是java和c++下UDP组件库。简单说你可以在.NET下发UDP，java项目下收到对应消息，中间的消息传递都是安全可靠和高效的。
* [akka.net](https://github.com/akkadotnet/akka.net) - 一个用于编写高并发，容错的基于事件驱动的分布式系统的应用程序框架。更详细的介绍看[百度 akka.net](https://www.baidu.com/s?wd=akka.net)。类似的流行的还有[orleans](https://github.com/dotnet/orleans)
* [ASP.NET MVC](https://github.com/aspnet/Mvc) - 需要介绍吗，不需要了吧。
* [CQRSlite](https://github.com/gautema/CQRSlite) - 一个轻量级的框架帮你去写 CQRS/ES 模型的应用程序。（@star:540）[不清楚问度娘](https://www.baidu.com/s?&wd=CQRS%2FES)。国内也有人做了一套类似的框架[ENode](https://github.com/tangxuehua/enode)，因为不是英文的，老外没收录而已。
* [ENode](https://github.com/tangxuehua/enode) - ENode is a framework aims to help us developing ddd, cqrs, eda, and event sourcing style applications.（@star:1100）
* [DotNetty](https://github.com/Azure/DotNetty) - 事件驱动的异步网络框架，源自java的[netty](https://github.com/netty/netty)，微软的[Azure团队](https://github.com/Azure)负责维护。使用方法问[度娘](https://www.baidu.com/s?wd=DotNetty)
* [EmbedIO](https://github.com/unosquare/embedio) - 一个超小的可跨平台的基于模块的Web服务器组件。(@star:417)通常是给你写的应用里集成了一个web服务器，当你部署到服务器后，偷偷的给自己开了一个后门端口，然后通过这个端口以web方式进行服务器管理。（以上说辞是根据官方文档里介绍整理出来的）
* [EventFlow](https://github.com/eventflow/EventFlow) - 用 Async/await 写的 CQRS/ES,DDD 框架（@star:640）。
* [ExtCore](https://github.com/ExtCore) - 一个基于asp.net core 的基于模块化可扩展的web应用框架。
* [Halibut](https://github.com/OctopusDeploy/Halibut) - .NET下的使用SSL做JSON-RPC的安全通讯组件。它是 [Octopus Deploy](https://octopus.com/) 持续集成部署系统的后台通讯组件。它除了普通的request/response这种应答响应方式外，还提供了polling（轮询）模式。简单说，传统的应用服务器是客户端发起tcp连接请求到服务器端，而halibut可以反过来操作，就是由服务端反过来连接到事实上的客户端。这也就是这套持续集成系统要叫做Octopus(章鱼)的原因。
* [grpc](https://github.com/grpc/grpc/tree/master/src/csharp) - [gRPC](https://github.com/grpc/grpc)在.net下的实现。gPRC的概念问[度娘](https://www.baidu.com/s?wd=gRPC)
* [MassTransit](https://github.com/MassTransit/MassTransit) - 基于消息，松耦合，异步通讯来获得高可用，高可靠与可扩展的分布式框架。（@star:1500）国内还是有一些人在研究的，可以问[度娘](https://www.baidu.com/s?wd=MassTransit)了解。
* [microdot](https://github.com/gigya/microdot) - 一个微服务框架，国内研究的人还不多(@star:600)
* [Nancy](https://github.com/NancyFx/Nancy) - 一个轻量级的web服务器框架。（@star:6112）看到这么多是star，老牌项目大家可以放心食用。
* [orleans](https://github.com/dotnet/orleans) - 微软出的分布式框架，不过多介绍了，大家自行[百度 Orleans](https://www.baidu.com/s?wd=Orleans)
* [protoactor-dotnet](https://github.com/AsynkronIT/protoactor-dotnet) -  也是一个基于 Actor 模式的分布式框架。[http://proto.actor](http://proto.actor).看作者的项目列表，有 go .net kotlin python 的实现。go的star最高(@star:2168)，其次是.net(@star:619)，kotlin(@star:105)和python(@star:43)应该是才开始进行开发，所以关注的人还不多。
* [RService.io](https://github.com/Stoom/RService.IO) - 一个轻量级的REST微服务框架，关注的人不多(@star:34)，而且也断更了，不用太关注他了。
* [ServiceStack](https://github.com/ServiceStack/ServiceStack) - 一个适用所有人的简单快速的结构设计良好的web服务框架。 [https://servicestack.net](https://servicestack.net).(@star:4229) 认识它是当年有人在群里问 ServiceStack.Redis 4.0 组件如何破解。不知道那位仁兄现在是否已经解决了这个问题。
* [Steeltoe OSS](https://github.com/SteelToeOSS) - 基于云服务的微服务工具包。国内的用户就不用关注了。

### Application Templates
* [ASP.NET Core Boilerplate](https://github.com/ASP-NET-Core-Boilerplate/Templates) - 一个专业的ASP.NET MVC模板，用于构建安全、快速、健壮和可适应的Web应用程序或站点。它提供了在微软提供的默认MVC模板之上所需的最小代码量。你可以通过 `dotnet new --install "Boxed.Templates::*"` 将模板加入系统，然后用 `dotnet new api` 的方式进行初始化。可以 `dotnet new api --help` 了解在初始化时，能配置那些参数。(@star:1240)
* [ASP.NET-MVC-Template](https://github.com/NikolayIT/ASP.NET-MVC-Template) - 一个开箱即用的asp.net mvc模板，有mvc5, .net core, .net core with Angular 三个。俄语好的可以看的[教学视频](https://www.youtube.com/watch?v=xhoBt9MscrY)。(@star:154)
* [AddFeatureFolders](https://github.com/OdeToCode/AddFeatureFolders) - 大家自己去看吧，我没看懂是怎么用的。Enable feature folders for MVC controllers and views in ASP.NET Core.
* [Angular Visual Studio Webpack Starter](https://github.com/damienbod/AngularWebpackVisualStudio) - 一个集成了asp.net core Angular Webpack Visual Studio的模板。它的好处是让你的前端代码与asp.net core代码在一起，发布的时候就更方便一些。
* [JavaScriptServices](https://github.com/aspnet/JavaScriptServices) - 微软出的一个能够让你在asp.net core里调用nodejs服务。[度娘](https://www.baidu.com/s?ie=UTF-8&wd=JavaScriptServices)里的介绍比较少，如果实在需要互相调用，可以问谷沟。
* [kendo-ui-core](https://github.com/telerik/kendo-ui-core) - 一个基于JQuery，HTML5构建web apps的模板。[http://www.telerik.com/kendo-ui](http://www.telerik.com/kendo-ui).(@star:1945)
* [QuickApp](https://github.com/emonney/QuickApp) - 一个基于 Angular5 ASP.NET Core Bootstrap4 的项目模板，并集成了用户，登录(IdentityServer4)，角色管理等模块。
* [Scaffolder](https://github.com/dncuug/scaffolder) - 这是一个数据库的脚手架工具，会根据数据库表的结构生成对应的管理界面，可以查看和修改数据库里的数据。适合拿来做简单的后台管理工具，不过作者是俄国人，blog也是俄文，看不懂啊。(@star:96)
* [Serenity](https://github.com/volkanceylan/Serenity) - 也是一个可以方便构造后台管理界面的应用程序模板。大家可以适度关注一下。（@star:1400）
* [Toucan](https://github.com/mrellipse/toucan) - 一个构建SPA（单页面）模板，服务端用 .net core，按照SOLID的设计原则来开发，客户端用TypeScript 2, Vuejs 2, Vuex2.(@star:125) 项目创建时间比较晚，所以star不高，但它的客户端用vuejs，国内的开发可以适度关注一下，毕竟vuejs比angular,reactjs要简单一些。

### Authentication and Authorization
* [AspNet.Security.OpenIdConnect.Server](https://github.com/aspnet-contrib/AspNet.Security.OpenIdConnect.Server) - OpenID Connect/OAuth2 的服务器框架。(@star:394)
* [Auth0](https://github.com/auth0/auth0.net) - Auth0 的客户端 api
* [Identity](https://github.com/aspnet/Identity) - 微软 asp.net 出的身份验证，登录以及授权系统。
* [IdentityServer](https://github.com/IdentityServer/IdentityServer4) - 微软身份验证，授权系统的服务端。
  * [IdentityServer4.EntityFramework](https://github.com/IdentityServer/IdentityServer4.EntityFramework) - EntityFramework persistence layer
  * [IdentityServer4.MongoDB](https://github.com/diogodamiani/IdentityServer4.MongoDB) - MongoDB persistence layer
  * [IdentityServer4.EntityFrameworkCore](https://github.com/2020IP/TwentyTwenty.IdentityServer4.EntityFrameworkCore) - Entity Framework Core persistence layer
  * [IdentityServer4.Templates](https://github.com/IdentityServer/IdentityServer4.Templates) - dotnet cli templates for IdentityServer4.
* [openiddict](https://github.com/openiddict/openiddict-core) - ASP.NET Core 下的OpenID连接服务器，简单易用.(@star:640)，看文档不是很复杂
* [stormpath-sdk](https://github.com/stormpath/stormpath-sdk-dotnet) - Build [simple, secure web applications](https://github.com/stormpath/stormpath-aspnetcore) with Stormpath and ASP.NET Core. Stormpath是一个云端的认证服务器，貌似收费的，这个是.net下的客户端sdk。
* [stuntman](https://github.com/ritterim/stuntman) - 一个能在开发阶段，帮你模拟不同登录用户的库。

### 区块链
* [NBitcoin](https://github.com/MetacoSA/NBitcoin) - 比特币在.net下的库。
* [NEO](https://github.com/neo-project/neo) - 一种智能经济分布式网络，国内发布的，小蚁区块链负责维护。
* [Nethereum](https://github.com/Nethereum) - .net 下接入以太坊的组件。
* [StratisBitcoinFullNode](https://github.com/stratisproject/StratisBitcoinFullNode) - 貌似是一个比特币在.net下的实现。

### Bot
* [NadekoBot](https://github.com/Kwoth/NadekoBot) - c#写的聊天机器人。

### Build Automation
* [cake-build](https://github.com/cake-build/cake) - 跨平台的自动化构建系统 [http://cakebuild.net](http://cakebuild.net).
* [CatLight](https://catlight.io) - 用来监控项目编译和任务并将状态通知给开发。不过收费的，国内的用户不用玩了。
* [Colorful.Console](https://github.com/tomakita/Colorful.Console) - 定制化控制台的样式输出。简单说就是让你的 Console.Write 输出的内容立马高大上起来。具体效果上他们的官网看[http://colorfulconsole.com](http://colorfulconsole.com).
* [dotnet-docker](https://github.com/dotnet/dotnet-docker) - The base Docker images for working with .NET Core and the .NET Core Tools.
* [GitInfo](https://github.com/kzu/GitInfo) - 可以在MSBuild编译的时候，把Git的版本信息写入你的dll文件里，你就可以已git的信息做为你的版本号来用。
* [GitVersioning](https://github.com/AArnott/Nerdbank.GitVersioning) - 也是把git信息写入你编译时的DLL。
* [go-dotnet](https://github.com/matiasinsaurralde/go-dotnet) - 让你的.net可以被go调用。
* [Image2Docker](https://github.com/docker/communitytools-image2docker-win) - PowerShell module which ports existing Windows application workloads to Docker.
* [msbuild](https://github.com/Microsoft/msbuild) - The Microsoft Build Engine is a platform for building applications.
* [Nuke](https://github.com/nuke-build/nuke) - Cross-platform build automation system.
* [Opserver](https://github.com/opserver/Opserver) - Stack Exchange's 开源的监控系统。如果没有太复杂的监控要求，直接按照到服务器后，配置一些监控的配置信息就可以使用了。
* [vsts-agent](https://github.com/Microsoft/vsts-agent) - Visual Studio Team Services Build and Release Agent.

### Bundling and Minification
* [BundlerMinifier](https://github.com/madskristensen/BundlerMinifier) - Visual Studio extension that let's you configure bundling and minification of JS, CSS and HTML files.
* [JavaScriptViewEngine](https://github.com/pauldotknopf/JavaScriptViewEngine) - ASP.NET MVC ViewEngine for rendering markup in a JavaScript environment. Ideal for React and Angular server-side rendering.
* [Smidge](https://github.com/Shazwazza/Smidge/) - Lightweight runtime CSS/JavaScript file minification, combination, compression & management library for ASP.NET Core.
* [Web Markup Minifier](https://github.com/Taritsyn/WebMarkupMin) - .NET library that contains a set of markup minifiers. The objective of this project is to improve the performance of web applications by reducing the size of HTML, XHTML and XML code.

### Caching
* [CacheManager](https://github.com/MichaCo/CacheManager) - Open source caching abstraction layer for .NET written in C#. It supports various cache providers and implements many advanced features. [http://cachemanager.michaco.net](http://cachemanager.michaco.net)
* [Foundatio](https://github.com/exceptionless/Foundatio) - Pluggable foundation blocks for building distributed apps.
* [Microsoft Caching](https://github.com/aspnet/Caching) - Libraries for in-memory caching and distributed caching.
* [Stack Exchange Redis](https://github.com/StackExchange/StackExchange.Redis) - High performance general purpose redis client for .NET languages (C# etc).

### CMS
* [Blogifier.Core](https://github.com/blogifierdotnet/Blogifier.Core) - ASP.NET applications to provide common blogging functionality.
* [Cofoundry](https://github.com/cofoundry-cms/cofoundry) - Open source .NET Core CMS and modular application framework. Code-first, unobtrusive and extensible.
* [Lynicon](https://github.com/jamesej/lyniconanc) - O/S ASP.Net Core/.Net Core CMS with paid for modules: JSON content, works with variety of data stores, c# content types
* [Orchard Core CMS](https://github.com/OrchardCMS/OrchardCore) - Open Source Content Management System built with ASP.NET Core on top of a Modular and Extensible Application Framework.
* [NetCoreCMS](https://github.com/OnnoRokomSoftware/NetCoreCMS) - An Open source ASP.NET Core 2.0 CMS. It currently supports MySQL and planned to implement MSSQL, SQLite and PostgreSQL. Also it is a modular CMS supports theme, skin, custom layout, widgets, multiple language (En, BN).
* [Platformus](https://github.com/Platformus) - Free, open source and cross-platform CMS based on ASP.NET Core 1.0 and ExtCore framework.
* [SimpleContent](https://github.com/joeaudette/cloudscribe.SimpleContent) - Simple, yet flexible content and blog engine for ASP.NET Core that can work with or without a database.
* [Squidex](https://github.com/Squidex/squidex) - Headless CMS, based on MongoDB, CQRS and Event Sourcing.
* [Weapsy](https://github.com/Weapsy/Weapsy) - Open source ASP.NET Core CMS based on DDD and CQRS. It supports MSSQL, MySQL, SQLite and PostgreSQL out of the box.
* [Wyam](https://github.com/Wyamio/Wyam) - Modular static content and static site generator.

### Code Analysis and Metrics
* [awesome-static-analysis](https://github.com/mre/awesome-static-analysis) - Curated list of static analysis tools, linters and code quality checkers for various programming languages.
* Code Analysis
  * [DevSkim](https://github.com/Microsoft/DevSkim) - A set of IDE plugins and rules that provide security "linting" capabilities.
  * [RefactoringEssentials](https://github.com/icsharpcode/RefactoringEssentials) - Refactoring Essentials for Visual Studio.
  * [roslyn-analyzers](https://github.com/dotnet/roslyn-analyzers) - .NET Compiler Platform ("Roslyn") Analyzers.
  * [StyleCopAnalyzers](https://github.com/DotNetAnalyzers/StyleCopAnalyzers) - StyleCop rules using the .NET Compiler Platform.
* Metrics
  * [AppMetrics](https://github.com/alhardy/AppMetrics) - App Metrics is an open-source and cross-platform .NET library used to record and report metrics within an application and reports it's health.
  * [Audit.NET](https://github.com/thepirat000/Audit.NET) - Small framework to audit .NET object changes.
  * [BenchmarkDotNet](https://github.com/PerfDotNet/BenchmarkDotNet) - Powerful .NET library for benchmarking.
  * [coverlet](https://github.com/tonerdo/coverlet) - Cross platform code coverage library for .NET Core.
  * [Foundatio](https://github.com/exceptionless/Foundatio#metrics) - A common interface with in memory, redis, StatsD, and Metrics.NET implementations.
  * [MiniCover](https://github.com/lucaslorentz/minicover) - Minimalist Code Coverage Tool for .NET Core.
  * [NBench](https://github.com/petabridge/NBench) - Performance benchmarking and testing framework for .NET applications.
  * [Nexogen.Libraries.Metrics](https://github.com/nexogen-international/Nexogen.Libraries.Metrics) - Library for collecting application metrics in .NET and exporting them to Prometheus.
  * [OpenCover](https://github.com/OpenCover/opencover) - Code coverage tool for .NET 2 and above (WINDOWS OS only), support for 32 and 64 processes with both branch and sequence points.
  * [prometheus-net](https://github.com/prometheus-net/prometheus-net) - .NET Client for [https://prometheus.io](https://prometheus.io).

### Compression
* [lz4net](https://github.com/MiloszKrajewski/lz4net) - 一个支持.net全平台的超级快的压缩算法LZ4。看介绍，可以单核400M/s压缩，2G/s解压，基本上达到内存的访问极限，压缩比比gzip要差一些。关于不同压缩算法的效率可以看[Quick Benchmark: Gzip vs Bzip2 vs LZMA vs XZ vs LZ4 vs LZO](https://blog.csdn.net/leilonghao/article/details/73200859)。
* [sharpcompress](https://github.com/adamhathcock/sharpcompress) - 一个完全用托管代码写的压缩组件，支持zip/tar/bzip2/gizp。

### Compilers, Transpilers and Languages
* [Fable](https://github.com/fable-compiler/Fable) - F# to JavaScript Compiler.
* [fparsec](https://github.com/stephan-tolksdorf/fparsec) - A parser combinatory library for F# and C#.
* [roslyn](https://github.com/dotnet/roslyn) - The .NET Compiler Platform ("Roslyn") provides open-source C# and Visual Basic compilers with rich code analysis APIs.
* [Pidgin](https://github.com/benjamin-hodgson/Pidgin) - A lightweight, fast and flexible parsing library for C#, developed at Stack Overflow.
* [Sprache](https://github.com/sprache/Sprache) - Tiny C# Monadic Parser Framework.

### Cryptography
* [BCrypt.Net](https://github.com/BcryptNet/bcrypt.net) - Bringing updates to the original bcrypt package
* [BCrypt.NET-Core](https://github.com/neoKushan/BCrypt.Net-Core) - .NET Core port of BCrypt.NET used to store passwords securely.
* [BouncyCastle PCL](https://github.com/onovotny/BouncyCastle-PCL) - The Bouncy Castle Crypto package is a C# implementation of cryptographic algorithms and protocols.

### Database
* [DBreeze](https://github.com/hhblaze/DBreeze) - C# .NET MONO NOSQL (key value store embedded) ACID multi-paradigm database management system.
* [JsonFlatFileDataStore](https://github.com/ttu/json-flatfile-datastore) - Simple JSON flat file data store with support for typed and dynamic data.
* [LiteDB](https://github.com/mbdavid/LiteDB) - .NET NoSQL Document Store in a single data file - [http://www.litedb.org](http://www.litedb.org).
* [NoDb](https://github.com/joeaudette/NoDb) - "no database" file system storage for .NET Core/ASP.NET Core because not every project needs a database.
* [marten](https://github.com/JasperFx/marten) - Postgresql as a Document Database and Event Store for .NET Applications [http://jasperfx.github.io/marten](http://jasperfx.github.io/marten).
* [yessql](https://github.com/sebastienros/yessql) - .NET document database working on any RDBMS.

### Database Drivers
* [cassandra-csharp-driver](https://github.com/datastax/csharp-driver) - DataStax C# Driver for Apache Cassandra.
* [confluent-kafka-dotnet](https://github.com/confluentinc/confluent-kafka-dotnet) - Confluent's Apache Kafka .NET client.
* [couchbase-lite-net](https://github.com/couchbase/couchbase-lite-net) - A lightweight, document-oriented (NoSQL), syncable database engine for .NET.
* [MongoDB.Driver](https://github.com/mongodb/mongo-csharp-driver) - .NET Driver for MongoDB.
* MySQL
  * [mysql-connector-net](https://github.com/mysql/mysql-connector-net/tree/8.0) - Connector/Net is a fully-managed ADO.NET driver for MySQL.
  * [MySqlConnector](https://github.com/mysql-net/MySqlConnector) - Async MySQL Connector for .NET and .NET Core.
* Neo4j
  * [neo4j-dotnet-driver](https://github.com/neo4j/neo4j-dotnet-driver) - Neo4j Bolt driver for .NET.
  * [Neo4jClient](https://github.com/Readify/Neo4jClient) - .NET client binding for Neo4j.
* [npgsql](https://github.com/npgsql/npgsql) - .NET data provider for PostgreSQL. It allows any program developed for .NET framework to access a PostgreSQL database server. It is implemented in 100% C# code. PostgreSQL versions since 9.1 are officially supported, others may work. [http://www.npgsql.org](http://www.npgsql.org)
* [ravendb](https://github.com/ayende/ravendb/tree/v4.0) - Linq enabled document database for .NET.
* [RethinkDb.Driver](https://github.com/bchavez/RethinkDb.Driver) - C#/.NET RethinkDB driver with 100% ReQL API coverage.
* [progaudi.tarantool](https://github.com/progaudi/progaudi.tarantool) - .NET client for Tarantool NoSql database.

### Database Tools and Utilities
* [DbUp](https://github.com/DbUp/DbUp) - .NET library that helps you to deploy changes to SQL Server databases. It tracks which SQL scripts have been run already, and runs the change scripts that are needed to get your database up to date.
* [NReco.PivotData](https://www.nuget.org/packages/NReco.PivotData) - In-memory data cube with OLAP operations and PivotTable data model.

### Date and Time
* [Exceptionless.DateTimeExtensions](https://github.com/exceptionless/Exceptionless.DateTimeExtensions) - DateTimeRange, Business Day and various DateTime, DateTimeOffset, TimeSpan extension methods.
* [FluentDateTime](https://github.com/FluentDateTime/FluentDateTime) - Allows you to write cleaner DateTime expressions and operation. Partially inspired by Ruby DateTime Extensions.
* [nodatime](https://github.com/nodatime/nodatime) - Better date and time API for .NET [http://nodatime.org](http://nodatime.org).

### Distributed Computing
* [aspnetcore-health](https://github.com/lurumad/aspnetcore-health) - Enables load balancers to monitor the status of deployed Web applications.
* [Foundatio](https://github.com/exceptionless/Foundatio) - Pluggable foundation blocks for building distributed apps.
* [Obvs](https://github.com/christopherread/Obvs) - An observable microservice bus .NET library that wraps the underlying transport in simple Rx based interfaces.
* [Ocelot](https://github.com/TomPallister/Ocelot) - API Gateway created using .NET Core.
* [OpenTracing](https://github.com/opentracing/opentracing-csharp) - Vendor-neutral APIs and instrumentation for distributed tracing.
* [Polly](https://github.com/App-vNext/Polly) - .NET 3.5 / 4.0 / 4.5 / PCL library that allows developers to express transient exception and fault handling policies such as Retry, Retry Forever, Wait and Retry or Circuit Breaker in a fluent manner.

### E-Commerce and Payments
* [SimplCommerce](https://github.com/simplcommerce/SimplCommerce) - Super simple ecommerce system built on .NET Core.
* [Stripe](https://github.com/ServiceStack/Stripe) - Typed .NET clients for stripe.com REST APIs.

### Exceptions
* [Exceptionless](https://github.com/exceptionless/Exceptionless.Net) - Exceptionless .NET Client
* [GlobalExceptionHandlerDotNet](https://github.com/JosephWoodward/GlobalExceptionHandlerDotNet) - GlobalExceptionHandlerDotNet allows you to configure exception handling as a convention with your ASP.NET Core application pipeline as opposed to explicitly handling them within each controller action.

### Functional Programming
* [CSharpFunctionalExtensions](https://github.com/vkhorikov/CSharpFunctionalExtensions) - Functional Extensions for C#.
* [DynamicData](https://github.com/RolandPheasant/DynamicData) - Reactive collections based on Rx.NET.
* [echo-process](https://github.com/louthy/echo-process) - Actor library for C# with additional modules that support persistence to Redis, as well as JS integration.
* [FsCheck](https://github.com/fscheck/FsCheck) - Random Testing for .NET.
* [Giraffe](https://github.com/dustinmoris/Giraffe) - A native functional ASP.NET Core web framework for F# developers.
* [language-ext](https://github.com/louthy/language-ext) - C# functional language extensions and 'Erlang like' concurrency system.
* [LaYumba.Functional](https://github.com/la-yumba/functional-csharp-code) - Utility library for programming functionally in C#.
* [NetMQ.ReactiveExtensions](https://github.com/NetMQ/NetMQ.ReactiveExtensions) - Effortlessly send messages anywhere on the network using Reactive Extensions (RX). Transport protocol is ZeroMQ.
* [Optional](https://github.com/nlkl/Optional) - A robust option type for C#.
* [reactive-streams-dotnet](https://github.com/reactive-streams/reactive-streams-dotnet) - [Reactive Streams](http://www.reactive-streams.org/) for .NET.
* [ReactiveUI](https://github.com/reactiveui/ReactiveUI) - A MVVM framework that integrates with the Reactive Extensions for .NET to create elegant, testable User Interfaces that run on any mobile or desktop platform.
* [Rx.NET](https://github.com/Reactive-Extensions/Rx.NET) - The [Reactive Extensions](http://reactivex.io) for .NET.
* [Qactive](https://github.com/RxDave/Qactive) - Reactive queryable observable framework. `4.x.x or above`
* [sodium](https://github.com/SodiumFRP/sodium/tree/master/c%23) - Functional Reactive Programming (FRP) Library. `4.x.x or above`

### Graphics
* [GLFWDotNet](https://github.com/smack0007/GLFWDotNet) - .NET bindings for GLFW.
* [ImageProcessor](https://github.com/JimBobSquarePants/ImageProcessor) - A fluent wrapper around System.Drawing for the processing of image files [http://imageprocessor.org](http://imageprocessor.org). `4.5.x or above`
* [ImageSharp](https://github.com/SixLabors/ImageSharp) - Cross-platform library for processing of image files written in C#.
* [Magick.NET](https://github.com/dlemstra/Magick.NET) - The .NET library for ImageMagick.
* [QRCoder](https://github.com/codebude/QRCoder) - A pure C# Open Source QR Code implementation.
* [SharpBgfx](https://github.com/MikePopoloski/SharpBgfx) - C# bindings for the bgfx graphics library.
* [Structure.Sketching](https://github.com/JaCraig/Structure.Sketching) - Image processing library for use in .NET applications that supports .NET Core.
* [veldrid](https://github.com/mellinoe/veldrid) - A low-level, hardware-accelerated 3D graphics library for .NET.

### GUI
* [Avalonia](https://github.com/AvaloniaUI/Avalonia) - A multi-platform .NET UI framework (formerly known as Perspex).
* [AvaloniaEdit](https://github.com/AvaloniaUI/AvaloniaEdit/) - The Avalonia-based text editor component forked from [AvalonEdit](https://github.com/icsharpcode/AvalonEdit)
* [WinApi](https://github.com/prasannavl/WinApi) - A simple, direct, ultra-thin CLR library for high-performance Win32 Native Interop with automation, windowing, DirectX, OpenGL and Skia helpers.

### IDE
* [Mono](https://github.com/mono/monodevelop) - MonoDevelop enables developers to quickly write desktop and web applications on Linux, Windows and Mac OS X. It also makes it easy for developers to port .NET applications created with Visual Studio to Linux and Mac OS X maintaining a single code base for all platforms.
* [rider](https://www.jetbrains.com/rider/) - Cross-platform C# IDE based on the IntelliJ platform and ReSharper.
* [Omnisharp](http://www.omnisharp.net/) - Family of Open Source projects, each with one goal: To enable a great .NET experience in YOUR editor of choice.
* [SharpDevelop](https://github.com/icsharpcode/SharpDevelop) - SharpDevelop is a free Integrated Development Environment (IDE) for C#, VB.NET, Boo, IronPython, IronRuby and F# projects on Microsoft's .NET platform. It is written (almost) entirely in C#, and comes with features you would expect in an IDE plus a few more.
* [Visual Studio Code](https://github.com/Microsoft/vscode) - New type of tool that combines the simplicity of a code editor with what developers need for their core edit-build-debug cycle. Code provides comprehensive editing and debugging support, an extensibility model, and lightweight integration with existing tools.
* [Visual Studio Community](https://www.visualstudio.com/en-us/products/visual-studio-community-vs.aspx) - Free editor for individual developers, open source projects, academic research, education, and small professional teams.

### Internationalization
* [Localization](https://github.com/aspnet/Localization) - Localization abstractions and implementations for ASP.NET Core applications.

### IOC
* [AutoDI](https://github.com/Keboo/AutoDI) - Super-fast compile-time dependency injection using IL weaving.
* [Autofac](https://github.com/autofac/Autofac) - Addictive .NET IoC container.
* [Castle.Windsor](https://github.com/castleproject/Windsor) Castle Windsor is a best of breed, mature Inversion of Control container available for .NET.
* [DryIoc](https://bitbucket.org/dadhi/dryioc) - Fast, small, full-featured IoC Container for .NET.
* [LightInject](https://github.com/seesharper/LightInject) - Ultra lightweight IoC container [http://www.lightinject.net](http://www.lightinject.net).
* [SimpleInjector](https://github.com/simpleinjector/SimpleInjector) - Easy, flexible, and fast Dependency Injection library that promotes best practice to steer developers towards the pit of success.
* [Stashbox](https://github.com/z4kn4fein/stashbox) - A lightweight, portable dependency injection framework for .NET based solutions.
* [StructureMap](https://github.com/structuremap/structuremap) - Dependency Injection/Inversion of Control tool for .NET.

### Logging
* [common-logging](https://github.com/net-commons/common-logging) - Portable logging abstraction for .NET [http://net-commons.github.io/common-logging](http://net-commons.github.io/common-logging).
* [dnxcore-logging-logstash](https://github.com/jvandevelde/dnxcore-logging-logstash) - Logstash logging extension for .NET Core applications with UDP and Redis transports.
* [Exceptionless](https://github.com/exceptionless/Exceptionless.Net) - Exceptionless .NET Client
* [Foundatio](https://github.com/exceptionless/Foundatio#logging) - A fluent logging api that can be used to log messages throughout your application.
* [LibLog](https://github.com/damianh/LibLog) - Single file for you to either copy/paste or install via nuget, into your library/ framework/ application to provide a logging abstraction.
* [log4net](https://github.com/apache/logging-log4net) - log4net is a port of the excellent Apache log4j™ framework to the Microsoft® .NET runtime.
* [NLog](https://github.com/NLog/NLog) - Advanced .NET, Silverlight and Xamarin Logging.
* [Q42.Logging.ApplicationInsights](https://github.com/Q42/Q42.Logging.ApplicationInsights) - Log appender for the build in ASP.NET Core logging to send all logs to Application Insights.
* [serilog](https://github.com/serilog/serilog) - Simple .NET logging with fully-structured events.
* [SEQ](https://getseq.net) - Seq collects data over HTTP, while your applications use the best available structured logging APIs for your platform.

### Machine Learning and Data Science
* [Accord](https://github.com/accord-net/framework) - Machine learning, computer vision, statistics and general scientific computing for .NET.
* [Spreads](https://github.com/Spreads/Spreads/) - Series and Panels for Real-time and Exploratory Analysis of Data Streams.
* [TensorFlowSharp](https://github.com/migueldeicaza/TensorFlowSharp) - TensorFlow API for .NET languages.

### Mail
* [MailBody](https://github.com/doxakis/MailBody) - Create transactional email with a fluent interface (.NET).
* [MailKit](https://github.com/jstedfast/MailKit) - Cross-platform .NET library for IMAP, POP3, and SMTP.
* [MailMergeLib](https://github.com/axuno/MailMergeLib) - SMTP mail client library which provides comfortable mail merge capabilities for text, inline images and attachments, as well as good throughput and fault tolerance for sending mail messages.
* [MimeKit](https://github.com/jstedfast/MimeKit) - Cross-platform .NET MIME creation and parser library with support for S/MIME, PGP, DKIM, TNEF and Unix mbox spools.
* [PreMailer.Net](https://github.com/milkshakesoftware/PreMailer.Net/tree/dotnet-core) - C# library that moves your stylesheets to inline style attributes, for maximum compatibility with E-mail clients.
* [SendGrid Client](https://github.com/0xdeafcafe/sendgrid-dotnet) - C# library for the SendGrid v3 mail endpoint.
* [StrongGrid](https://github.com/Jericho/StrongGrid) - Client for SendGrid's v3 API. Not only allows you to send emails, but also allows you to bulk import contacts, manage lists and segments, create custom fields for your lists, etc. Also includes a parser for SendGrid Webhooks.

### Mathematics
* [UnitConversion](https://github.com/Stratajet/UnitConversion) - Expansible Unit Conversion Library for .NET Core and .NET Framework.

### Misc
* [AngleSharp](https://github.com/AngleSharp/AngleSharp) - The ultimate angle brackets parser library. It parses HTML5, MathML, SVG and CSS to construct a DOM based on the official W3C specification. Comparable to beautifulsoup4 of python.
* [AutoMapper](https://github.com/AutoMapper/AutoMapper) - Convention-based object-object mapper in .NET.
* [Castle.Core](https://github.com/castleproject/Core) - Castle Core, including Castle DynamicProxy, Logging Services and DictionaryAdapter [http://www.castleproject.org](http://www.castleproject.org).
* [Chessie](https://github.com/fsprojects/Chessie) - Railway-oriented programming for .NET [http://fsprojects.github.io/Chessie](http://fsprojects.github.io/Chessie).
* [CliWrap](https://github.com/Tyrrrz/CliWrap) - Wrapper for command line interfaces.
* [CommonMark.NET](https://github.com/Knagis/CommonMark.NET) - The implementation of CommonMark specification in C# for converting Markdown documents to HTML.
* [ConsoleTableExt](https://github.com/minhhungit/ConsoleTableExt) - Fluent library to create table for .NET console application.
* [datatables](https://github.com/ALMMa/datatables.aspnet/tree/dev) - Microsoft ASP.NET server-side support and helpers for jQuery DataTables.
* [DinkToPdf](https://github.com/rdvojmoc/DinkToPdf) - C# .NET Core wrapper for wkhtmltopdf library that uses Webkit engine to convert HTML pages to PDF.
* [Enums.NET](https://github.com/TylerBrinkley/Enums.NET) - Enums.NET is a high-performance type-safe .NET enum utility library
* [FluentFTP](https://github.com/robinrodricks/FluentFTP/) - FTP and FTPS client, with extensive FTP commands, SSL/TLS connections, hashing/checksums and more.
* [HdrHistogram.NET](https://github.com/HdrHistogram/HdrHistogram.NET) - High Dynamic Range (HDR) Histogram.
* [httpclient-interception](https://github.com/justeat/httpclient-interception) - .NET Standard library for intercepting server-side HTTP dependencies.
* [Humanizer](https://github.com/Humanizr/Humanizer) - Humanizer meets all your .NET needs for manipulating and displaying strings, enums, dates, times, timespans, numbers and quantities.
* [Humidifier](https://github.com/jakejscott/Humidifier) - Write and maintain AWS Cloudformation templates using C#.
* [LibSass Host](https://github.com/Taritsyn/LibSassHost) - .NET wrapper around the [libSass](http://sass-lang.com/libsass) library with the ability to support a virtual file system.
* [markdig](https://github.com/lunet-io/markdig) - Fast, powerfull, CommonMark compliant, extensible Markdown processor for .NET.
* [NReco.LambdaParser](https://github.com/nreco/lambdaparser) - Parses string expressions (formulas, methods calls, conditions) to LINQ expression tree that can be compiled to lambda and evaluated.
* [readline](https://github.com/tsolarin/readline) - Pure C# GNU-Readline like library for .NET/.NET Core.
* [Relinq](https://github.com/re-motion/Relinq) - With re-linq, it's now easier than ever to create full-featured LINQ providers.
* [ReverseMarkdown](https://github.com/mysticmind/reversemarkdown-net) - Html to Markdown converter library.
* [PdfReport.Core](https://github.com/VahidN/PdfReport.Core) - PdfReport.Core is a code first reporting engine, which is built on top of the iTextSharp.LGPLv2.Core and EPPlus.Core libraries.
* [Scientist](https://github.com/github/Scientist.net) - .NET library for carefully refactoring critical paths. It's a port of GitHub's Ruby Scientist library.
* [Scrutor](https://github.com/khellang/Scrutor) - Assembly scanning extensions for Microsoft.Extensions.DependencyInjection.
* [SmartFormat.NET](https://github.com/scottrippey/SmartFormat.NET) - An extensible replacement for string.Format.
* Stocks
  * [Trady](https://github.com/lppkarl/Trady) - Handy library for computing technical indicators, and it targets to be an automated trading system that provides stock data feeding, indicator computing, strategy building and automatic trading.
* [System.Linq.Dynamic.Core](https://github.com/StefH/System.Linq.Dynamic.Core) - The .NET Standard (.NET Core) version from the System Linq Dynamic functionality.
* Validation
  * [FluentValidation](https://github.com/JeremySkinner/FluentValidation) - Small validation library for .NET that uses a fluent interface and lambda expressions for building validation rules.
  * [Valit](https://github.com/valit-stack/Valit) - A dead simple validation for .NET Core. No more if-statements all around your code. Write nice and clean fluent validators instead!
* [warden-stack](https://github.com/warden-stack) - "health checks" for your applications, resources and infrastructure. Keep your Warden on the watch.
* [Xabe.FFmpeg](https://github.com/tomaszzmuda/Xabe.FFmpeg) - .NET Standard wrapper for FFmpeg. It allows to process media without know how FFmpeg works, and can be used to pass customized arguments to FFmpeg from C# application.
* [YoutubeExplode](https://github.com/Tyrrrz/YoutubeExplode) - Ultimate library for extracting metadata and downloading Youtube videos and playlists.

### Networking
* [CurlThin](https://github.com/stil/CurlThin) - Lightweight cURL binding library for C# with support for multiple simultaneous transfers through curl_multi interface.
* [NETStandard.HttpListener](https://github.com/StefH/NETStandard.HttpListener) - HttpListener for .NET Core (NETStandard).

### ORM
* [Entity Framework Core](https://github.com/aspnet/EntityFramework) - Familiar developer experience to previous versions of EF, including LINQ, POCO, and Code First support.
  * [EntityFramework-Plus](https://github.com/zzzprojects/EntityFramework-Plus) - Entity Framework Utilities | Bulk Operations | Batch Delete | Batch Update | Query Cache | Query Filter | Query Future | Query Include | Audit.
  * [EntityFramework.Triggers](https://github.com/NickStrupat/EntityFramework.Triggers) - Trigger events for EF.
  * [EntityFramework.Rx](https://github.com/NickStrupat/EntityFramework.Rx) - Reactive **hot** observables of your EF operations.
  * [EntityFramework.PrimaryKey](https://github.com/NickStrupat/EntityFramework.PrimaryKey) - Easily get the primary key of any entity (including composite keys).
  * [EntityFramework.TypedOriginalValues](https://github.com/NickStrupat/EntityFramework.TypedOriginalValues) - Get a proxy object of the orginal values of your entity (typed access to Property("...").OriginalValue).
  * [EntityFramework.VersionedProperties](https://github.com/NickStrupat/EntityFramework.VersionedProperties) - Classes which auto-magically keep an audit history of the changes to the specified property.
  * [LINQKit](https://github.com/scottksmith95/LINQKit) - A free set of extensions for LINQ to SQL and Entity Framework power users.
  * [Pomelo.EntityFrameworkCore.MySql](https://github.com/PomeloFoundation/Pomelo.EntityFrameworkCore.MySql) - Entity Framework Core provider for MySql built on top of mysql-net/MySqlConnector.
* [Dapper](https://github.com/StackExchange/Dapper) - Simple object mapper for .NET.
  * [Dapper-FluentMap](https://github.com/henkmollema/Dapper-FluentMap) - Provides a simple API to fluently map POCO properties to database columns when using Dapper.
  * [Dommel](https://github.com/henkmollema/Dommel) - Simple CRUD operations for Dapper.
  * [MicroOrm.Dapper.Repositories](https://github.com/phnx47/MicroOrm.Dapper.Repositories) - CRUD for Dapper.
* [Limebean](https://nick-lucas.github.io/LimeBean/) - Hybrid-ORM, designed to be simple to use and not totally hide SQL, while having all the nice things you expect from an ORM. Inspired by RedBeanPHP.
* [LINQ to DB (linq2db)](https://linq2db.github.io/) - The fastest LINQ database access library offering a simple, lightweight, fast, and type-safe layer between your POCO objects and your database for more than 10 database engines with full SQL support.
* [NEventStore](https://github.com/NEventStore/NEventStore/tree/feature/dotnetcore) - Persistence library used to abstract different storage implementations when using event sourcing as storage mechanism. This library is developed with a specific focus on DDD/CQRS applications.
* [NPoco](https://github.com/schotime/NPoco) - Simple microORM that maps the results of a query onto a POCO object. Project based on Schotime's branch of PetaPoco.
* [NReco.Data](https://github.com/nreco/data) - Lightweight provider-independent DAL for SQL commands generation, CRUD operations and simple POCO mapping.
* [ServiceStack.OrmLite](https://github.com/ServiceStack/ServiceStack.OrmLite) - Light, simple and fast convention-based POCO ORM.
* [SqlFu](https://github.com/sapiens/SqlFu) - Fast and versatile Micro-ORM.
* [SQLStreamStore](https://github.com/SQLStreamStore/SQLStreamStore) - Stream Store library targeting SQL based implementations for .NET.

### Profiling
* [Glimpse](https://github.com/Glimpse/Glimpse.Prototype) - Lightweight, open-source, real-time diagnostics and insights profiler for .NET. `Unstable version`
* [MiniProfiler](https://github.com/MiniProfiler/dotnet) - A simple but effective mini-profiler for ASP.NET websites.

### Query Builders
* [SqlKata](https://github.com/sqlkata/querybuilder) - Elegant Sql Query Builder, that supports complex queries, joins, sub queries, nested where conditions, vendor engine targets and more

### Queue and Messaging
* [emitter](https://emitter.io/) - Free open source real-time messaging service that connects all devices. This publish-subscribe messaging API is built for speed and security.
* [EventStore](https://github.com/EventStore/EventStore) - The open-source, functional database with Complex Event Processing in JavaScript.
* [Foundatio](https://github.com/exceptionless/Foundatio#queues) - A common interface with in memory, redis and azure implementations.
* [MediatR](https://github.com/jbogard/MediatR) - Simple, unambitious mediator implementation in .NET.
 * [MediatR.Extensions.Microsoft.DependencyInjection](https://github.com/jbogard/MediatR.Extensions.Microsoft.DependencyInjection) - MediatR extensions for Microsoft.Extensions.DependencyInjection.
* [Mediator.Net](https://github.com/mayuanyang/Mediator.Net) - A simple mediator for .Net for sending command, publishing event and request response with pipelines supported.
* [MicroBus](https://github.com/Lavinski/Enexure.MicroBus) - Simple in process mediator for .NET.
* [netmq](https://github.com/zeromq/netmq) - 100% native C# implementation of ZeroMQ for .NET.
* [rabbitmq-dotnet-client](https://github.com/rabbitmq/rabbitmq-dotnet-client) - RabbitMQ .NET client [https://www.rabbitmq.com](https://www.rabbitmq.com).
* [RawRabbit](https://github.com/pardahlman/RawRabbit) - Modern .NET framework for communication over RabbitMq.
* [Rebus](https://github.com/rebus-org/Rebus) - Simple and lean service bus implementation for .NET.
* [Restbus](http://restbus.org) - Messaging library for RabbitMq.
* [Tossit](https://github.com/turgayozgur/tossit) - Simple, easy to use library for distributed job/worker logic. Distributed messages handled by built in RabbitMQ implementation.

### Scheduler and Job
* [Chroniton.NetCore](https://github.com/leosperry/Chroniton) - Lightweight robust library for running tasks(jobs) on schedules.
* [FluentScheduler](https://github.com/fluentscheduler/FluentScheduler) - Automated job scheduler with fluent interface.
* [HangfireIO](https://github.com/HangfireIO/Hangfire) - Easy way to perform fire-and-forget, delayed and recurring tasks inside ASP.NET apps [http://hangfire.io](http://hangfire.io).
* [LiquidState](https://github.com/prasannavl/LiquidState) - Efficient asynchronous and synchronous state machines for .NET
* [quartznet](https://github.com/quartznet/quartznet/) - Quartz Enterprise Scheduler .NET [http://www.quartz-scheduler.net](http://www.quartz-scheduler.net).
* [stateless](https://github.com/dotnet-state-machine/stateless) - Simple library for creating state machines in C# code.

### SDKs
* [AWS SDK](https://github.com/aws/aws-sdk-net) - The Amazon Web Services (AWS) .NET Core SDK components. Each AWS service has its own NuGet package.
* [azure-event-hubs-dotnet](https://github.com/azure/azure-event-hubs-dotnet) - .NET Standard client library for Azure Event Hubs.
* Blockchain clients
  * [Bittrex.Net](https://github.com/JKorf/Bittrex.Net) - C# .Net wrapper for the Bittrex web API including all features easily accessible and usable.
  * [Binance.Net](https://github.com/JKorf/Binance.Net) - .Net API wrapper for the Binance web API.
* [consuldotnet](https://github.com/PlayFab/consuldotnet/tree/develop) - .NET API for Consul.
* [DarkSkyCore](https://github.com/amweiss/dark-sky-core) - A .NET Standard wrapper for the [Dark Sky API](https://darksky.net/dev/docs).
* [Docker.DotNet](https://github.com/Microsoft/Docker.DotNet) - .NET (C#) Client Library for Docker API.
* [google-cloud-dotnet](https://github.com/GoogleCloudPlatform/google-cloud-dotnet) - Google Cloud Client Libraries for .NET.
* [Microphone](https://github.com/rogeralsing/Microphone) - Lightweight framework to run self hosting REST services using Web Api or NancyFx ontop of a Consul or ETCD cluster.
* [NetTelegramBotApi](https://github.com/justdmitry/NetTelegramBotApi) - C# client library for building Telegram bot [https://core.telegram.org/bots/api](https://core.telegram.org/bots/api).
* [octokit.net](https://github.com/octokit/octokit.net) - GitHub API client library for .NET.
* [Open-XML-SDK](https://github.com/OfficeDev/Open-XML-SDK) - The Open XML SDK provides tools for working with Office Word, Excel, and PowerPoint documents.
* [PreStorm](https://github.com/jshirota/PreStorm) - Parallel REST Client for ArcGIS Server.
* [SendGrid-csharp](https://github.com/sendgrid/sendgrid-csharp) - C# client library for using the full SendGrid API.
* [statsd-csharp-client](https://github.com/Pereingo/statsd-csharp-client) - .NET Standard compatible C# client to interface with Etsy's excellent [statsd](https://github.com/etsy/statsd) server.
* [tweetinvi](https://github.com/linvi/tweetinvi) - Intuitive .NET C# library to access the Twitter REST and STREAM API.

### Security
* [HtmlSanitizer](https://github.com/mganss/HtmlSanitizer) - Cleans HTML to avoid XSS attacks.
* [jose-jwt](https://github.com/dvsekhvalnov/jose-jwt) - Library for processing JOSE objects (JWT, JWA, JWS and related).
* [NWebsec](https://github.com/NWebsec/NWebsec) - Security libraries for ASP.NET [https://www.nwebsec.com](https://www.nwebsec.com).
* [reCAPTCHA](https://github.com/PaulMiami/reCAPTCHA) - reCAPTCHA 2.0 for ASP.NET Core.
* [roslyn-security-guard](https://github.com/dotnet-security-guard/roslyn-security-guard) - Roslyn analyzers that aim to help security audit on .NET applications.
* [OwaspHeaders](https://github.com/GaProgMan/OwaspHeaders.Core) - .NET Core middleware for injecting the Owasp recommended HTTP Headers for increased security.
* [Security](https://github.com/aspnet/Security) - Middleware for security and authorization of web apps.
* [SecurityHeaders](https://github.com/andrewlock/NetEscapades.AspNetCore.SecurityHeaders) - Small package to allow adding security headers to ASP.NET Core websites.

### Searching
* [AutoComplete](https://github.com/omerfarukz/autocomplete) - Persistent, simple, powerful and portable autocomplete library.
* [Elasticsearch.Net & NEST](https://github.com/elastic/elasticsearch-net) - Repository for both NEST and Elasticsearch.NET, the two official elasticsearch .NET clients.
* [ElasticsearchCRUD](https://github.com/damienbod/ElasticsearchCRUD) - Elasticsearch .NET API.
* [SimMetrics.Net](https://github.com/StefH/SimMetrics.Net) - A Similarity Metric Library, e.g. from edit distance's (Levenshtein, Gotoh, Jaro etc) to other metrics, (e.g Soundex, Chapman)
* [SolrExpress](https://github.com/solr-express/solr-express) - Simple and lightweight query .NET library for Solr, in a controlled, buildable and fail fast way.

### Serialization
* [bond](https://github.com/Microsoft/bond) - Cross-platform framework for working with schematized data. It supports cross-language de/serialization and powerful generic mechanisms for efficiently manipulating data. Bond is broadly used at Microsoft in high scale services.
* [Channels](https://github.com/davidfowl/Channels) - Push based .NET Streams.
* [CsvHelper](https://github.com/JoshClose/CsvHelper) - Library to help reading and writing CSV files.
* [Edi.Net](https://github.com/indice-co/EDI.Net) - EDI Serializer/Deserializer. Supports EDIFact, X12 and TRADACOMS format.
* [ExtendedXmlSerializer](https://github.com/wojtpl2/ExtendedXmlSerializer) - Extended Xml Serializer for .NET.
* [Jil](https://github.com/kevin-montrose/Jil) - Fast .NET JSON (De)Serializer, Built On Sigil.
* [msgpack-cli](https://github.com/msgpack/msgpack-cli) - MessagePack implementation for Common Language Infrastructure / [msgpack.org](http://msgpack.org).
* [Newtonsoft.Json](https://github.com/JamesNK/Newtonsoft.Json) - Popular high-performance JSON framework for .NET.
* [protobuf-net](https://github.com/mgravell/protobuf-net/) - Protocol Buffers library for idiomatic .NET.
* [Schema.NET](https://github.com/RehanSaeed/Schema.NET) - Schema.org objects turned into strongly typed C# POCO classes for use in .NET. All classes can be serialized into JSON/JSON-LD and XML, typically used to represent structured data in the head section of html page.
* [ServiceStack.Text](https://github.com/ServiceStack/ServiceStack.Text) - JSON, JSV and CSV Text Serializers.
* [TinyCsvParser](https://github.com/bytefish/TinyCsvParser) - Easy to use, easy to extend and high-performance library for CSV parsing with .NET.
* [Wire](https://github.com/rogeralsing/Wire) - Binary serializer for POCO objects.
* [YamlDotNet](https://github.com/aaubry/YamlDotNet) - .NET
* [ZeroFormatter](https://github.com/neuecc/ZeroFormatter) - Fast binary (de)serializer for .NET.
* [Utf8Json](https://github.com/neuecc/Utf8Json) - Definitely Fastest and Zero Allocation JSON Serializer for C#(NET, .NET Core, Unity, Xamarin).
* [YAXLib](https://github.com/sinairv/YAXLib) - XML Serialization Library for the .NET Framework and .NET Core. Extremely flexible and powerful.

### Template Engine
* [dotliquid](https://github.com/dotliquid/dotliquid) - .NET Port of Tobias Lütke's Liquid template language.
* [fluid](https://github.com/sebastienros/fluid) - Open-source .NET template engine that is as close as possible to the Liquid template language.
* [Razor](https://github.com/aspnet/Razor) - Parser and code generator for CSHTML files used in view pages for MVC web apps.

### Testing
* [Bogus](https://github.com/bchavez/Bogus) - Simple and sane fake data generator for C#. Based on and ported from the famed faker.js.
* [FakeItEasy](https://github.com/FakeItEasy/FakeItEasy) - The easy mocking library for .NET.
* [FluentAssertions](https://github.com/dennisdoomen/FluentAssertions) - Set of .NET extension methods that allow you to more naturally specify the expected outcome of a TDD or BDD-style test.
* [GenFu](https://github.com/MisterJames/GenFu) - Library you can use to generate realistic test data.
* [LightBDD](https://github.com/LightBDD/LightBDD) - BDD framework allowing to create easy to read and maintain tests.
* [mockhttp](https://github.com/richardszalay/mockhttp) - Testing layer for Microsoft's HttpClient library.
* [moq.netcore](https://github.com/Moq/moq4) - Most popular and friendly mocking framework for .NET.
* [MSpec](https://github.com/machine/machine.specifications) - Popular testing framework for writing BDD-style tests.
* [MyTested.AspNetCore.Mvc](https://github.com/ivaylokenov/MyTested.AspNetCore.Mvc) - Fluent testing
  framework for ASP.NET Core MVC.
* [Netling](https://github.com/hallatore/Netling) - Load tester client for easy web testing.
* [NSpec](https://github.com/nspec/NSpec) - Battle hardened testing framework for C# that's heavily inspired by Mocha and RSpec.
* [NSubstitute](https://github.com/nsubstitute/NSubstitute) - A friendly substitute for .NET mocking frameworks.
* [nunit](https://github.com/nunit/dotnet-test-nunit) - NUnit test runner for .NET Core.
* [shouldly](https://github.com/shouldly/shouldly) - Should testing for .NET - the way Asserting *Should* be! [http://shouldly.readthedocs.org/en/latest](http://shouldly.readthedocs.org/en/latest)
* [SpecFlow](https://github.com/techtalk/SpecFlow/tree/DotNetCore) - Pragmatic BDD solution for .NET. It uses the Gherkin specification language and integrates to Visual Studio.
* [Storyteller](https://github.com/storyteller/Storyteller) - Executable Specifications for .NET [http://storyteller.github.io](http://storyteller.github.io).
* [Stubbery](https://markvincze.github.io/Stubbery/) - A simple library for creating and running Api stubs in .NET.
* [TestStack.BDDfy](https://github.com/TestStack/TestStack.BDDfy) - The simplest BDD framework EVER!
* [xBehave.net](https://github.com/xbehave/xbehave.net) - An xUnit.net extension for describing your tests using natural language. [http://xbehave.github.io](http://xbehave.github.io)
* [xUnit.net](https://github.com/xunit/xunit) - A free, open source, community-focused unit testing tool for the .NET Framework.

### Tools
* [CommandLineUtils](https://github.com/natemcmaster/CommandLineUtils) - Command line parsing and utilities for .NET Core and .NET Framework.
* [docfx](https://github.com/dotnet/docfx) - Tools for building and publishing API documentation for .NET projects [http://dotnet.github.io/docfx](http://dotnet.github.io/docfx)
* [dotnetfiddle](https://dotnetfiddle.net) - .NET sandbox for developers to quickly try out code and share code snippets.
* [EntryPoint](https://github.com/Nick-Lucas/EntryPoint) - Composable CLI (Command Line) Argument Parser for .Net Core & .Net Framework 4.5+.
* [Fake JSON Server](https://github.com/ttu/dotnet-fake-json-server) - Fake REST API for prototyping or as a CRUD Back End. No need to define types, uses dynamic typing. Data is stored to a single JSON file. Has authentication, WebSocket notifications, async long running operations, random generation for errors/delays and experimental GraphQL support.
* [gitignore.io](https://github.com/joeblau/gitignore.io) - Create useful .gitignore files for your project [https://www.gitignore.io](https://www.gitignore.io).
* [ICanHasDotnetCore](https://github.com/OctopusDeploy/ICanHasDotnetCore) - Scans uploaded packages.config files or GitHub repository and determines whether the nuget packages target .NET Standard [https://icanhasdot.net](https://icanhasdot.net).
* [json2csharp](http://json2csharp.com) - Generate C# classes from JSON.
* [letsencrypt-win-simple](https://github.com/Lone-Coder/letsencrypt-win-simple) - A Simple ACME Client for Windows.
* [NuGetPackageExplorer](https://github.com/NuGetPackageExplorer/NuGetPackageExplorer) - Create, update and deploy Nuget Packages with a GUI.
* [NugetVisualizer](https://github.com/sepharg/NugetVisualizer) - Visualize all of the nuget packages and their corresponding versions for a set of given git repositories or folders.
* [OctoLinker](https://github.com/OctoLinker/browser-extension) - Navigate through `projects.json` files efficiently with the OctoLinker browser extension for GitHub.
* [ShareX](https://github.com/ShareX/ShareX) - Free and open source program that lets you capture or record any area of your screen and share it with a single press of a key. It also allows uploading images, text or other types of files to over 80 supported destinations you can choose from. [https://getsharex.com](https://getsharex.com)
* [SharpLab](https://github.com/ashmind/SharpLab) - .NET code playground that shows intermediate steps and results of code compilation. [https://sharplab.io](https://sharplab.io)
* [X.Web.Sitemap](https://github.com/dncuug/X.Web.Sitemap) – Simple sitemap generator for .NET and .NET Core
* [X.Web.RSS](https://github.com/dncuug/X.Web.RSS) – Simple RSS Feed generator for .NET and .NET Core

### Web Framework
* WebAssembly
  * [Blazor](https://github.com/SteveSanderson/Blazor) - UI framework running .NET in the browser via WebAssembly.
  * [Ooui](https://github.com/praeclarum/Ooui) - Small cross-platform UI library that brings the simplicity of native UI development to the web.
* [ReactJS.NET](https://github.com/reactjs/React.NET) - .NET library for JSX compilation and server-side rendering of React components.
* [redux.NET](https://github.com/GuillaumeSalles/redux.NET) - Predictable state container for .NET apps. Inspired by [https://github.com/reactjs/redux](https://github.com/reactjs/redux).

### Web Socket
* [Fleck](https://github.com/statianzo/Fleck) - Fleck is a WebSocket server implementation in C#. Fleck requires no inheritance, container, or additional references.
* [SignalR Server](https://github.com/aspnet/signalr) - Real-time web functionality for web apps, including server-side push.
* [SuperSocket](https://github.com/kerryjiang/SuperSocket) - Light weight, cross platform and extensible socket server application framework.
* [WampSharp](https://github.com/Code-Sharp/WampSharp) - C# implementation of [The Web Application Messaging Protocol](http://wamp-proto.org/) - Protocol that provides messaging patterns of Remote Procedure Calls and Publish/Subscribe over WebSockets.
* [websocket-manager](https://github.com/radu-matei/websocket-manager) - Real-Time library for ASP .NET Core.

### Windows Service
* [dotnet-win32-service](https://github.com/dasMulli/dotnet-win32-service) - Set up and run as Windows Service directly from .NET Core.
* [Topshelf](https://github.com/Topshelf/Topshelf) - Easy service hosting framework for building Windows services using .NET.

### Workflow
* [CoreWF](https://github.com/dmetzgar/corewf/) - Port of Windows Workflow Foundation (WF) to .NET Core.
* [workflow-core](https://github.com/danielgerlag/workflow-core) - Lightweight workflow engine for .NET Standard.

## Starter Kits
* [Arch](https://github.com/Arch) - The collection of .NET Core libraries that are created by software architects who embrace all the new stuff in .NET Core.
* [AspNetCore-Angular2-Universal](https://github.com/MarkPieszak/aspnetcore-angular2-universal) - Cross-platform - w/ server-side rendering for SEO, Bootstrap, i18n internationalization (ngx-translate), Webpack, TypeScript, unit testing w/ Karma, WebAPI REST setup, SignalR, Swagger docs, and more!
* [ASP.NET Core Starter Kit](https://github.com/kriasoft/aspnet-starter-kit) - Opinionated boilerplate for web development based on .NET Core, Kestrel, GraphQL on the backend and Babel, Webpack, React and Redux on the frontend. This boilerplate comes in both C# and F# flavors.
* [ASP.NET Boilerplate](https://github.com/aspnetboilerplate/aspnetboilerplate) - ASP.NET Boilerplate is a starting point for new modern web applications using best practices and most popular tools. It's aimed to be a SOLID model, a general-purpose application framework and a project template. `4.5.x or above`
* [aspnetcore-spa generator](https://github.com/aspnet/JavaScriptServices) - Yeoman generator to build a brand-new ASP.NET Core single page application that uses Angular 2 / React / React With Redux / Knockout / Aurelia on the client.
* [ASP.Net Core Vue Starter](https://github.com/MarkPieszak/aspnetcore-Vue-starter) - Asp.NETCore 2.0 Vue 2 (ES6) SPA Starter kit, contains routing, Vuex, and more!.
* [bitwarden-core](https://github.com/bitwarden/core) - The core infrastructure backend (API, database, etc) [https://bitwarden.com](https://bitwarden.com).
* [dotNetify](https://github.com/dsuryd/dotNetify) - Simple, lightweight, yet powerful way to build real-time HTML5/C# .NET web apps.
* [generator-aspnet](https://github.com/OmniSharp/generator-aspnet) - yo generator for ASP.NET Core.
* [react-aspnet-boilerplate](https://github.com/pauldotknopf/react-aspnet-boilerplate) - Starting point for building isomorphic React applications with ASP.NET Core 1, leveraging existing techniques.
* [saaskit](https://github.com/saaskit/saaskit) - Developer toolkit for building SaaS applications.

## Sample Projects
* [AlbumViewerVNext](https://github.com/RickStrahl/AlbumViewerVNext) - West Wind Album Viewer ASP.NET 5 Sample.
* [allReady](https://github.com/HTBox/allReady) - Open-source solution focused on increasing awareness, efficiency and impact of preparedness campaigns as they are delivered by humanitarian and disaster response organizations in local communities. [http://www.htbox.org/projects/allready](http://www.htbox.org/projects/allready)
* [AspNet5GeoElasticsearch](https://github.com/damienbod/AspNet5GeoElasticsearch) - ASP.NET Core MVC Geo Elasticsearch Swashbuckle Swagger.
* [aspnet-servicediscovery-patterns](https://github.com/cecilphillip/aspnet-servicediscovery-patterns) - Samples of implementing Service Discovery patterns with ASP.NET Core.
* [AspNetAuthorizationWorkshop](https://github.com/blowdart/AspNetAuthorizationWorkshop) - A workshop for moving through the various new pieces in ASP.NET Core Authorization
* [BikeSharing360 Suite of Apps from Microsoft](https://blogs.msdn.microsoft.com/visualstudio/2016/12/14/connectdemos-2016-bikesharing360-on-github/) Presented December Connect 2016 Conference, a compreshsive set of interworking apps for both enterprise users and the consumers (bike riders):
 [Mobile Apps](https://github.com/Microsoft/BikeSharing360_MobileApps), [Backend Services](https://github.com/Microsoft/BikeSharing360_BackendServices), [Websites](https://github.com/Microsoft/BikeSharing360_Websites), [Single Container Apps](https://github.com/Microsoft/BikeSharing360_SingleContainer), [Multi Container Apps](https://github.com/Microsoft/BikeSharing360_MultiContainer), [Cognitive Services Kiosk App](https://github.com/Microsoft/BikeSharing360_CognitiveServicesKioskApp),
 [Azure Bot App](https://github.com/Microsoft/BikeSharing360_BotApps).
* [cloudscribe](https://github.com/joeaudette/cloudscribe) - ASP.NET Core Multi-tenant web application foundation.
* [CoreCodeCamp](https://github.com/shawnwildermuth/CoreCodeCamp) - An Open Source Website for running small, local development events.
* [distributed-playground](https://github.com/jvandevelde/distributed-playground) - Distributed service playground with Vagrant, Consul, Docker & ASP.NET Core.
* [DotNetClub](https://github.com/scheshan/DotNetClub) - Tiny club written in ASP.NET Core.
* [Entropy](https://github.com/aspnet/Entropy) - Chaotic experimental playground for new features and ideas - check here for small and simple samples for individual features.
* [EquinoxProject](https://github.com/EduardoPires/EquinoxProject) - Full ASP.NET Core 2.0 application with DDD, CQRS and Event Sourcing.
* [eShopOnContainers](https://github.com/dotnet/eShopOnContainers) - Microservices Architecture and Containers based Reference Application.
* [guidance-identity-management-for-multitenant-apps](https://github.com/Azure-Samples/guidance-identity-management-for-multitenant-apps) - How to manage user identities in a multitenant app on Microsoft Azure, using Azure Active Directory for authentication.
* [magazine-website](https://github.com/thangchung/magazine-website) - Magazine website (using .NET Core, ASP.NET Core, EF Core) with DDD, CQRS, microservices, asynchronous programming applied.
* [MegaMine](https://github.com/Nootus/MegaMine) - Open source mining solution that helps miners in extracting Gold, Quartz, Granite etc. This solution is built using ASP.NET Core and AngularJS utilizing multiple light weight components in a Microservices way.
* [minicompiler](https://github.com/ealsur/minicompiler) - Minification, bundling and compiling sample.
* [MusicStore](https://github.com/aspnet/MusicStore) - Sample MusicStore application that uses MVC and Entity Framework.
* [NLayerAppV3](https://github.com/cesarcastrocuba/nlayerappv3) - NLayerAppV3 N-Layered Architecture with .NET Core Preview 2.
* [Orchard Core - Modular and Multi-tenant applications](https://github.com/OrchardCMS/OrchardCore.Samples) - Use Orchard Core Framework to create Modular and Multi-tenant applications.
* [ReactiveTraderCloud](https://github.com/AdaptiveConsulting/ReactiveTraderCloud) - Real-time trading platform demo showcasing reactive programming principles applied across the full application stack.
* [PhotoGallery](https://github.com/chsakell/aspnet5-angular2-typescript) - Cross-platform Single Page Applications with ASP.NET Core, Angular 2 & TypeScript [http://wp.me/p3mRWu-11L](http://wp.me/p3mRWu-11L).
* [Practical ASP.NET Core](https://github.com/dodyg/practical-aspnetcore) - A daily updated micro samples of ASP.NET Core features and facilities.
* [JustA.ML](https://github.com/mustakimali/JustA.ML) - A web application that lets you share files/URL/text between your devices written in ASP.NET Core 2.0. Open source, live at [https://justa.ml](https://justa.ml)

## Articles
* Basic knowledge
  * [A guide to the .NET Core projects on GitHub](https://blog.rendle.io/a-guide-to-the-net-projects-on-github/)
  * [Microsoft architectual overview of comprehensive BikeSharing360 suite of demo apps with related videos](https://blogs.msdn.microsoft.com/visualstudio/2016/12/14/connectdemos-2016-bikesharing360-on-github/)
  * [Porting a .NET Framework library to .NET Core](https://www.codeproject.com/Articles/1190475/Porting-a-NET-Framework-library-to-NET-Core)
  * [The 68 things the CLR does before executing a single line of your code](http://mattwarren.org/2017/02/07/The-68-things-the-CLR-does-before-executing-a-single-line-of-your-code/)
  * The comparison between .NET Core and Nodejs at [here](https://manuel-rauber.com/2016/03/07/node-js-asp-net-core-1-0-a-usage-comparison/), [here](https://gist.github.com/ilyaigpetrov/f6df3e6f825ae1b5c7e2) and [here](https://github.com/thinktecture/nodejs-aspnetcore-webapi)
  * [Understanding ASP.NET Core Initialization](http://developer.telerik.com/featured/understanding-asp-net-core-initialization/)
  * [Why you should join .NET Core and ASP.NET Core train](https://codingblast.com/why-you-should-join-asp-net-core/)
* Cloud Development
  * [Configuring the AWS SDK in .NET Core](https://aws.amazon.com/blogs/developer/configuring-aws-sdk-with-net-core/)
  * [Serverless Architecture using C# and AWS Amazon Gateway Api/Lambda](https://www.codeproject.com/Articles/1178781/Serverless-Architecture-using-Csharp-and-AWS-Amazo)
  * [Using C# and .NET Core in Amazon Web Services (AWS) Lambda](https://aws.amazon.com/blogs/compute/announcing-c-sharp-support-for-aws-lambda/)
* Configuration and deployment
  * [.NET project structure](https://gist.github.com/davidfowl/ed7564297c61fe9ab814)
  * [Adding Travis CI builds to a .NET Core app](http://andrewlock.net/adding-travis-ci-to-a-net-core-app/)
  * [ASP.NET Core 1.0 - Configure ApplicationInsights](http://social.technet.microsoft.com/wiki/contents/articles/35918.asp-net-core-1-0-configure-applicationinsights.aspx)
  * [haproxy, nginx, Angular 2, ASP.NET Core, Redis and Docker](http://tattoocoder.azurewebsites.net/legion-of-heroes-haproxy-nginx-angular2-aspnetcore-redis-docker/)
  * [Project.json to MSBuild conversion guide](http://www.natemcmaster.com/blog/2017/01/19/project-json-to-csproj/)
  * [Publishing a .NET project with Appveyor and NuGet](https://few-lines-of-code.blogspot.com/2016/03/publishing-net-project-with-appveyor.html)
  * [The New Configuration Model in ASP.NET Core](http://developer.telerik.com/featured/new-configuration-model-asp-net-core/)
* Entity Framework Core
  * [.NET Core Data Access](https://blogs.msdn.microsoft.com/dotnet/2016/11/09/net-core-data-access/)
  * [A very good example about EF Core](https://github.com/rowanmiller/Demo-EFCore)
* Miraculous
  * [Getting started with Orchard Core as a NuGet package](http://www.ideliverable.com/blog/getting-started-with-orchard-core-as-a-nuget-package)
  * [How to export HTML to PDF in ASP.NET Core](https://code.msdn.microsoft.com/How-to-export-HTML-to-PDF-c5afd0ce)
  * [Vue.js server side rendering with ASP.NET Core](http://mgyongyosi.com/2016/Vuejs-server-side-rendering-with-aspnet-core/)
* Security
  * [.NET Continuous Delivery Microservices](http://stackshare.io/tomstaijen/net-continuous-delivery-microservices)
  * [ASP.NET Core 2.0 Authentication and Authorization System Demystified](https://digitalmccullough.com/posts/aspnetcore-auth-system-demystified.html)
  * [A walk-through for an ASP.NET Authorization Lab](https://github.com/blowdart/AspNetAuthorizationWorkshop)
  * [Authentication in ASP.NET Core](https://stormpath.com/blog/authentication-asp-net-core)
* Testing
  * [Selenium with .NET Core](http://www.dotnetcatch.com/2016/11/23/selenium-with-net-core/)

## Books
* [.NET Core in Action](https://manning.com/books/dotnet-core-in-action)
* [ASP.NET Core Application Development: Building an application in four sprints (Developer Reference)](https://www.amazon.com/ASP-NET-Core-Application-Development-application/dp/1509304061)
* [ASP.NET Core in Action](https://www.manning.com/books/asp-dot-net-core-in-action)
* [ASP.NET Core 1.0 High Performance](https://www.amazon.com/ASP-NET-Core-1-0-High-Performance/dp/1785881892)
* [Building Microservices with ASP.NET Core: Develop, Test, and Deploy Cross-Platform Services in the Cloud](https://www.amazon.com/Building-Microservices-ASP-NET-Core-Cross-Platform/dp/1491961732)
* [C# 6 and .NET Core 1.0: Modern Cross-Platform Development](https://www.amazon.com/NET-Core-1-0-Cross-Platform-Development/dp/1785285696)
* [Dependency Injection in .NET Core, 2nd edition](https://www.manning.com/books/dependency-injection-in-dot-net-second-edition)
* [Exploring .NET Core with Microservices, ASP.NET Core, and Entity Framework Core - free eBook sampler](https://www.manning.com/books/exploring-dot-net-core)
* [Microservices in .NET Core: with C#, the Nancy framework, and OWIN middleware](https://www.amazon.com/Microservices-NET-Core-framework-middleware/dp/1617293377)
* [Professional C# 6 and .NET Core 1.0](https://www.amazon.com/Professional-NET-Core-Christian-Nagel/dp/111909660X)
* [The little ASP.NET Core](https://www.recaffeinate.co/book)

## Videos
* [Channel9](https://channel9.msdn.com)
 * [ASP.NET Monsters](https://channel9.msdn.com/Series/aspnetmonsters)
* [Visual Studio](https://www.youtube.com/user/VisualStudio/channels)

## Podcasts
* [.NET Rocks](https://www.dotnetrocks.com)
* [Merge Conflict](http://www.mergeconflict.fm/)
* [The sound of .NET](http://thesoundof.net/?q=.NET+Core)

## Community
* [ASP.NET](https://forums.asp.net)
* [.NET Foundation](http://forums.dotnetfoundation.org)
* [Channel9](https://channel9.msdn.com)
* [Slack](http://tattoocoder.com/aspnet-slack-sign-up)
* Stack Overflow
  *  [.NET Core](https://stackoverflow.com/questions/tagged/.net-core)
  *  [CoreCLR](https://stackoverflow.com/questions/tagged/coreclr)
  *  [ASP.NET Core](https://stackoverflow.com/questions/tagged/asp.net-core)
  *  [ASP.NET Core MVC](https://stackoverflow.com/questions/tagged/asp.net-core-mvc)
  *  [ASP.NET Core 1.0](https://stackoverflow.com/questions/tagged/asp.net-core-1.0)
  *  [Entity Framework Core](https://stackoverflow.com/questions/tagged/entity-framework-core)

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [thangchung](http://weblogs.asp.net/thangchung) has waived all copyright and related or neighboring rights to this work.
