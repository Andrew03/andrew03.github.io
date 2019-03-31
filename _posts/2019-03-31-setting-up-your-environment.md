---
layout: post
title: Setting Up Your Programming Environment
subtitle: How to set up something that looks nice and works well!
tags: [vim, tmux, coding-environment]
comments: true
---

# What is this?
This environment is designed to make programming in your terminal window a pleasure rather
than a pain. As a college student, I know tnat there are plenty of people who prefer using
IDE's nowadays, especially since IDE's have begun to support ssh'ing into machines, one of
the few times that programming through the terminal was necessary. There's a lot of stuff
out on the internet about how people like to program, but personally I prefer to use my
terminal over an IDE. However, without a few of the additions I've made over the years, I'm
sure I would have found programming in my terminal almost intolerable. This post will outline
a few of the additions I've made, and also show you how I set up my environment on a new machine.

![Environment](https://github.com/Andrew03/Environment-Setup/raw/master/imgs/environment_screenshot.png)

## What I use

### Vim
Vim, in essence, is just a text editor; you can think of it as Notepad on steroids. The main
thing people seem to like about Vim is how efficient it is. Since you can accomplish an array 
of tasks without ever moving your hands off your keyboard, you eliminate the need to use a mouse.
Also, you have shortcuts for just about anything you'd want to do. I personally enable mouse usage
in Vim, but I definitely make use of the shortcuts. To be honest, I've become a little reliant on 
Vim; whenever I'm doing an online coding interview, Vim is one of the first things I turn on if 
the IDE allows it, and I feel like I don't think as well if I cant't use Vim. If you want to learn more
about Vim, type `vimtutor` into your terminal to go through a tutorial, or just look it up online.

### Tmux
Tmux is a screen multiplexer. Yeah, I don't really know what that means either. What I do know is
that it allows me to split my terminal window into multiple panes so I can easily edit multiple files, 
look at debugger output, and switch through different projects, all at once. Something that's especially
important for me as someone who does work in deep learning is that I can connect to a server, start a job,
disconnect from the server, and reconnecting to the server later without any impact to my job. So, I can 
run jobs for hours, or days on end, which is fairly normal when it comes to training models. There's plenty
of information on Tmux online along with the regular commands, but I added in a few more that I found
easier to remember.

### Powerline
Powerline is a statusline plugin. Essentially, it makes your terminal window look nice by improving your 
Bash, Vim, and Tmux prompts. Rather than just plain-text, you get color, arrows, and additional information
if you want it such as virtual environment and GitHub branch.

### Solarized
Solarized is the main theme that I use in my programming environment. It has a nice color scheme,
especially when it comes to dark mode. It's probably the main difference between the programming
environment above, and the one you have.

## The Actual Setup
I have a GitHub repository [here](https://github.com/Andrew03/Environment-Setup) that makes it really
easy to get my exact environment. All you have to do is follow the commands there, and then you'll
have the same environment as me! Unfortunately, my setup does currently only work on Linux and Mac,
with the caveat that it doesn't work on Mojave yet (there's an issue with Powerline and Mjoave that 
hasn't been resolved yet).
