# hackai-2023

Website:

https://zratrout.wixsite.com/jazs

This Github contains an example for how our backend processes Twitter and play-by-play (pbp) data. 

In this example, I am generating an image from a game between the Dallas Mavericks and the Phoenix Suns. The tweet we are looking at is "LD out here playing bully ball 🤯" (https://t.co/BVdnaUcjhl). Tweets are selected only among those with the most fan interactions per game.

The program selects pbps which occurred at least 5 minutes before the tweet was created. Then, it makes an API call to respell to determine which selected pbp best relates to the tweet. Then, the respell-selected pbp is passed to the Wombo/Dream API to generate an image of the pbp.

For example, the example tweet is saying LD (Luka Doncic) did something insane, then the respell call returns the most relevant pbp in which Luka do something insane. Then, an image is generated which shows Luka doing an insane maneuver.
