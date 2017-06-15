---
layout: post
title: "(Neo)Vim Bracket Matching Hilighting"
comments: true
description: "A quick solution for a vimmer's pain"
keywords: "vim, neovim, matching parenthesis"
---

Usually, bracket (or parenthesis, etc.) matching in vim is extremely annoying and unreadable because both brackets will have
a different background color, regarding to the rest of the colorscheme. For me this is particularly annoying because i never 
get to know above which one my cursor is.

You can disable the background color change for the matching one like this if you are using a gui :

```
highlight     Cursor                  guifg=black   guibg=white
highlight     MatchParen              guifg=red     guibg=none
```

if you are using a terminal this is pretty much the same thing, just replace **gui** by **cterm**.

I just wish i found this sooner !

Enjoy.
