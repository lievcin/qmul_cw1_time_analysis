# README #

### What is this repository for? ###

Part B of the Coursework1 for Big Data Processing module

### Task ###

Create a bar plot showing the number of Tweets that were posted each hour of the event. You should aggregate together all the messages 
emitted at the same hour, regardless of the day the messages were sent (hence, you will have 24 different groups). 
When checking the correctness of your results, keep in mind the timezone of the 2016 Olympic games, as that should give you base 
expectations about the prime time when the main activities occurred. [30 marks]
For the most popular hour of the games, compute the top 10 hashtags that were emitted during that hour. 

Hashtags are words contained inside the tweet, starting with the hashcode (#) character. Does that information provide you any hint on the 
main events/activities that took place at peak time? [5 marks)

### How do I get set up? ###

To build the project run: 
# ant clean dist #
To run the task on the server:
# hadoop jar dist/TweetPerHour.jar TweetPerHour /data/olympictweets2016rio out #
to merge results
# hadoop fs -getmerge out tweets_by_hour.txt #

# chart at https://cloud.highcharts.com/charts/asefimu/ #