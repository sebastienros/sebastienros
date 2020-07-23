### Hi, I am Sebastien Ros 👋

I am a software developer in the ASP.NET team at Microsoft. I currently work on [benchmarking ASP.NET Core](https://github.com/aspnet/benchmarks) and [building distributed benchmarking services](https://github.com/dotnet/crank). I also spend some of this time helping the [Orchard Core project](https://github.com/OrchardCMS/OrchardCore) by leading the community and contributing to features.

If I am not working or coding for fun, I am probably 
- sleeping
- doing husband and father duties
- listening to James Taylor
- playing guitar
- biking
- running
- swimming

[My stava profile](https://www.strava.com/athletes/8834137)

#### My current bikes (we never have enough bikes)

- Specialized Diverge Comp, mostly for commuting now.
- Specialized Roubaix Expert Di2, for long/group rides.
- Specialized Stump Jumper, for mountain biking.
- Canyon Speedmax Cf 8.0 Di2, for triathlons.

#### My current guitars (we never have enough guitars)

- Taylor 214ce
- Yamaha SLG200S Silent Guitar

#### My current running gear (one pair is enough)

- Nike Pegasus Turbo 2
- Balega Hidden Comfort Running Socks

### Open source

When I don't get paid to code, I still code, mainly on these open source projects:

#### Jint - [https://github.com/sebastienros/jint](https://github.com/sebastienros/jint) 

A JavaScript interpreter for .NET, which allows to run standard scripts in any .NET application. If you need to add some scripting capabilities to your apps, to build a rules engine, or evaluate configurable predicates, you should use it. It's fast and standard compliant. 

The first version of this project started at a previous job, where we needed to send email compains, and we wanted to customize these emails using templates. We followed the way Razor was working by translating the template into pure code, but decided that JavaScript would be easier than C# for editors. A few years ago I decided to rewrite it from scratch following the ECMAScript specs. The first week I joined Microsoft I was asked to show a prototype to Scott Guthrie of "jQuery on the server" which I had built with it, that was fun!

#### YesSQL - [https://github.com/sebastienros/yessql](https://github.com/sebastienros/yessql) 

A NoSQL-like document database layer for .NET that works on existing RDBMS like SQL Server, PostgresQL, Sqlite, MySQL. It allows to store documents and define materialized indexes you can query on using SQL directly. Because it's using the database system you want, you can reuse your existing knowledge, and also use custom SQL queries when you need to optimize for performance.

The idea of the project came to me while working on the first version of Orchard CMS, where we would have to split entities in many tables, which was impacting perf a lot. A CMS usually fits a document based approach, with denormalized data. However using brand new NoSQL databases is often an issue in terms of vendor lock-in, or lack of experience on these systems. RavenDB paved the way in .NET, and I thought we could definitely provide similar features using an RDBMS. Now YesSQL is the standard way to store content in Orchard Core.
