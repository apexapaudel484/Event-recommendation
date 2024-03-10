In all the files data is read,cleaned,visualized and required dataset with required field is created to work with.

**Content_based:**
A recommendation system introduced to recommend the events to the user according to the similarity of the content they choose to view(i.e content based recommendation system). All the data like title , date , location , description are combined in a tag where we perform stemming using natural language processing then the similarity with each event is calcualted (cosine distance) and recommend 5 most similar events.  
The dataset used here contains data of events happening in USA extracted from eventribe website using Webscrapping.

**Collaborative_filtering:**
A user based recommendation system build using collaborative filtering approach where events are recommended on the basis of user who were interersted in more than 200 events and event in which more than 10 users were interested.Formed a cluster,computed cosine distance and recommend 5 events on the basis of similarity.
The data used is from the competition to build event recommender system .

The data contains : 
event.csv = events.csv contains data about events in our system, and has 110 columns. 

user.csv = users.csv contains demographic data about our user.

train.csv = train.csv has six columns:  user, event, invited, timestamp, interested, and not_interested.


These are the mostly used data. The name of the events and user were not clarified in the data only event_id and user_id was provided.


**Sentiment analysis:**
Perfomed using natural language processing .The dataset used is downloaded from yelp academic dataset provied by yelp. Here,I used bussiness data to see  business ,review dataset to see the review of the business , user dataset to see what user left the review . 

To classfiy the review as negative, positive or neutral i used two approaches:
-The vader model which check the polarity of the review and give us positive,negative,neutral,compound value of the review . It uses bag of word approach and check polarity without context.
-The roberta model which uses pre-trained model "sentiment anayalysis of twiter"  which is trained in larger data, this also takes context in consideration and classify those review in positive ,negative, neutral. Used Hugging Face Transformers library.
and compared two model.

In the same dataset topic modelling is perfomed to identify key topics of review using LDA .
for this genesim is used to identify the topics and visualize the result.
