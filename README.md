# cl-lib highlighting

Since the Emacs devs have chosen not to add this, this library adds
all of the familiar highlighting to `cl-lib` functions (`cl-defun`,
`cl-loop`, etc.) that were originally provided for `cl`.

## Usage

Load this library and run `cl-lib-highlight-initialize`.

If you want to mark out the old `cl` functions, also run
`cl-lib-highlight-warn-cl-initialize`.

## Motivation

I think `cl-lib` was a mistake, but since it here it may as well be
well-supported.
