# Introduction #

<!--TOC-->


This document aims to explain how I came to writing an open source software. The reasons are multitude and very interesting. It is a non technical document about my history.
For short, the main reason for creating an open source project was that I had the benefit to use other open source projects. I understood the value in it and decided to make my project open source as well. The reason starting my own framework and stuff has to do with companies that potentially drop their products - or they have a live cycle that will end at a given time. I probably also have a problem to keep pace with that live cycle and rather stick to an older product for a longer time.
I will extend this document from time to time and fill it up with my history.

Lothar Behrens - Saturday, 20.10.2024



----

# Early days in computing #

My first computer was one that I have bought at the start of my education. It was an IBM PC compatible computer having only 512 KB of RAM - at that time well enough RAM. It was MS DOS and GEM only at that days. While in my education I grabbed every book I could and read through it learning the ins and outs of computers.

I learned programming with Basic (really at my aunt’s C64 home computer and I realized very early at my education that there are better languages than Basic. Thus I have never done anything with my Schneider PC Basic2 (Locomotive Software).


![][PastedGraphic]
This is the Basic2 programming environment on my Schneider PC 1512 within GEM

----

# Starting with programming #

As I told, I had purchased my first computer at or short before my education, I quickly stumbled upon an object oriented language. It appealed me more than Basic and I did my next purchase. In my education, Basic was the language we learned and I was most of the time ready before the rest. That was probably because I learned Basic on the C64 and it was similar to GWBasic I think it was.

----

# My first software ideas #

As soon as I had Turbo Pascal I also had my first ideas for a software. While my education, I had collected many diskettes and it seemed to be complicated to keep notes on paper or only on the stickers to know, what is on these diskettes.

I started to write ‚dateiver‘ - a disk cataloging system. It had only a command line UI. Even today there exists many command line tools and on Linux there are many that also work together and are very helpful. But my application was a standalone application not designed to work with other applications together.

![][Dateiver]
Dateiver console application within Turbo Pascal 6.0

As you may notice, the folder is named differently. At that time I didn’t structure my source code well and that leads to struggle as well. Dateiver was copied over for a new application - Tvvt.

At that time I also learned much about programming data structures and I needed them in my disk cataloging system. Databases where not known to me at that time - I would have not learned data structures so early. Also I learned how to store and load the collected data and also to traverse a file system to read in the data from a disk.



----

# A first attempt for a customer #

After my education my first customer came to appear by contacts asking me if I could do what the customer wants to do. I contacted the customer and negotiated what the software should do and what I could start with as a first attempt.

After a.while of work I have presented the first solution. The customer was not satisfied about the software I had presented. The UI still was a console based one and that looked not appealing to the customer. I was a bloody beginner and failed…

----

# The professionals use SAA #

Later, when I tried to market Dateiver as a shareware version, I got told that this application would not win a price. It was lacking a modern UI and thus the software dealer I contacted, was not appealed about it to put that in his store. I learned that as well with my customer and there seems to be more than this one picky customer not wanting to work on console. The shareware seller told me that I could have a look at that fancy SAA UI and I did so and learned.

I had to buy another compiler version and needed to migrate my software from Turbo Pascal 5.5 to 6.0 to be able to utilize that new fancy SAA UI toolkit.


----

# My first model driven ideas #

After learning SAA and modern UI in that days, I learned to know a dialog designer from a book. It should help me in software creation. Quickly I found that I would do more like that and created my own first way to produce software without typing code. TVBuild was my first attempt for a model driven application development environment.

![][TVBuild]

TVBuild - an attempt to produce code by an application that offers me menus and dialogs.

----

# After Pascal came Windows and C++ #

The time goes and I had to buy a more modern computer. While the first purchase after my Schneider PC was for a followup school and thus a notebook - it indeed was a sub notebook - one of the first DIN A 5 format notebooks that looked so cute. It still was a MS DOS only machine and I had to go further, I had made a decision to buy into a new tower 386 DX 40 PC with Windows 3.1 and a whooping 4 MB of RAM. With that PC I also shortly have purchased one of the fastest compilers available at that time - known to be used by Doom - a game. It was Watcom 10.6.

![][Bildschirmfoto2024-10-20um105545]
The Watcom IDE with a splash screen

Using that compiler, I learned C++ and Windows programming. I started with simple C API but moved fast into object oriented programming and started using MFC. There I still didn’t started with database programming and repeated my experiences with data structures using MFC and Drawcli as a base for my own application I started to write for a model railroad club that also had activities in riding real steam locomotives and old trains to take those people wanting to sit in old trains getting some coal smoke	 into the face.

----

# Trainres and the journey through MFC #

With the new compiler and with some help from some club team mates I wrote a train reservation system - or more, I tried too. There was a stakeholder wanting fancy diagrams of the ride like those maps shown on train stations - in a shrinked down version though. At that time in 16 Bit Windows 3.1 on my 386 DX 40.

![][Bildschirmfoto2024-10-20um111447]
Train - A windows application written using MFC

At that time I went far with my knowledge - I thought - and was eager to further develop that application for the club. In the screenshot you see a net list with some red colored lines and one without. The colored ones represent the entry of two train ride plans shown on the right middle screen. The application reacted upon entering that plan with the drawing of the respective tables to start adding ride time schedules below the header. That was the plan.

Also the plan was to use that graphical presentation to store data within. As you see a customer was entered into the bottom left window to have been registered for the train ride 001. All made with data structures and the help of the basics of Drawcli.


----

# Trainres the MFC version survived into Windows 10 #

And you see some wonder I come to talk about later. Train survived into the Windows 10 era and can be developed with Visual Studio.

![][Bildschirmfoto2024-10-20um112431]
Train in Visual Studio 2022

![][Bildschirmfoto2024-10-20um112746]
And Train on Windows 10

----

# Starting to learn databases #

After a while using Watcom 10.6 and MFC I got notice of a much fancier development tool than Watcom. It was Power++ from Powersoft. Powersoft purchased Watcom and it’s compiler tools and database stuff I didn’t were aware of yet.

The marketing of Power++ appealed me to look into that tool - as it included my next journey to learn databases within that tool and claimed to be RAD and I could get ready with my application fast.

![][Bildschirmfoto2024-10-20um114925]
Power++ from Sybase


----

# I began porting Train #

When I have purchased Power++ Developer - the smallest version I was capable of buying at that time, I started porting my application I was developing for the club to use the Power++ class library. While doing this I added more time into building my sophisticated diagramming stuff than database, I can now say, I have neglected one of my biggest issue in my career as a professional software developer - I still wasn’t professional.

The diagramming capabilities were interesting, because I have done my own interpreter to let the user design it’s own symbols. While doing so, the stuff was stored within a database and I even had some simple customer entries in my table.

![][Bildschirmfoto2024-10-20um115956]
Trainres - the new application with database and custom interpreter for symbols



----

# After some time Sybase dropped Power++ #

It came to pass that Sybase decided to drop Power++ and I was upset. Not only that I have wasted money, but also my effort into the port was likely some dead cow now. I was really angry and I stopped development of that application immediately. Because it made no sense for me in that stage of the application. The club never got a running application. 

I had to learn hard, that companies don’t really care about their customers - at least those small ones that the company may neglect due to the sales. I never had found out, why they have dropped Power++. There was a final release I didn’t got notice about and recently I found out that the company gave the enterprise version to all registered customers - even with the Developer version only.

After years I had found out that fact. I come back to the Enterprise version later.

At that point in time I had to rethink my way to develop software. It probably was at the announcement or short after that, when I made my rethinking. Also at that time I started learning to cope with Linux - the new thing. I wanted to start also programming there. Experimenting with Linux as a programmer, I looked around what to use as an API or framework to write software with. I started learning to know wxWidgets and other stuff. wxWidgets was most appealing as it was free of charge and I made a decision to use that framework, because I could save time again.

When playing with Linux and Windows in parallel, I figured out that I also wanted to run the application on one machine and using the other as a server speaking together. So, doing client server stuff was the next big thing beside my last client server thing (database) that implicitly was using client server communication.

It was about 1999 and long story short - I started a new project. A project I still work on today…

My project was born - not yet open source. I started trying to create an UI wrapper that I do no longer depend upon UI specific stuff or even UI frameworks. I wanted to include somewhat like CORBA or similar thing, but my own. That was because I have lost my trust into products I purchase and then I go to the next product and that has it’s own framework I probably would use ending up in a rewrite of my application again.

At that time I had a job as a software developer and gained some experience in the area of client server programming and database programming. I also learned to know CVS - a version management system. I learned much at that time jumping into the cold water. All I needed in the future - really worth the experience. I made it from a hobby developer to a professional software developer - yet a beginner - but that is another story.

----

# Starting my open source project #

When I had made some progress with my Windows and Linux trials and my first attempt within my big project goal, I stepped back and thought twice about the goals. I started to realize that it was too big at once. I also realized that the attempt at first would not succeed at the scale I had in my mind.

Nevertheless I proceeded with the project and a full rewrite. Most parts were reusable and I had only to make it compatible to the new design. The snippets are still viewable within the CVS project history. Now, of course, I have made a migration path to Git while keeping that history. That Git migration is part of my current attempt to start over with development after a long break. I was caught into my next show stopper. That was CVS, but that is also another story and only partly related to obsolescence.

To sum it up, why I started an open source project was as follows:

Products provide their own frameworks. These frameworks may be available with other products, but that is no guarantee for no porting effort required. If the product has no common framework, such as MFC (within Watcom and Microsoft Visual C++ onwards I think), you end up using their own frameworks and risk a lock in into that product line. It was not only a lock in (Power++), but also a show stopper at all when Sybase decided to drop that product.

With my own framework, I indeed write another framework and do the same as those companies, but it is at my control. I can keep using it. I can make decisions at my own pace to keep using it and I can still make it available in the public. The project has been started, rewritten, made public and is still in active development at a stable state. I designed it in a way similar to COM or CORBA using pure abstract classes (much more technically), but that is the main decision, I made and why it is still alive.

----

# The current state and why it is still alive #

Today, the project is still alive and that has a reason. The initial design led into a rewrite, but I made that early and fully toward a modular software system. In that early stage, I understood, what COM had demonstrated so far. The building block of COM literally was its interface design technique. The interfaces were designed once and as I think, never changed. If a change was required, it led into a new interface - say, with a trailing number of the version. The next thing I understood, but I have not applied to my version, was a basically as low as C language level based technique of binding things together. Meaning not necessarily requiring object oriented languages. I didn’t followed that path, because I didn’t needed that low level. I kept using C++ and pure abstract classes (interfaces).

I also skipped one goal after starting the project due to it’s sheer size and additional stuff to bring to live. That was the remote API part. I started with local only and didn’t started utilizing the client server API part for my project until now. It kept sleeping in my code base, though.

Why is the project still alive? It is due to the fact, that I am my own stakeholder. I am using it - for software development purposes. One part is of course the cross platform capability to let me use the main application on my Mac OS X, Linux and on Windows of course. The second reason is that the main functionality within that project is a model driven software prototyping approach that let me quickly develop database software prototypes. That important part I have neglected uproot with the migration to Power++ what literally lead to an unfinished product.

Today, I am capable of creating from this UML model (the main application it self) a modern looking application in a completely different software development language and framework.

![][lbDMFManager]
Part of the main UML model for the main application

![][2024-07-0916_35_43-Greenshot]
Main application. In front tne open source wxWidgets prototyper. In back generated DevExpress

----




[PastedGraphic]: PastedGraphic.png

[Dateiver]: Dateiver.png

[TVBuild]: TVBuild.png

[Bildschirmfoto2024-10-20um105545]: Bildschirmfoto2024-10-20um105545.png

[Bildschirmfoto2024-10-20um111447]: Bildschirmfoto2024-10-20um111447.png

[Bildschirmfoto2024-10-20um112431]: Bildschirmfoto2024-10-20um112431.png

[Bildschirmfoto2024-10-20um112746]: Bildschirmfoto2024-10-20um112746.png

[Bildschirmfoto2024-10-20um114925]: Bildschirmfoto2024-10-20um114925.png

[Bildschirmfoto2024-10-20um115956]: Bildschirmfoto2024-10-20um115956.png

[lbDMFManager]: lbDMFManager.png width=1076px height=900px

[2024-07-0916_35_43-Greenshot]: 2024-07-0916_35_43-Greenshot.png width=1440px height=810px