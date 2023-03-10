# Version control

## What is it & why do we need it?
Version control, in this context, is a system of methods used in an attempt to manage the versions of one or more libraries/services in a software application.

When I first started, I am aware of this concept. However, I didn't have a reason to use it until a series of bugs rained upon me when my 3rd & 4th project comes along.
Let's just say we all started the same way, we learned a new programming language when we get into this field, and we installed a compiler or engine on our machine (be it your own or one your company provides). You will never run into any problems with your first project. But when the second project comes in and it requires the same programming language. Things start to become troublesome, here's a list of symptoms that might have encountered:   

 - The package/library installed on your first project collides with your second projects  
 - Your second project requires a different version of the same engine/compiler as your previous ones.  
 - Exporting the installed lib into a package file is a mess because it includes not only your previous project but also the sub-dependencies of that project.  
 - Installing an additional version of your programming language can cause some confusion. Your machine might have trouble finding the correct interpreter/version of your programming language. You have to be a bit more careful when declaring the pathing on your machine.  

What I'm trying to get at is that if we can control the version of the programming language and/or its dependencies, we will run into a lot fewer dependencies collision problems.

> :material-comment-text-outline: **note**  
I admit, I did ran into all 3 problems in the first 2 years when I started working in the field. Initially the problem persists even after I fix them. A series of bugs began to appear, one after another. It's like I can cut the stem but the root remain. At the time I thought I was already exploring uncharted territory since I was the only one having that problem.   
I still ran into this problem until I start to use docker. As you may or may not know, docker container is a tool that allow you to isolate environment for your software. This is the core component of any microservice architecture. It's similar to a virtual machine, isolated, separated and perfectly clean of unused packages.   
Once I discovered docker, I used it pretty much anytime I can, from creating a development environment with a docker container and terminal into it with an IDE. Lots of fun, but also clunky and inefficient. 
---

Package Manager:
A package manager is a tool that helps developers manage dependencies and packages for their projects. Popular package managers for different programming languages include npm for Node.js, pip for Python, and RubyGems for Ruby.

With a package manager, developers can easily install, update, and remove packages and dependencies for their projects. This helps ensure that the project remains up-to-date with the latest versions of packages and dependencies and reduces the risk of compatibility issues. Additionally, package managers often include features such as package discovery, version tracking, and dependency resolution to help developers work more efficiently and effectively.

## How should we do it?
> :material-comment-text-outline: **note**  
At the time I write this document, I've only used python and nodejs so I can only refer to those two. But I assume other languages also have similar concepts related to version control. For demonstration purposes, I will choose python as our example. 
---

Currently, there are 3 main types of operating systems out there: Linux, MacOS & Windows. Each might have a different set of tools that we for version control, however, the core concepts should be the same:  

 - Version manager (manage version of your programming language)  
 - Package manager (manage the library/packages and its version of your project)  
 - Dev/production package  
 - Lockfile  

In python, we have a python version manager and a python package manager. 
In nodejs, we have node version manager and node package manager.
... So on and so forth





