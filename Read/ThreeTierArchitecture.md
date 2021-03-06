﻿        In a C# application. 3-tier architecture is a very famous and well known buzzword in the world of software development. If we analyze any traditional project then we will find that most of (at least 60-70%) them have traditional N-tier, basically 3-tier architecture. It does not matter whether it is a web or Windows application, we can implement 3-tier architecture in any type of environment.

        Although it is a very well known and common architecture, it's not very clear to beginner developers or those who are very new in project development.

        Why 3-Tier Architecture?

        Still I can remember that, the first organization in my career was dealing with one small Point of Sales (POS) project. It was a Windows application and there was no layered architecture. We developers started to write all code in the Windows Forms Application. The problem started after a few days. How? When our manager announced that we need to develop one web version of the same product. Again we started to develop web pages from scratch and started to write all code. A total mess.

        So, this is the problem and the solution is tierd architecture. If we separate our code by layers then changes in one layer will not affect another very much. Tomorrow if the business demands, we can change the UI very quickly by using existing code.

        Difference between tier and layer

        It is a confusing question for beginners. A few think that both are the same. But they are not the same. Tier represents multiple hardware boxes. In other words the components are physically separated into multiple machines. But in the case of layers all components are in the same system.

        What are the Layers?

        Theoretically it is N-tier architecture. So, we can create as many layers as possible but basically people classify code in three categories and put them in three layers. So, for this article we will consider N-tier architecture as 3-tier architecture and try to implement one sample application.

        Let's explain each and every layer first.

        Presentation Layer/ UI Layer

        This is the top-most layer of the application where the user performs their activity. Let's take the example of any application where the user needs to fill up a form. This form is nothing but the Presentation Layer. In Windows applications Windows Forms are the Presentation Layer and in web applications the web form belongs to the Presentation Layer. Basically the user's input validation and rule processing is done in this layer.

        Business Layer

        This is on top of the Presentation Layer. As the name suggests, most of the business operations are performed here. For example, after collecting form data we want to validate them with our custom business rule. Basically we define classes and business entities in this layer.

        Data Access Layer

        On top of the Business Logic Layer is the Data Access Layer. It contains methods that help the business layer to connect with the database and perform CRUD operations. Generally all database related code and stuff belongs to the Data Access Layer. Sometimes people use a platform-independent Data Access Layer to fetch data from various database vendors.