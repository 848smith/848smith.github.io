---
layout: post
title:      "Importance of Associations"
date:       2020-06-08 21:27:45 +0000
permalink:  importance_of_associations
---


Associations in Sinatra or any application that uses it is makes it a lot easier to figure out how to code something so you don't have to write as much. This may look to be lazy which it may be but being easier also helps for other people to read it. It's a lot better to use a convention that makes it easier to code and easier to read. For example this line of code it in my Sinatra Project about storing Pokemon.
```@pokemons = Pokemon.select{|pokemon| pokemon.user_id == @user.id}``` 
This line helps me get a variable that houses all the pokemons for a single user and just their pokemon. However, this can be easily achieved with this code.
```@pokemons = @user.pokemons```
Since earlier in the code I defined @user this is saying you take all the pokemons associated with that user and have it equal to @pokemons. As you can see this is much earier to write and does the same thing as the code above. The best part is that if everyone knows this convention which they should this is easier to read cause they know associations. The one above they will have to read the whole line and make sure they understand what it is doing. Of course it makes sense but someone may have to fact check to make sure they fully get what it is saying.

In order to get this to work I made a belongs_to and mas_many relationship between users and pokemons. This works by saying a user has many pokemons while a pokemon belongs to a user. I did this in the user models. The only code I had to put was for the user model saying ```has_many :pokemons``` and then pokemon model said ```belongs_to :user```. This then associated the tables together for each model. I also had to put a column in the pokemon table that had user_id for it. That way when you join the tables it has a way to belong to a user. It belongs to that user that has the corresponding id. 

This is just one of way you can use associations. You can also use has_many :through. This will let you set up a many to many connection with another model. It could work possibly if I wanted to introduce a third model called battles. I could then join them all by saying a user has_many pokemons and has_many :battles, through: pokemons. Then you would say a pokemon belongs_to :user and has_many :battles. Finally the battles model would say it belongs_to :pokemons. This will then associate the tables so you can say @user.battles will show all the battles a user has had.

To wrap this up the main reason again this is so helpful is that it is a common convention any engineer should know. This means that if you use it and someone has to come in and take over your code or help they can read it easily and know what it is talking about. A long formula could mean they have to dig or look at for a second to interpret what it means. Also, it means less code so you don't have to think as hard to get the same outcome.
