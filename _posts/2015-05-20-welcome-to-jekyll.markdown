---
layout: post
title:  "Building a blog with Jekyll"
date:   2015-05-20 16:40:37
categories: development
---
For ever I've been thinking, I need to write a blog. Honestly, I think that if I can learn to talk about what I'm learning then it will help cement things in my mind a little better.

Truthfully though, I've been muddling through this project with no idea what's going on. Initially, Jekyll seems pretty simple. To start your project you'll need to install a few things, you'll need Ruby, you'll need to install the Jekyll gem and you'll need true grit.

I have never really worked on anything IRL. So, this is tough, unpacking such a huge project with so many files and styles was a huge effort. But I found it was a great way to learn how to dive into an existing codebase and really begin to understand what was happening slowly. I learnt a lot.

I finally managed to rip out some of the things I didn't need and did some _very_ basic styling, all within the limits of my understanding – which I should add is pretty shit and almost non-existant.

I decided to deploy to github pages I pushed it and realise my styles were all seriously borked. My SVG icons were full screen! After flipping the table I set about trying to work out why. Turns out that I failed to change my baseurl to "/my_project", simple as that. So it was trying to load the CSS from the incorrect path. Anyways, I fixed it, and pushed but the change wasn't reflected. Lea Verou saved the day with her post <a href="http://lea.verou.me/2011/10/easily-keep-gh-pages-in-sync-with-master/">easily keep gh pages in sync with master</a>.

Never forget to run the following commands:

- git checkout gh-pages

- git push origin gh-pages

- git checkout master


So it's up but now something else is broken and it's bedtime. It can wait until tomorrow.

