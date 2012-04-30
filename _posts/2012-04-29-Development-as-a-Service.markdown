--- 
layout: post
title: "Development as a Service on its baby steps" 
date: Sun Apr 29 20:26:09 +0200 2012
---

Let me start by presenting a new web service [pythonanywhere.com](http://www.pythonanywhere.com/).

It's a full python development stack, ready to be used in your browser. After a quick subscription for a free account,
you have access from your dashboard to [python, ipython,  bash] consoles in different python flavours. 

You can also browse your files, make cron scripts and create python web apps on the fly.

The most interesting features are the consoles pause/resume feature, which can be shared 
with other people. This could be very helpful to collaborate on code or teach python.
Behind the scene, it's an encrypted ajax window over your home folder running on a remote server hosted on EC2.

DaaS may be on it's first baby steps. Though, it could rapidly become a standard way to code for developers especially in startups.
Before diving in the pros and cons, let's analyse the different development stacks possibilities. 

First, there's the good old fashion way. Setup a server on a cloud service 
(I guess there's still people doing it with bare metal servers ). You have plenty of choice there, (EC2, AppEngine, Azure, Rackspace...), 
it depends on your IT needs, spiritual beliefs (many don't care) and your pockets. 

Then pick the development stack of your preferred language/framework: Python(Django, Web2py, Pylons, Flask...), Ruby(Ruby On Rails) for the rock stars, Java/.Net, PHP ... 

Here, you have to maintain every piece involved in the process, packages versions, build tools, deployment, scaling. That's a lot of time and resources needed to finally get your developers pushing and your apps running.

The next big step was the [Heroku](www.heroku.com) and [ Dotcloud ]( www.dotcloud.com ) like services, aka Deployment/Scaling as a Service. 
They release from the burden of deploying and give enough abstraction to exclusively focus your effort on the application logic. 
The process is often the same, basically setup your project with a simple conf file, then deploy to the server with one command. 
They practically all handle version control systems like git,
so your project is deployed every time you push your code. 
I believe Github helped a lot making these services exist as deployment is often tightly bound to code revisions, it offers an excellent API and a huge community.


We have been adding more and more abstraction to the development process in order to make it easier, faster, stronger ... 
However, there is still one constant, "localhost development". The coding itself is done on your machine/laptop.You still can use your favourite OS, IDE, tools. 

Well, DaaS is going to cross that last barrier. 
There are already several web services for online development like [jsfiddle.net](jsfiddle.net) for web design or [koding.com](koding.com).
They offer something that could change the way we see development, the abstraction of your OS, ide and development environment. 
If you think about it, that's a lot of time saved. No multi-platform mess, no more scripts to ensure the same development stack. Using the enormous processing power
of cloud platforms, there is virtually no compile time. You can even forget about your machine, all you need is a keyboard and a screen.

It seems only benefit but the thing is, if DaaS is really going to be the next step,I think we are missing something very important. 
Before a developer learns to code, he has 
to understand the building blocks of programming, what's a computer, what's an Operating System, how does it do its work. All the abstractions we built are built 
using this knowledge. How could a programmer understand code optimization ? Security flows? 
How could he understand the interaction of his code with its environment if he's not gonna use it? 
Maybe we're not concreted with that yet, but the next generations of programmers are. 


What do you think ?
