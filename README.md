Digital Futures Capstone Project: Come Wine With Me
======
The following outlines the capstone project I completed to end my time at the Digital Futures Academy.

Project Aims
------
My project aimed to create a summative way to detail all of the skills acquired at the Digital Futures Academy.
I decided the best way to showcase this was by combining a natural interest of mine with the Data Science / Machine
Learning skillset I'd acquired. That's where the concept of building a wine recommendation system using natural language 
processing and an unsupervised clustering algorithm began. My overall aim was to build a mechanism to ease the 
customer experience of successfully purchasing a wine they will enjoy drinking, as the jargon surrounding
wine tasting is quite exclusionary to the average consumer.

Dataset Acquisition
------
To build a system that can take user input of wine flavours they enjoy and output similarly tasting wines,
and their names, it was vital to secure a dataset with wine names, flavour descriptions, and review data. Luckily, I 
was able to find two Kaggle datasets that had been web scraped from the same wine review website from differing years.
I concatenated these datasets to create a combined data frame that I would feed into my clustering algorithmn. [Here is
the link to the first Kaggle file](https://www.kaggle.com/code/sudhirnl7/wine-recommender/data) and [heres the second](https://www.kaggle.com/code/theolegall/what-makes-a-wine-good/data). 
Both of which included data scraped from [this wine reivew site](https://www.winemag.com/)

Approach Overview
------
Following obtaining the data, the next stage of my project involved cleaning the data frame and creating extensive
data-prep functions to optimize the wine review descriptions for NLP methodology. (i.e. utilising regex
and lemmatisation to get a corpus of individual descriptors that, using vectorisation, could be weighted and fed 
into a clustering model on the optimised descriptions left by reviewers. Initially, I used KMeans clustering to produce
clusters based on wine similarity groupings but altered my approach to suit customer needs. I didn't want the final
output to be a cluster number, but an actual wine name, therefore by modifying KNN to function in an unsupervised fashion,
I was able to produce an output of the top three wine recommendations based on the user’s attributes. This worked by using the
nearest three KNN points based on NLP vectorisation and clustering to output the three nearest neighbors as product information.

Project Conclusions
------
I was able to create a user-friendly wine recommendation system that could reduce customer dissatisfaction with wine 
purchases by outputting wines that should be similar tasting to something they already enjoy. This was a really
fun project to complete and helped solidify the machine-learning skillset I have been working on the past 12 weeks of 
the academy. Something difficult to track with unsupervised clustering methods is the accuracy of the algotirmn,
I have to rely on my domain knowledge to guide how well my algorithm is fitted. One thing this led me to notice was that
inexperienced users who lack domain knowledge could receive less than optimal results. For example, if you wanted to find
a similar-tasting red wine, but input typically white wine characteristics such as ‘citrus’ and 'floral', the clustering will
suggest white wines. Having had more time I would have loved to be able to refine user input in terms of categorising the
types (red, white, sparkling) to return more specialised recommendations and thus circumvent the outlined issue.

Future Improvements
------
Additionally to the above, having had more time on the project I would have loved to implement perhaps a feature where the user
can dictate the price range of the recommendation they would like the recieve. Being able to incorporate mid-range, high-end
or budget wines into the output would enhance the users' experience in receiving a wine recommendation. Also to take this 
project further I would love to implement wine-food pairings, and perhaps allow users to input the meal they're having and
what wines would pair well with said flavours. Overall I am happy with my project and it was a fun way to implement ML and NLP
skills into something I enjoy.

Capstone Presentation
------
[You can view my capstone presentation here](https://docs.google.com/presentation/d/15IRw7o4vAPIsvgicCaZoDDI7o-1IiEhN2Sj5HdwHEj8/edit?usp=sharing)

![title page](https://github.com/Orla-Cronin/digital-futures-projects/blob/main/capstone_titlepage.png)

[pdf version of the presentation](https://github.com/Orla-Cronin/digital-futures-projects/blob/main/Capstone_Presentation.pdf)
