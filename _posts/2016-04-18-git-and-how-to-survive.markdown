---
layout: post
title:  "how to git and survive – part I"
date:   2016-04-18 22:54:00
---
On Friday afternoon I embarked on my new profile site. A project I've really taken to. It's been great exploring CSS and using Flexbox, Media queries and having fun with layout and typography.

I felt as though I'd reached the limits (fairly quickly) of what you could feasibly do with a static site, and after copying and pasting my Nav HTML into 3 .html files I realised I needed to tackle a templating framework. I've decided to look at Sinatra – because Ruby.

I set about trying to read the documentation – which naturally omits all the things a n00b needs to really get started. So, after messing up my project with some half implemented features I thought I'd like to park it so that the evidence was gone for a bit.

That's when I learn't about `git stash` *head explode moment!*

So when using `git stash` you can literally stash any uncommitted work in the bottom drawer for later. And when you want it, you can rumage about and include it back into your project.

I ran into some issues when the command didn't want to work as expected, I kept running into the old `Your branch is up to date with origin/master` yet when running `git stash show` there was `no stash found`. I first thought it was because my changed files were staged, so I unstaged them with `git reset HEAD .` But still no joy :'(

I then resorted to bugging people on Twitter and thanks to @willrax I discovered that if the files haven’t been committed yet `git stash save -u` should catch them and it did! Win – I now have a working directory sans the half baked Sinatra implementation. I now have a neat and tidy stash in the bottom drawer that I can forget about for a bit.

To check out what's in there with the sticky tape, scissors and birthday candles run `$ git stash list`.

To restore and include the most recent stash into your project tree run `git stash apply`.
To include one of the older stashes, simply specify which one like this `it stash apply stash@{2}`

You can read all about stashing on the <a href="https://git-scm.com/book/no-nb/v1/Git-Tools-Stashing">Git site </a>.







