# A reciprocal recommender for online dating: RECON summary

Reciprocity is the key to success in online dating.

Characteristics of an explicit profile include information that users disclose about themselves and their preferences, while an implicit profile is based users’ actual behavior. What people say vs. what they do has been found to be incongruent.

Examining the user’s implicit behavior is telling. For instance, if a user sees a match via initial recommendations, and chooses to go back to explore other recommendations, then something about the match’s profile discouraged the user.

Depending on the online dating system, the system may not be able to recognize success or failure. Feedback is lacking: A person may leave the website after finding a successful match, or conversely, may have been discouraged and quit the website prematurely. One way of understanding the user is by looking at the amount of mutual messaging – or lack of messaging – that occurs between two users.

It is important to not recommend users who are popular to everyone, because they may get too much attention and stop messaging. The user that sent the message to the popular match may assume disinterest when the reality is the user is overwhelmed and cannot siphon through all profiles.
Because the system can not distinguish between proactive and reactive users, it is key for reactive users to be in the recommendations for the system to learn their preference.

At IBM, there is a social networking website that uses content-based filtering. Content-based filtering in this context tags users using certain keywords to understand what the user is interested in. Then it looks up those keywords and recommends similar users that share the same interest. This yields the best recommendations at connecting users with people that can assist them with unfamiliar tasks.

In one study, personal characteristics are more important to certain group of users. For instance, women are pickier about their match’s occupation than men are. There is a positive relationship in personal attributes between compatible matches. The article suggests there is a possible value of integrating content-based techniques into online dating recommenders.

The dataset used to create the recommender in this article is based on an Australian dating website. They observed that mutual messaging was correlated with proceeding to communicate via email on the website, which typically is not free. 

Once mutual messaging is established, a preference model is constructed which records the attributes of both parties. This is a good signal of the type of user liked by the initiator of the message.

While profiles have both free text and attributes, free text was ignored and only attributes like body shape, personality, marital status, and education were considered in building the recommender.  The recommender finds people who contain all the attributes that the user looked for and generates a preference model, which learns based on mutual messaging. 

If a person is messaging in a big city, their number of recommendations is going to be larger than someone who messaged in a smaller area. Ranking recommendations can be based on user’s engagement on the website or if they are a premium member.

The recommender in this article was initialized with a reduced set of users only looking at three attributes: gender, age, and location, which was considered as most important in successful online dating communication.

The algorithm was built on 6 weeks of data – 4 weeks of data used for training and 2 weeks for testing of active users. The algorithm’s accuracy was evaluated by looking at the success rate of known interactions. For instance, if the algorithm recommended 5 people, the user messaged 2 people, but 1 person responded favorably, the success rate is 50%. The authors found their recommender outperformed a user’s own search in finding a successful interaction.

It was found that using top 10 / top 20 recommendations for new users, 1 in 4 known messages were successful if the recommendation is based on preference for a particular peer group.

Reciprocal recommenders must deal with how to distribute recommendations, to not overload popular matches or forget to include matches that are not popular. Most users like popular users, but reciprocal recommenders index for reciprocation, which may match a popular user with a non-popular user.

In the foreseeable future, I plan to digest and understand other proposed reciprocal recommenders that optimizes for successful matches.
