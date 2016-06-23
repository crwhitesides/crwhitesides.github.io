---
layout: post
title:  "See what sticks (and try to understand why)"
date:   2016-06-23 17:37:20 -0400
---

Anyone who has spent any time in a kitchen has, at some point, flung a noodle at a wall in an attempt to determine whether the pasta is ready. If the noodle doesn't stick, just try again in a few minutes...because eventually it will stick! Why does the noodle stick? I don't know. Who cares. What matters is that I eventually get to a point where I can eat my pasta. The same process can be applied to all Learn.co labs, since each lab has tests that ultimately determine whether we've successfully completed a lesson or not. Since I'm already talking about spaghetti, I'll use a spaghetti analogy to describe how tests can become an unhealthy dependecy.

**Possible recipe for completing labs: **

1. Fork and clone the lab (get the pot of water boiling) and try to understand what is expected (review the recipe)
2. Start writing code and work on it until you *hope* it's right (put pasta in the pot)
3. Fling code at the tests to see if it passes (fling noodle at wall and see if it sticks)
4. If it doesn't stick, repeat steps 2 and 3 until it finally does

Pretty simple process. But what if there weren't any tests? What if there wasn't a wall to fling the noodle at? How can I determine whether my code (or pasta) actually does what it is supposed to? There's a whole lot of unnecesary hoping in step 2 that can't be satisfied without tests. But maybe there is hope? In fact, this is where IRB, Pry and other tools can take a person from merely hoping that something will work to knowing it will. In my opinion, using these tools should be the rule and not the exception.

For example, when I run into failing tests in any lab with methods and classes (pretty much all of them), I throw those very same methods and classes in to Pry and use the "dummy data" from the tests to figure out why my code isn't meeting the expectations of the tests. More often than not, after playing with the code for a while in Pry, I come up with the exact results expected by the tests and modify my code accordingly. When it comes to SQL queries, I create a test database, create the tables expected by the lab with their corresponding columns, throw in the seed data provided by the lab, and write queries in SQLite3 so that I can see what each query returns. Then it's just a matter of copying and pasting the queries from my terminal to my text editor. 

In conclusion, I would simply modify step 2 of the above-mentioned recipe so that it includes iterative experimentation in IRB, Pry, or SQLite prior to moving on to step 3. There are no guarantees that things will always work out, but I'm probably going to fling code a lot less and learn a lot more. 









