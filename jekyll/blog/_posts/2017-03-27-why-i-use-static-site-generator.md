---
layout: post
title:  "Why I use a static site generator (and store all my content in a public Git repo)"
date:   2017-03-27 15:55:41 -0700
featured_image: "http://placehold.it/350x350"
excerpt: Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit.
categories: blog cms github
---
I’ve spent over a decade managing various content management systems as part of my day job. Drupal, Wordpress, ExpressionEngine. Custom CMSes built in-house. Tumblr instances. For a long time I used Wordpress, until about this time last year, I migrated this blog from Wordpress to Hugo.

<h2>Why use a static site generator at all?</h2>
I think that many marketers may find this decision strange. Wordpress makes things easy! You don’t have to touch code, all the logic to display, organize, and style your content is taken care of, and so on. If you use something like Wordpress VIP, you don’t even have to worry about security updates or server maintenance.

Why would you give this up? I mean, just look at how much work it is to implement features that you get for free in most CMSes.

Honestly? I kind of hate content management systems. I guess this is for a few reasons:

1) Lots of baggage

I’ve written simple Wordpress modules and done light theming for Wordpress and Drupal. I found it really, really difficult. To get the tremendous customizability advantages of CMSes (you can do pretty much anything you want through modules), you add a lot of baggage. These blog engines are frameworks, and you have to learn to work within them, using their conventions. You have to learn the_post(); vs. $post.

Whereas with a static site generator (well, with this one, at least), things are a lot simpler. Standard styling that I can write that gets applied everywhere, for example. Really simple page templates.

It’s much, much harder to build advanced functionality that I might be able to get simply from a Wordpress or Drupal modules, but I really only need something pretty lightweight. In fact, I suspect that if you really think about what you need and what adds value to your blog or website, you might only need something lightweight, too.

2) Your data is locked up

All the major CMSes store content data in a database. This is (was?) for very good reasons related to flexibility and speed. And since CMSes are targeted at non-technical users, it’s not a big deal that they can’t get their data out, because they probably don’t care anyway, right? As long as the site works.

Except I really do care. I like to have my data in standard files that I can easily retrieve and back up. Critically, I like the idea of being able to reuse this data easily if I ever want to move to another system. Migrating out of Wordpress was pretty difficult; I’d rather not do that again.

<img src="http://placehold.it/320x240">
Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit.

Etiam porta sem malesuada magna mollis euismod. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod. Nullam quis risus eget urna mollis ornare vel eu leo.

3) They’re insecure and a pain to back up Because CMSes store important data in two places — a database for content and a bunch of files for everything else — and because they’re accessible from the public internet, they require lots of updating and various bits of maintenance. Whereas with a static site, you’re just dealing with a bunch of files.