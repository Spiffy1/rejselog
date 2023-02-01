# Version control

## What is it & why do we need it?
Version control, in essence, is a system of methods used in an attempt to manage the versions of one or more library/service in a software application.

When I first started, I am aware of this concept. However, I didn't have a reason to use it until a series of bugs rain upon me until my 3rd & 4th projects come along.
Let's just say we all started the same way, we learned a new programming language when we get into this field, we installed a compiler or engine on our machine (be it your own or one your company provide). You will never run into any problem on your first project. But when the second project come in and it requires the same programming language. Things start to become trouble some, here's a list of symptom that might have encountered:   

 - The package/library installed on your first project collide with your second projects  
 - Your second project requires a different version of the same engine/compiler to your previous ones.  
 - Exporting the installed lib into a package file is a mess because it includes not only your previous project but also the subdependencies of that project.  
 - Installing an additional version of your programming language can cause confusion some confusion. You machine might have trouble finding the the correct interpreter/version of your programming language. You have to be a bit more careful when declaring the pathing on your machine.  

What I'm trying to get at is that if we can control the version of the programming language and/or its dependencies, we will run into a lot less dependencies collision problems.

> :material-comment-text-outline: **note**  
I admit, I did ran into all 3 problems in the first 2 years when I started working in the field. Initially the problem persists even after I fix them. A series of bugs began to appear, one after another. It's like I can cut the stem but the root remain. At the time I thought I was already exploring uncharted territory since I was the only one having that problem.   
I still ran into this problem until I start to use docker. As you may or may not know, docker container is a tool that allow you to isolate environment for your software. This is the core component of any microservice architecture. It's similar to a virtual machine, isolated, separated and perfectly clean of unused packages.   
Once I discovered docker, I used it pretty much anytime I can, from creating a development environment with a docker container and terminal into it with an IDE. Lots of fun, but also clunky and inefficient. 
---



## How should we do it?


> :material-comment-text-outline: **note**  
At the time I write this document, I've only used python and nodejs so I can only make reference to those two. But I assume other language also have similar concept related to version control. For demonstration purpose, I will choose python as our example. 
---

Currently there are 3 main type of operating systems out there: Linux, MacOS & Windows. Each might have different set of tools that we for version control, however, the core concepts should be the same:  

 - Version manager (manage versioning of your programming language)  
 - Package manager (manage the library/packages and its version of your project)  
 - Dev/production package  
 - Lockfile  

In python we have python version manager and python package manager. 
In nodejs we have node version manager and node package manager.
... So on and so forth





