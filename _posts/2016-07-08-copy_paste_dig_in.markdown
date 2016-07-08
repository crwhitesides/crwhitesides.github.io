---
layout: post
title:  "Copy, Paste, Dig In"
date:   2016-07-08 15:03:53 -0400
---


The purpose of my CRUD app is to keep track of the ever-growing list of books I want to read. (I love to read.)

If there's one thing I've learned from the Sinatra lessons, it is that copying and pasting controller actions from other projects is an easy way to establish a template for any app. This is exactly what I did for the [Book Wishlist app](https://github.com/crwhitesides/sinatra-book-wishlist-app) (and I'm not ashamed to admit it). Now, I made the incorrect assumption that a little refactoring here and there shoulg be enough to make things *just work*. However, I came to the quick realization that although a template is useful, domains vary greatly and, therefore, require specific care. 

With that said, allow me to briefly describe the process I went through to create the Book Wishlist app:

* Determine models (User and Book) and their corresponding associations (I usually draw this out...on paper)
* Copy general file structure of Fwitter app (adapted to the needs of my app)
* Create Users and Books tables with corresponding columns
* Build out controllers and views in the order (more or less) established in Fwitter's specs (I did copy and paste a few controller actions, but found that I ended up refactoring so much of them that I just started writing them myself using Fwitter's specs as a basic guide)
* Refactor, refactor, refactor
* Realize that my `Slugifiable` model only finds the first instance of a book in the database. But what if more than one user has added the same book to their list (and, therefore, to the database)? Refactor `Slugifiable` class methods to ensure that users can always find the instances of books that belong to them (using `find_all` and `detect` methods based on slug and session id).
* Refactor, refactor, refactor

Now, this is an oversimplification of the process I went through to create my app. However, it offers a look at how I created a basic template for my app and then adapted it to my specific needs. That's pretty much all I did. 
