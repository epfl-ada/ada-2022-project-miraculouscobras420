
The Cobras: Ilker Gul, Mark Tropin, Emna Fendri, Ralph El Haddad.
# Beer :beer:
Or America's latest obsession...

## Abstract :page_facing_up:
The sense of belonging has always been an important human factor, whether it’s in opinion formation, judgment, or decision making. Cleveland people, for example, will usually root for their local NFL team, the Browns, even though that same team ends up last pretty much every season! The sense of belonging does not exclusively mean an emotional connection though, it might also express a sort of camaraderie, a sense of mutual support in financial matters. But how does this apply to beers? <br>
Beers are the most social alcoholic drinks out there: whether it’s with friends or coworkers, beers are the usual go-to in outdoor social gatherings. But how easy is it to dissociate one’s opinion about the beer from the memories that come with it? Does the sense of belonging to a group influence our supposedly impartial judgment of the product? In this project, we turn to the datasets provided by 2 major beer rating websites, BeerAdvocate and RateBeer, in search of user bias towards “local” breweries. A brewery is labeled “local” if it is located in the same state as the user, and “outsider” otherwise.



## Research Questions :thinking:
* Does the brewery's location influence users' reviews? <br>
* Do consumers prefer local or foreign beers? <br>
* How important is local support for breweries to increase sales in foreign states? <br>
* How does the burgeoning of craft beer breweries reflect users' bias for their hometown beers? 


## Proposed Additional Datasets :books:


* **[beer - worldwide](https://www.statista.com/outlook/cmo/alcoholic-drinks/beer/worldwide)** <br>
Dataset containing world ranking in beer consumption and global beer market shares between 2012 and 2022.

* **[Craft breweries per capita in 2021  in the US](https://datasetsearch.research.google.com/search?src=2&query=U.S.%20craft%20beer%20breweries%20per%20capita%202021%2C%20by%20state&docid=L2cvMTFwd2Y1NzR5NA%3D%3D)** <br>
Dataset containing craft breweries per capita data in the UD in year 2021, could illustrate the involvement of the users in the beer market and reflect potential bias towards their hometown beers.
* **[ Major beer vendor market share in the United States from 2014 to 2021](https://datasetsearch.research.google.com/search?src=2&query=Major%20beer%20vendor%20market%20share%20in%20the%20United%20States%20from%202014%20to%202021&docid=L2cvMTFyOW1iYm5jdw%3D%3D)** <br>
Dataset containing local US beer vendor market shares from 2014 to 2021, could show correlation between local and nation-wide brewery success.




## Methods :wrench: :hammer:
### Data Handling:
Extract the files content using pandas to recombine data and obtain matched location dataset. The files contain user, brewery, and beer data, as well as .txt files containing user reviews and ratings. We extract the reviews and ratings from txt files and join them to the user and brewery data to obtain a dataframe containing every review's user and brewery location among others. We then split the data in two: one dataframe containing local reviews, another containing outsider reviews.

### Exploratory Data Analysis:
* **Visualise and explore the distribution of the datasets' different attributes using histograms and map visualizations. Get familiar with the data and ensure feasibility of the project. One notable visualization is the local reviews map shown below:


* **Sentiment Analysis** : In order to analyze the validity of the reviews present in the datasets, use a sentiment analysis model. We have picked a Transformer model and then evaluated it on random subsets of the beer reviews. As expected, negative reviews (i.e. Bad Overall Score) contained mostly negative words (vice versa for positive reviews (Overall Score = 5)). For the next milestone, we anticipate using this model to confirm whether a given review is legitimate or not.



## Proposed Timeline :hourglass_flowing_sand:
* Week 10: Sentiment Analysis : Check if users are prone to give positive ratings to their homestate beers.
* Week 11: Hypothesis testing : Check whether a review sentiment correlates with proposed user's score.
* Week 12: Debugging + Optimizing implementation.
* Week 13: Visualizations for datastory.
* Week 14: Wrapping up for final submission.

## Team Organization :snake:
* Ilker, Mark: Machine Learning (sentiment analysis).
* Ralph, Emna: Data Exploration, Hypothesis testing and Visualizations.
