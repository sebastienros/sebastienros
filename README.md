### Hi, I am Sebastien Ros 👋

I am a software developer in the ASP.NET team at Microsoft. I currently work on [benchmarking ASP.NET Core](https://github.com/aspnet/benchmarks) and [building distributed benchmarking services](https://github.com/dotnet/crank). I also spend some of this time helping the [Orchard Core project](https://github.com/OrchardCMS/OrchardCore) by leading the community and contributing to features.

If I am not working or coding, I am probably 
- sleeping
- doing husband and father duties
- listening to James Taylor
- playing guitar
- biking
- running
- swimming

### Open source

When I don't get paid to code, I still code, mainly on these open source projects:

#### Jint - [https://github.com/sebastienros/jint](https://github.com/sebastienros/jint) 

A JavaScript interpreter for .NET, which allows to run standard scripts in any .NET application. If you need to add some scripting capabilities to your apps, to build a rules engine, or evaluate configurable predicates, you should use it. It's fast and standard compliant. 

The first version of this project started at a previous job, where we needed to send email compains, and we wanted to customize these emails using templates. We followed the way Razor was working by translating the template into pure code, but decided that JavaScript would be easier than C# for editors. A few years ago I decided to rewrite it from scratch following the ECMAScript specs. The first week I joined Microsoft I was asked to show a prototype to Scott Guthrie of "jQuery on the server" which I had built with it, that was fun!

#### YesSQL - [https://github.com/sebastienros/yessql](https://github.com/sebastienros/yessql) 

A NoSQL-like document database layer for .NET that works on existing RDBMS like SQL Server, PostgresQL, Sqlite, MySQL. It allows to store documents and define materialized indexes you can query on using SQL directly. Because it's using the database system you want, you can reuse your existing knowledge, and also use custom SQL queries when you need to optimize for performance.

The idea of the project came to me while working on the first version of Orchard CMS, where we would have to split entities in many tables, which was impacting perf a lot. A CMS usually fits a document based approach, with denormalized data. However using brand new NoSQL databases is often an issue in terms of vendor lock-in, or lack of experience on these systems. RavenDB paved the way in .NET, and I thought we could definitely provide similar features using an RDBMS. Now YesSQL is the standard way to store content in Orchard Core.

#### Fluid - [https://github.com/sebastienros/fluid](https://github.com/sebastienros/fluid) 

A Liquid template engine. Liquid is a templating language created by Shopify and used in other places like Jekyll. This can be used to provide a safe way for users to author templates. It also contains an MVC view engines where files like `index.liquid` will be used automacically for MVC Views.

This project was created for [Orchard Core](https://github.com/OrchardCMS/OrchardCore) in order to enable users to create safe templates, and faster cold rendering of templates. The issue with Razor for content editors is that it's not safe, as it allows to access anything that C# allows, including reading the whole filesystem, and it is also slower to render a template the first time as it requires compilation. Fluid solves these two issues and now used in other .NET CMSes. Initially I tried to use [dotLiquid](http://dotliquidmarkup.org/) but was faced with performance issues as it is using regular expressions to parse the templates.

#### Esprima.NET - [https://github.com/sebastienros/esprima-dotnet](https://github.com/sebastienros/esprima-dotnet) 

Is it a fully compliant ECMAScript parser for .NET. It allows to parse and manipulate JavaScript files, either for executing them, minifying, linting, finding bugs, ... It's use in [Jint](https://github.com/sebastienros/jint).

When I started rewriting [Jint](https://github.com/sebastienros/jint) I followed an advice that [Atif Aziz](https://github.com/atifaziz) made on the previous version, and made the parser a separate library to Jint. The project is mainly a port of the JavaScript implementation named [Esprima](https://esprima.org) created by [Ariya Hidayat](https://github.com/ariya).

#### Shortcodes - [https://github.com/sebastienros/shortcodes](https://github.com/sebastienros/shortcodes) 

A .NET library to parse and evaluate [shortcodes](https://wordpress.com/support/shortcodes/). It allows text content editors to inject specialized content blocks using custom arguments, like images, twitter embeds, youtube videos, only with simple blocks like `[video 123]`.

Shortcodes are essential to WordPress, and for the [Orchard Core](https://github.com/OrchardCMS/OrchardCore) we wanted a similar feature. The parser was written by hand as the syntax is simple and it needs to be efficient.

### More about myself

#### Personal life

I am French, married and father of two. I joined Microsoft in 2010 and live in Bellevue WA (US). 

#### My current bikes (we never have enough bikes)

- Specialized Diverge Comp, mostly for commuting now.
- Specialized Roubaix Expert Di2, for long/group rides.
- Specialized Stump Jumper, for mountain biking.
- Canyon Speedmax Cf 8.0 Di2, for triathlons.

[My stava profile](https://www.strava.com/athletes/8834137)

#### My current guitars (we never have enough guitars)

- Taylor 214ce
- Yamaha SLG200S Silent Guitar

#### My current running gear (one pair is enough)

- Nike Pegasus Turbo 2
- Balega Hidden Comfort Running Socks
