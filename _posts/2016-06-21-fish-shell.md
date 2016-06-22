---
layout: post
title: "Fish Shell"
comments: true
description: "fish, a very cool shell !"
keywords: "Bash, Zsh, Fish, oh-my-zsh, oh-my-fish, shell, terminal"
---

#### Bash

When i started using linux (circa 2006) i was using the default shell, bash. It works pretty fine but 
seriously lacks of ease of use (completion, syntax highlighting, hints and so on).

#### Zsh and oh-my-zsh

Three years ago i discovered Zsh. It has some great features bash doesn't have such as a way better completion and the ability of 
completion based on jokers, for example :

```bash
ls D*
```
Pressing tab, the command will become something like 

```bash
ls Desktop Documents Downloads
```
I immediately found this very handful.

Also, the ability to add plug-ins (keyboard movements for completion, git state in the prompt, etc.) and themes is really great.

However i found that zsh (especially when used with oh-my-zsh) was pretty laggy and slow. This conducted me to recently look 
for something better.

#### Fish

![fish_shell](/images/fish_shell.png)

I switched to fish this week. A lot of features of zsh requiring oh-my-zsh work natively in fish, plus very sweet ones like :

* syntax hilightning
* paginated completion
* options completion
* etc.

![fish shell](/images/fish_mat.png)

Besides, i find it way faster than zsh.

The package manager, oh-my-fish (pretty much like pip for python or apt-get) enables you to install a wide variety of plug-ins and themes.

More information on [fishshell.com](https://fishshell.com/) and [oh-my-fish page](https://github.com/oh-my-fish/oh-my-fish)

This is my favorite shell so far and i highly recommend it to you ! :^)
