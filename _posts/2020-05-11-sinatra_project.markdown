---
layout: post
title:      "Sinatra Project"
date:       2020-05-11 21:30:19 +0000
permalink:  sinatra_project
---


This entry is for the Sinatra project and everything I have learned in the last few months.

To me building this Sinatra application has been exciting in seeing how everything has come together even from the beginning. Learning how to build something that we use daily is amazing to see come together and where we may be headed. Don’t get me wrong, I loved building the CLI app but it could only really work on that terminal. Watching this app work on a website and be able to navigate it was very heartwarming.

I learned a lot with Object Oriented Ruby and Procedural Ruby. I think the one thing I did not expect is how you really only use the key aspects of that for other applications. Of course we wouldn’t use everything and being able to know how it works is very key in understanding it. Still watching all that I learned in there play a key role in the Sinatra app was good to see. One of the more complex things I used that helped was `@pokemons = Pokemon.select {|pokemon| pokemon.user_id == @user.id}`. Then I would iterate over `@pokemons` in the view page. 

I know in the readings it mentioned rails is a lot more built out and user friendly and you can do more with it but understanding where it came from and how to use Sinatra only sets us up to use rails a lot better. Working with activerecord and rake is something that I believe will follow into other applications and learning now on a less advanced application makes it easier to use.

One thing I for sure will do during this week break is going over some of the bonus work like CSS, Rack and HTML. That way I can understand rack a lot better and I would love to be able to build out the view page to look a lot nicer. There were some things I wanted to do with my app to make it look a lot better. I just did not know how to do it and did not have the time to learn all of it. I would love to be able to add a little bit more of a touch to it.

The one thing I will say I used the most in that project were the helper methods. If you look through all of that code you will see a lot. The one thing in there though that shows up in almost every controller line is `current_user` and `is_logged_in`. They make a lot of sense but I never realized how useful and needed they are. When you visit almost any site with a login you cannot type in the URL to a site without it taking you to the home page or the login. I am not sure what I thought before but it makes sense now that almost every page has that line of code in it’s controller action. This makes sure every user has to login and that no one else can view or edit things they should not be able to!

The final thing that surprised me and taught me a lot was sessions. I had a basic understanding of a cookie that they stored data for you and only you at that website. However, I had no idea that there were two kinds of cookies and how they help making that website more convenient. The most underrated thing they did I never realized was keeping you logged in when you went from page to page. Of course everything on the internet has to be coded so nothing was like the internet does this by default but I never realized sessions and cookies are what kept you logged in just going from page to page.

With this project I have learned so much and am excited to see our code being used in something that we use everyday! I am excited to keep going and even dive into rails.



