---
layout: post
title:      "First Project!"
date:       2020-03-16 02:24:37 -0400
permalink:  remembering_the_index
---


I have completed my first project. To be honest I started on it late because this has been rough and pretty tough in this course. That is something I enjoy because I love a challenge! These first couple months have been a challenge balacing school, work and life. Nonetheless, this project has been fun to figure out and get working as I will explain how my project went.

At first, as I stated above, I had a rough time getting this started. With life and it being tough to start from scratch I was not sure what to do. Lately though me and my friend have picked back up in Pokemon Go. It made sense to try and make a CLI that can pull any pokemon name and display info on that pokemon. When I started to actually dig in and watch the basics on how to set this up I really started to get into it.

The first thing I worked on was getting the gemspec, the bin and the main .rb file working as to how it should be. Once I watched the setup on that I started working on the API. This was my first challenge because I was going to scrape a sight but after my teacher mentioned there is APIs out there for almost everything I searched PokeAPI. I got an instant hit for a well none API that is free to use with no sign up. Figuring out how to get this to work was tough. I tried using the httparty as best I could but I ran into some issues. Figuring out the API was the hardest task but not the longest. I did some searching and actually found someone who made a gem for the PokeAPI that made it easier to use. Once I installed that gem I got the data functionally working. Next I had to figure out how to break all the info down. Once I figured that out for the first information piece it was all about trying to find what I needed.

This process was the most I had ever used pry. I knew it was useful but during the labs I had used Repl. I would try code on there to see if it worked first or why it was not working. This project though I used pry to find out each piece of info and how to pull it. Once I got what I wanted I plugged it in. Finally, once I figured out the whole hash of my data and how I wanted to store it the next part was making objects out of it!

Making objects was easy. This part I have done in labs almost everyday and was like second nature. The one thing that I learned how to use more in depth and saw it's functionality was the self.send(("#{lkey}="), value). This made it so easy to set up the initialize method. After that setting up a save and self.all method is something I can do in my sleep.

Finally the longest pary was making the CLI. This was tough cause I wanted to make it look good and user friendly. The longest part was typing out all the puts and making sure the lines lined up so it looked nice. It was a bit hard as I ran into some issues with making sure quits worked and interpolating nested hashes for a second. Once I got those going I went through most of it with ease! There was two parts that slowed me down. The frist one was trying to remember how to do a while loop and looping through an array. I figured out I could just do the counter minus 1 to pull out each individual game the pokemon was in. It looked something like @data.games[i-1]. Doing that I was able to loop each game out of the array as I increased the counter each time. 

The second one that gave me trouble was trying to display two strings out of an array by making it look like "poison and grass" and not ["poison", "grass"]. I ran an if statement that said if the length of the array was larger than the size of one then I would interpolate each part of the array. I knew I could do it like this because no pokemon has more than two types. Then the else was just interpolating one part of the array.

Once I got that last part I made a edited_display method that basically repeated the display. This made the whole class look super big but it was mostly copy and paste. The one edit on this was to make sure when having someone prompt to pick another selection it would not greet them or tell them what they selected since they already know. After this my project was done! 

This project again was fun. I shouted each time I got a major piece of it working without an error telling me how it was not working each step of the way. I liked making this mostly on my own. I personally cannot wait till we get to learn more and make more projects that won't be just a gem but much more.
