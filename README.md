# Movie-Recommendation-System


A recommendation system is a type of information filtering system which challenges to assume the priorities of a user, and make recommendations on the basis of user’s priorities. Huge range of applications of recommendation systems are provided to the user. The popularity of recommendations systems have gradually increased and are recently implemented in almost all online platforms that people use. The content of such system differs from films, podcasts, books and videos, to colleagues and stories on social media, to commodities on e-commerce websites, to people on commercial and dating websites. Often, these systems are able to retrieve and filter data about a user’s preferences, and can use this intel to advance their suggestions in the upcoming period. For an instance, Twitter can analyze your collaboration with several stories on your wall so as to comprehend what types of stories please you. Many a times, these systems can be improvised on the basis of activities of a large number of people. For example, if Flipkart notices that a large number of users who buy the modern laptop also buy a laptop bag. They can commend the laptop bag to a new customer who has just added a laptop to his cart. Due to the advances in recommender systems, users continuously expect good results. They have a low edge for services that are not able to make suitable recommendations. If a music streaming application is not able to foresee and play song that the user prefers, then the user will just stop using it. This has led to a high importance by technical corporations on refining their recommendation structures. However, the problem is more complicated than it appears. Every user has different likes and dislikes. In addition, even the taste of a single customer can differ depending on a large number of aspects, such as mood, season, or type of activity the user is performing. For an instance, the type of music one would prefer to listen during exercising varies critically from the type of music he would listen to while preparing dinner. They must discover new areas to determine more about the customer, whilst still determining almost all of what is already known about of the customer. Two critically important methods are widely used for recommender systems. One is content-based filtering, where we attempt to shape the users preferences using data retrieved, and suggest items based on that profile. The other is collaborative filtering, where in we try to cluster alike users together and use data about the group to make recommendations to the customer.

1.1 Introduction to Collaborative Filtering 

The basic methodology of collaborative filtering systems is that these undetermined ratings can be credited since the noticed ratings are often highly linked across several users and items. For an instance, assume two users named Ramu and Shamu, who have very comparable tastes. If the ratings, which both have stated, are very similar, then their resemblance can be determined by the fundamental algorithm. In such cases, there is a high probability that the ratings where in just one of them has definite value, are also likely to be similar. This similarity can be used to make interpretations about partly stated values. Almost all the projects for collaborative filtering emphasis on leveraging either item associations or user associations for the calculation procedure. Many of the models implement both kinds of correlations. Additionally, some mock-ups use judiciously designed optimization procedures to generate a training model in much the similar way a classifier generates a training model from the mentioned or specified information. This model is later used for assigning the absent values in the matrix, in the similar way that a classifier assigns the absent test tags. There are two types of methods which are frequently implemented in collaborative filtering that are denoted to as memory-dependent procedures and model-dependent procedures.

 1.2 Introduction to Content Based Filtering 

Content Based Recommendation procedure checks for the adores and aversions of the user and creates a User-based Profile. For producing a user profile, we check for the item profiles and their equivalent user rating. The user profile is the combination of sum of the item profiles where combination being the ratings customer or user has evaluated. After profile of the user has been generated, we estimate the resemblance of the user profile with all the items in the database, which is considered using cosine resemblance between the user generated profile and item profile. Benefits of Content oriented procedure is that other user’s information or data is not essential, and the recommender system can commend new commodities or anything which are not evaluated presently, nevertheless the recommender system will not recommend the items outside the type of items the user has given ratings of.

1.3 Problem Statement & Objectives

Everyone loves movies irrespective of age, gender, race, color, or geographical location. We all in a way are connected to each other via this amazing medium. Yet what most interesting is the fact that how unique our choices and combinations are in terms of movie preferences. Some people like genre-specific movies be it a thriller, romance, or sci-fi, while others focus on lead actors and directors. When we take all that into account, it’s astoundingly difficult to generalize a movie and say that everyone would like it.
So here’s where we extract the juice out of all the behavioral patterns of not only the audience but also from the movies themselves 

 
1.4 Hardware & Software requirements

Hardware Requirements
•	RAM: Minimum 16gb
•	CPU: Above Intel core i7 7th Gen
•	GPU: Is required
•	Storage: 1TB HDD
•	Operating system: Linux, MacOS or Windows

Software Requirement
•	TensorFlow 
•	Python

2. Literature Survey
MOVREC is a movie recommendation system presented by D.K. Yadav et al. based on collaborative filtering approach. Collaborative filtering makes use of information provided by user. That information is analyzed and a movie is recommended to the users which are arranged with the movie with highest rating first. Luis M Capos et al has analyzed two traditional recommender systems i.e. content based filtering and collaborative filtering. As both of them have their own drawbacks he proposed a new system which is a combination of Bayesian network and collaborative filtering. A hybrid system has been presented by Harpreet Kaur et al. The system uses a mix of content as well as collaborative filtering algorithm. The context of the movies is also considered while recommending. The user - user relationship as well as user - item relationship plays a role in the recommendation. The user specific information or item specific information is clubbed to form a cluster by Utkarsh Gupta et al. using chameleon. This is an efficient technique based on Hierarchical clustering for recommender system. To predict the rating of an item voting system is used. The proposed system has lower error and has better clustering of similar items. Urszula Kużelewska et al. proposed clustering as a way to deal with recommender systems. Two methods of computing cluster representatives were presented and evaluated. Centroid-based solution and memory-based collaborative filtering methods were used as a basis for comparing effectiveness of the proposed two methods. The result was a significant increase in the accuracy of the generated recommendations when compared to just centroid-based method. Costin-Gabriel Chiru et al. proposed Movie Recommender, a system which uses the information known about the user to provide movie recommendations. This system attempts to solve the problem of unique recommendations which results from ignoring the data specific to the user. The psychological profile of the user, their watching history and the data involving movie scores from other websites is collected. They are based on aggregate similarity calculation. The system is a hybrid model which uses both content based filtering 10and collaborative filtering. To predict the difficulty level of each case for each trainee Hongli LIn et al. proposed a method called content boosted collaborative filtering (CBCF).The algorithm is divided into two stages, First being the content-based filtering that improves the existing trainee case ratings data and the second being collaborative filtering that provides the final predictions. The CBCF algorithm involves the advantages of both CBF and CF, while at the same time, overcoming both their disadvantages.

3. Approach
There are various types of recommender systems with different approaches and some of them are classified as below:
 
3.1 Demographic Filtering

They offer generalized recommendations to every user, based on movie popularity and/or genre. The System recommends the same movies to users with similar demographic features. Since each user is different , this approach is considered to be too simple. The basic idea behind this system is that movies that are more popular and critically acclaimed will have a higher probability of being liked by the average audience. Before getting started with this – 
● We need a metric to score or rate movie 
● Calculate the score for every movie 
● Sort the scores and recommend the best rated movie to the users. We can use the average ratings of the movie as the score but using this won't be fair enough since a movie with 8.9 average rating and only 3 votes cannot be considered better than the movie with 7.8 as as average rating but 40 votes. So, I'll be using IMDB's weighted rating (wr) which is given as :-


where,

●	v is the number of votes for the movie;
●	m is the minimum votes required to be listed in the chart;
●	R is the average rating of the movie; And
●	C is the mean vote across the whole report

 

3.2 Content Based Filtering

In content-based filtering, items are recommended based on comparisons between item profile and user profile. A user profile is content that is found to be relevant to the user in form of keywords(or features). A user profile might be seen as a set of assigned keywords (terms, features) collected by algorithm from items found relevant (or interesting) by the user. A set of keywords (or features) of an item is the Item profile. For example, consider a scenario in which a person goes to buy his favorite cake ‘X’ to a pastry. Unfortunately, cake ‘X’ has been sold out and as a result of this the shopkeeper recommends the person to buy cake ‘Y’ which is made up of ingredients similar to cake ‘X’. This is an instance of content-based filtering.
 

We will be using the cosine similarity to calculate a numeric quantity that denotes the similarity between two movies. We use the cosine similarity score since it is independent of magnitude and is relatively easy and fast to calculate. Mathematically, it is defined as follows:

We are now in a good position to define our recommendation function. These are the following steps we'll follow :-

●	Get the index of the movie given its title.
●	Get the list of cosine similarity scores for that particular movie with all movies.
●	Convert it into a list of tuples where the first element is its position and the second is the similarity score.
●	Sort the aforementioned list of tuples based on the similarity scores; that is, the second element.
●	Get the top 10 elements of this list. Ignore the first element as it refers to self (the movie most similar to a particular movie is the movie itself
●	Return the titles corresponding to the indices of the top elements.

Advantages of content-based filtering are:
●	They capable of recommending unrated items.
●	We can easily explain the working of recommender system by listing the Content features of an item.
●	Content-based recommender systems use need only the rating of the concerned user,and not any other user of the system.

Disadvantages of content-based filtering are:
●	It does not work for a new user who has not rated any item yet as enough ratings are required content based recommender evaluates the user preferences and provides accurate recommendations.
●	No recommendation of serendipitous items.
●	Limited Content Analysis- The recommend does not work if the system fails to distinguish the items hat a user likes from the items that he does not like.

3.3 Collaborative Filtering based systems

Our content based engine suffers from some severe limitations. It is only capable of suggesting movies which are close to a certain movie. That is, it is not capable of capturing tastes and providing recommendations across genres.
Also, the engine that we built is not really personal in that it doesn't capture the personal tastes and biases of a user. Anyone querying our engine for recommendations based on a movie will receive the same recommendations for that movie, regardless of who she/he is.


 

Therefore, in this section, we will use a technique called Collaborative Filtering to make recommendations to Movie Watchers. It is basically of two types:-

1.	User based filtering- These systems recommend products to a user that similar users have liked. For measuring the similarity between two users we can either use Pearson correlation or cosine similarity. This filtering technique can be illustrated with an example. In the following matrix's, each row represents a user, while the columns correspond to different movies except the last one which records the similarity between that user and the target user. Each cell represents the rating that the user gives to that movie. Assume user E is the target.

 
 

2.	Item Based Collaborative Filtering - Instead of measuring the similarity between users, the item-based CF recommends items based on their similarity with the items that the target user rated. Likewise, the similarity can be computed with Pearson Correlation or Cosine Similarity. The major difference is that, with item-based collaborative filtering, we fill in the blank vertically, as oppose to the horizontal manner that user-based CF does.

 




Advantages of collaborative filtering based systems:
●	It	is	dependent	on	the	relation	between	users	which	implies	that	it	is content-independent.
●	CF recommender systems can suggest serendipitous items by observing similar-minded people’s behavior.
●	They can make real quality assessment of items by considering other peoples experience


Disadvantages of collaborative filtering are:
●	Early rater problem: Collaborative filtering systems cannot provide recommendations for new items since there are no user ratings on which to base a prediction.
●	Gray sheep: In order for CF based system to work, group with similar characteristics are needed. Even if such groups exist, it will be very difficult to recommend users who do not consistently agree or disagree to these groups.
●	Sparsity problem: In most cases, the amount of items exceed the number of users by a great margin which makes it difficult to find items that are rated by enough people.


 

 
  

   

 
  

 
  

   

  
