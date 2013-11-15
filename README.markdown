About
=====

ag-and-a-half.el provides a simple compilation mode for [the silver searcher ag](https://github.com/ggreer/the_silver_searcher)

Installation
============

Add the following to your .emacs:

```lisp
(add-to-list 'load-path "/path/to/ag-and-a-half")
(require 'ag-and-a-half)
;; Create shorter aliases
(defalias 'ag 'ag-and-a-half)
```

This will load the `ag-and-a-half` functions, and create shorter
aliases for them.

Untested Commands
=================

```lisp
(defalias 'ag-same 'ag-and-a-half-same)
(defalias 'ag-find-file 'ag-and-a-half-find-file)
(defalias 'ag-find-file-same 'ag-and-a-half-find-file-same)
```

I haven't tried these.  Use at your own risk!

Credits
=======

ag-and-a-half was haphazardly hacked up from [ack-and-a-half](https://github.com/jhelwig/ack-and-a-half).  I only ever used the main ack-and-a-half function, so I quickly ported it to ag (mainly through find and replace).
