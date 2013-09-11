# cl-lib highlighting

This library adds all of the familiar highlighting to `cl-lib` macros
(`cl-defun`, `cl-loop`, etc.) that were originally provided for `cl`.

It's not simply throwing in all the symbols as keywords. They're being
added using the same regular expressions that `cl` gets, so function
names get highlighted with `cl-defun`, type names get highlighted with
`cl-defstruct`, etc.

![](http://i.imgur.com/hwenyf3.png)

## Usage

Load this library and run `cl-lib-highlight-initialize`.

If you want to mark out the old `cl` functions with a warning face,
also run `cl-lib-highlight-warn-cl-initialize`.

## Motivation

I think `cl-lib` was a mistake, but since it's here it needs to be
well-supported. The Emacs devs
[have chosen to exclude `cl-lib` font-locking](http://emacs.1067599.n5.nabble.com/bug-12761-cl-lib-el-functions-do-not-get-font-locked-like-cl-el-ones-td268332.html)
so it must be supported through a library.
