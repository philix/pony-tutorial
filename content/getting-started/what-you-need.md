---
title: "What You Need"
section: "Getting Started"
menu:
  toc:
    parent: "getting-started"
    weight: 5
toc: true
---
To get started, you'll need a text editor and the [ponyc](https://github.com/ponylang/ponyc) compiler. Or if you are on a not supported platform or don't want to install the compiler you can use the [Pony's Playground](https://playground.ponylang.io/).

## The Pony compiler

Before you get started, please check out the [installation instructions](https://github.com/ponylang/ponyc/blob/master/README.md#installation) for the Pony compiler.

## A text editor

While you can write code using any editor, it's nice to use one with some support for the language. Here are some:

* [Sublime Text](http://www.sublimetext.com/). There's a [Pony Language](https://packagecontrol.io/packages/Pony%20Language) package.
* [Atom](https://atom.io/). There's a [language-pony](https://atom.io/packages/language-pony) package.
* [Emacs](https://www.gnu.org/software/emacs/emacs.html). There's a [ponylang-mode](https://github.com/ponylang/ponylang-mode).
* [Vim](http://www.vim.org). There's a [ pony-vim-syntax](https://github.com/dleonard0/pony-vim-syntax) plugin. Install `pony` with `vim-plug` or `pathogen`.
* [Microsoft Visual Studio](http://www.visualstudio.com/). There's a [VS-pony](https://github.com/CausalityLtd/VS-pony) plugin.
* [BBEdit](http://www.barebones.com/products/bbedit/). There's a [bbedit-pony](https://github.com/TheMue/bbedit-pony) module.
* [Microsoft Visual Studio Code](https://code.visualstudio.com/). There's a [Pony Language Colorizer](https://marketplace.visualstudio.com/items?itemName=npruehs.pony)

If you have a favourite editor that isn't supported, we'd love to help you build a Pony package for it.

## The compiler

Pony is a _compiled_ language, rather than an _interpreted_ one. In fact, it goes even further: Pony is an _ahead-of-time_ (AOT) compiled language, rather than a _just-in-time_ (JIT) compiled language.

What this means is that once you build your program, you can run it over and over again without needing a compiler or a virtual machine or anything else. It's a complete program, all on its own.

But it also means you need to build your program before you can run it. In an interpreted language or a JIT compiled language, you tend to do things like this to run your program:

```bash
$ python helloworld.py
```

Or maybe you put a __shebang__ in your program (like `#!/usr/bin/env python`), then `chmod` to set the executable bit, and then do:

```bash
$ ./helloworld.py
```

When you use Pony, you don't do any of that!

## Compiling your program

If you are in the same directory as your program, you can just do:

```bash
$ ponyc
```

That tells the Pony compiler that your current working directory contains your source code, and to please compile it. If your source code is in some other directory, you can tell ponyc where it is:

```bash
$ ponyc path/to/my/code
```

There are other options as well, but we'll cover those later.
