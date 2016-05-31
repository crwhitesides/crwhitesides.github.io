---
layout: post
title:  "require 'patience'"
date:   2016-05-30 20:05:21 -0400
---

![](http://i.imgur.com/GzoDlAv.gif)

Today I completed a working version of my `crowd-forecast` gem. Disneyland, Legoland and other US-based theme parks probably won't see an increase in foot traffic (primarily because the gem hasn't been published), but at least I can access the necessary information to try and avoid huge crowds this summer. I'll be honest, I probably took somwhere between 7-10 days to complete this project. Why? Well, mainly because I got sidetracked. However, in the process I made three RubyGems and, quite frankly, I'm pretty proud of them all. So, here's a look at the resources I used and the process I went through to complete this project.


Where to begin?
Like many out there, I wasn't entirely sure how to begin the process of building a RubyGem. Scraping wasn't terribly intimidating. But bringing it all together into one application sounded daunting. Luckily, the lesson provides some examples and a video walkthrough of Avi making a CLI gem. So, that's where I started. 

#### Resources:

* Watch walkthrough of [Avi building the `daily-deal` gem](https://www.youtube.com/watch?v=_lDExWIhYKI)
* Peruse the repositories of the [`playing-now`](https://github.com/learn-co-curriculum/now-playing-cli-gem) and [`worlds best restaurants`](https://github.com/dannyd4315/worlds-best-restaurants-cli-gem) gems


RubyGems 101
Throughout the video walkthrough, Avi briefly scans a [rubygem.org](https://rubygems.org/) guide titled Make Your Own Gem . The likelihood of publishing my gem to [rubygems.org](https://rubygems.org/) was high, so I decided to spend time reading some of their guides and going through their walkthroughs. 

#### Resources:

* Read the following four guides: [RUBYGEMS BASICS](http://guides.rubygems.org/rubygems-basics/), [WHAT IS A GEM?](http://guides.rubygems.org/what-is-a-gem/), [MAKE YOUR OWN GEM](http://guides.rubygems.org/make-your-own-gem/), and [PUBLISHING YOUR GEM](http://guides.rubygems.org/publishing/).
* Go through the process of building the gem in the Make Your Own Gem guide. The gem I built was [`hola_crwhitesides`](https://github.com/crwhitesides/hola_crwhitesides).


##  Shiny object
Upon completing the `hola-crwhitesides` gem, I found out that Netflix had launched [fast.com](https://fast.com/). This website allows anyone to easily check their download speed. The functionality of the site seemed simple and I, therefore, concluded I could create a CLI gem that would show people their download speeds. Well, this took longer than anticipated. It turns out that Nokogiri is great for parsing HTML, but parsing HTML+Javascript is a bit more complicated. Anyways, as I moved forward with this side project, I became acquainted with [Capybara](https://github.com/jnicklas/capybara), [Poltergeist](https://github.com/teampoltergeist/poltergeist) and [PhantomJS](http://phantomjs.org/). Ultimately, these tools allowed me to complete a working version of the [`how-fast`](https://github.com/crwhitesides/how-fast-cli-gem) CLI gem. 

##  Look, Ma, no hands!
Finally, after building and publishing the `hola-crwhitesides` and `how-fast` gems, I felt pretty good about actually making a RubyGem that met the specifications of the project. Without further ado, I present to you the [`crowd-forecast`](https://github.com/crwhitesides/crowd-forecast-cli-gem) CLI gem. The main challenge of this gem was the investigative work involved in scraping. However, Nokogiri's documentation and Pry proved an effective combination in overcoming any issues.

#### Resources:

* [Nokogiri cheat sheet](https://github.com/sparklemotion/nokogiri/wiki/Cheat-sheet)
* [Nokogiri tutorials](http://www.nokogiri.org/)



