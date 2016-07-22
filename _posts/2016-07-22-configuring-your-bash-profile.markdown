---
layout: post
title:  "Configuring your .bash_profile"
date:   2016-07-22
<!-- categories: development -->
---


# Configuring your bash profile for some sort of productivity :)


## So what’s Bash?

Bash is a Unix shell and command language that was first released in 1989. It’s the default shell on OS X so I guess that’s why I use it  – you’ll use it to run scripts that deploy your code, with git, and to navigate your file system etc.

Over time you’ll get frustrated with the long form of commands that you’re using all the time, so it’s a great idea to add some aliases to a dotfile (what is a DF?) called .bash_profile. So let’s do that.

## Setting up your own Bash Profile

You can do a search on github to get some great examples of the types of things people add. I’m just going to add the things I need right now, but once you know how to do this – you’ll be able to iteratively build up your bash profile so that using the CLI is a lot faster.

So first up let’s make sure you don’t yet have a bash profile. In the terminal navigate to your home directory ` cd ~`. 

Now let’s list all of the files that sit in that location, `ls` will show your files and folders minus your dot files (or config files) so run `ls -a` to see everything – now you should see all your system level configuration files, if there’s no .bash_profile, we’ll create one:

`touch .bash_profile`

run `ls -a` to make sure it’s there, if so, let’s open it `open .bash_profile` – this will open it with your default text editor. Simply add all the aliases you want to be able to use when in the terminal.

For example: `alias gs=‘git status’`

When you run gs in the terminal after you’ve saved this to your bash profile, it will be interpreted as the git status command. I’ve uploaded my bash profile config to github so that I can simply clone that file whenever I need to set it up on my machine again. 

Let’s set up git, commit that file and push it up to github:
* Run:
– `git init`
– `git status`
* Find the file you need to stage ie. .bash_profile and stage it `git add .bash_profile`
* Commit your file `git commit -m “First commit”`
* Set the origin upstream for where you want to push that file `git remote add origin https://github.com/MelissaKaulfuss/.bash_profile.git`
* Now commit it `git push origin master`

Now when you restart your terminal you’ll now be able to run heavily used commands with fewer keystrokes –– FTW!

Here’s a link to mine on [github](https://github.com/MelissaKaulfuss/.bash_profile) –– I expect these to change dramatically over the coming weeks, months and years!
