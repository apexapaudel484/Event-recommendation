Recommendation_system:
A recommendation system introduced to recommend the events to the user according to the similarity of the content they choose to view(i.e content based recommendation system). 
The dataset used here contains data of events happening in USA extracted from eventribe website using Webscrapping.

Collaborative_filtering:
A user based recommendation system build using collaborative filtering approach where events are recommended on the basis of user who were interersted in more than 200 events and event in which more than 10 users were interested.
The data used is from the competition to build event recommender system .

The data contains : 
event.csv = events.csv contains data about events in our system, and has 110 columns.  The first nine columns are event_id, user_id, start_time, city, state, zip, country, lat, and lng.  event_id is the id of the event, and user_id is the id of the user who created the event.  city, state, zip, and country represent more details about the location of the venue (if known).  lat and lng are floats representing the latitude and longitude coordinates of the venue, rounded to three decimal places.  start_time is the ISO-8601 UTC time string representing when the event is scheduled to begin.  The last 101 columns require a bit more explanation; first, we determined the 100 most common word stems (obtained via Porter Stemming) occuring in the name or description of a large random subset of our events.  The last 101 columns are count_1, count_2, ..., count_100, count_other, where count_N is an integer representing the number of times the Nth most common word stem appears in the name or description of this event.  count_other is a count of the rest of the words whose stem wasn't one of the 100 most common stems.

user.csv = users.csv contains demographic data about our some of our users (including all of the users appearing in the train and test files), and it has the following columns: user_id, locale, birthyear, gender, joinedAt, location, and timezone. user_id is the id of the user in our system.  locale is a string representing the user's locale, which should be of the form language_territory. birthyear is a 4-digit integer representing the year when the user was born. gender is either male or female, depending on the user's gender.  joinedAt is an ISO-8601 UTC time string representing when the user first used our application.  location is a string representing the user's location (if known).  timezone is a signed integer representing the user's UTC offset (in minutes).

train.csv = train.csv has six columns:  user, event, invited, timestamp, interested, and not_interested.


These are the mostly used data. The name of the events were not clarified in the data only event_id was provided.
