---
layout: post
title: Better Rspec errors with Vim formatting and quickfix
excerpt: "Jump straight to your rspec error locations from Vim using this nifty trick with the quickfix window"
tags: [sample post, code, highlighting]
modified: 2014-09-14
comments: true
quickfix: 
---

If you, like me, drank the TDD/BDD Kool-aid and liked how it tasted, you probably started spending a lot of time writing tests which drive most of the application code you write.  Red, Green, Refactor, etc.  My tool of choice is Rspec, although Minitest is also quite nice.


Maybe I just have lazy eyes, but I get tired of scanning the pane where my tests run to find the exact location of each test failure, then navigating to it.  I'm pretty fast with vim file navigation, but I wanted a better way.


Enter the [quickfix](http://vimdoc.sourceforge.net/htmldoc/quickfix.html)
feature in Vim.  It was originally conceived to save error messages from compilers and allow you to to jump from the list of errors to the actual location of the errors, one by one.  Yeah so that's exactly what we want to do with our Rspec errors, right?  It's just a matter of formatting the rspec output to match what quickfix expects.






