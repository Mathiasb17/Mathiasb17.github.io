---
layout: post
title: "VCSH Config Manager"
comments: true
description: "VCSH is a config manager based on git"
keywords: "VCSH GIT bash zsh fish config manager"
---

I have loads of config files that i absolutely want to save on github so i don't have to write them again. 
Some examples : neovim, i3wm, cmus, irssi, and a lot more.

First i was using git with [my associated github repo](https://github.com/Mathiasb17/mathias), which i found not really convenient
for this kind of task, and i ended up with a mess accidentally (*.git/* in my *$HOME* and this kind of garbage). An horror to maintain
correctly.

Then a friend told me about [vcsh](https://github.com/RichiH/vcsh) so i gave it a try. It is kind of an extension of git to manage your *$HOME*.

It avoids the problems mentioned earlier and does its own work without me worrying, in *$HOME/.config/*.

For example if i want to create a git repo dedicated to my *nvim* and *i3* config files :

```bash
vcsh init configs
vcsh configs add ~/.config/nvim/init.vim
vcsh configs add ~/.config/i3/config
vcsh configs commit -m 'first commit !'
```

It will locally create a repository for those two files, named configs in *$HOME/.config/vcsh/repo.d*.

And then add an origin and push !

Enjoy.

