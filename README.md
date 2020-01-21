The CCM (C# Collections Mapper) is a working version of the handwritten mini ORM, working with the database and C # collections. Productivity is quite high, resource consumption is minimal. This ORM works directly with SQL Server stored procedures. The code is accompanied by descriptions and example .Net Console project showing the technique of ORM using.

Data is stored on the SQL server and when a large number of simultaneously connected users access it this creates a serious load on the database server. In addition, often database queries fetch the same data, which is not good in terms of server and applications load. One of ways to optimize the database in ligament with client application is to reduce traffic and to store data already received from the server on the client or in the middle application tier. Or to store already received data on the application server, especially when the database server and client applications are distributed across the network. For this purpose, the collections stored in the Session or at the application level are the best suited.

Below is a solution for the data management layer in the combination of MS Sql Server with a C # application. In whole this is a strongly typed entity mapper projecting the application's business logics onto database tables using T-SQL stored procedures. In this realiasation of ORM the tables, procedures, and entity constructors are written by hand. They are not generated automatically by a mapper. 

At the same time, the entity code and stored procedures can be minimased and simplified and fully controll by the developer. As well as a process of data obtaining.
All client code is reduced to writing the simplest one string calls to the mappers methods and to creating the simplest constructors for entities by template.

CCM allows you to implement fairly complex data structures in your application, without bothering about difficult and tedious questions of data acquisition and conversion issue, allowing you to pay more attention to the develop of business logic and UI. There no need to worry about migrations, context, etc. At the same time, ORM completely relieves the developer from direct communicating with ADO - datasets, tables,  rows, and other data aceess component, to track connections, commands or operate with adapters because ORM works at a higher level of data abstraction. At the same time you will be completely protected from memory leaks and free to create complexity application logic at the primary data level. 

How to say thanks? 

The application is free to download and is distributed under the terms of the MIT license. Don't forget to thanks to developer using the Donate link at this page http://prozarium.ru/TextDetails.aspx?TextID=1410

Please read License Agreement for details of using CCM in your projects.

(c)2010-2020 Eugene Trifonov, 
aka p.v.(pterodactilus vulgaris)
Saint Petersburg, Russia
mailto: pterodactilus@rambler.ru
Skype prozarium
Telegram @EugeneTrifonov

I'm looking for remote work on C#, ASP.Net, MS SQL. 
CV is here https://spb.hh.ru/resume/78cedb6fff01b150c00039ed1f434c364b7257
Feel free to make an offer that is hard to refuse
