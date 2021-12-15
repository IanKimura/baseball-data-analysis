# baseball-data-analysis
## About the dataset
The dataset is called mlbBat10 which is a dataset that has every 
baseball player that played a game in the year 2010 along with 
their corresponding stats. I chose this dataset because of my 
strong interest in the sport of baseball. I have been playing
and watching baseball since I was 5 and wanted to take my 
interest further analyzing players. 
## Stating the problem
The problem or question I wanted to ask was about what made 
baseball good offensively. Baseball is such an interesting sport 
because of how diverse the definition of "good" is and is 
fascinating hearing the conversations of people comparing 
players. I want to see what basic statistic will have the most 
effect on how good a player is. I also take a look at the 
differences in speed and strength while comparing it to the
different position that each player plays to see any 
relationships.
## Analysis for the offense variable question
To start analyzing the dataset, I needed to first manipulate 
some aspects of the data to suit what I need. For example, I 
had to get rid of some data points that will skew my date. 
Players that don't play enough games will have too little of a
sample size to be taken seriously and so to combat this I took 
out all the players who played less than 50 games. Since I only 
care about offense I took out all the players that were the 
position "P". I then needed a stat to compare the players with. 
Because there was a limited selection on what stats to use I, 
with whatever information present, created the best stat in my 
opinion to judge a player's offensive performance. It is called
OPS and stands for On-Base plus Slugging and I do in fact have 
those stats available. I also added my own variable which I 
think will have a great effect on this OPS. I named it as 
extra base hit rate which is basically the rate that a player 
gets a really good hit. The way I added this was taking adding up
all the extra base hits which included doubles, triples, and home
runs and then divided it by the number of hits. Now that my data 
is ready I can start to play around with it to see any trends. I 
plotted every variable against this OPS and came up with my best
three variables. The three that came out the best were AVG(the 
rate you get a hit), HR(the best hit possible), and my own extra
base hit rate stat. Using a linear regression model on these three
variables I saw the strongest linear trend with AVG with an R-
squared of 0.574. This value just goes to show how hard 
determining the quality of a baseball player just by one stat. 

## Analysis for the position by SB vs HR question
For this question, I used the same adjusted data set from the
first question to help provide an answer. To begin, I actually 
plotted SB by HR to see what I was dealing with. I notice a 
negative trend with how HR and SB interacts. SB stands for stolen
base and in baseball in order for someone to do this it takes a 
lot of speed. HR stands for homerun which is when a player hits 
the ball outside of the playing area inside the guid.lines and
to do this, it takes a lot of strength. I saw that the more HR 
a player hits the less amount of stolen base they will have and
vise verca. I then created a new dataset for the players of the same position 
to see any relationship. I found that some positions had particular
trends about strength and speed. For example the strongest trend 
was with the position called first base and they particulary only
homeruns and like no stolen bases. When I looked up the average height
and weight of first basemen it said that they were the biggest and
tallest players. It was interesting to see that based on some trends
using their play I could see that one postion is going to be stronger
or faster than the other. 

[RStudio-ymHDaW.pdf](https://github.com/IanKimura/baseball-data-analysis/files/7717218/RStudio-ymHDaW.pdf)
