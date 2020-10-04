# Exercise: Processing Conventions

In this exercise we process the convention data and store it in a database. This 
is a convenient thing to do with any text data set that you'll be working with
over a longer period of time and will greatly increase the power of our analyses. 

The convention data has the following structure: 

* Boilerplate text before the first speaker. We'll ignore that.
* Speakers marked with text in the form of `Nancy Pelosi: ( 02:53 )`. We'll
  use our regular expressions to pull out the speaker and the time. 
* Different nights are stored in different files. 

We'll store the convention data in a single DB table with the following columns: 

1. party
1. night
1. speaker
1. speaker_count: This will be a counter that will go from 1 (the first time a speaker speaks
   on that night) up to the final utterance by the speaker. 
1. time
1. text

If you haven't taken ADA, I'd urge you to look at the solutions for some of the DB code after you've
spent a bit of time Googling. Some of the statements, particularly inserting data into the DB, are 
not intuitive. 

