# Beers :beer:
Or America's latest obsession 

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
This will help us analyse ranking and word beer consumptions and have an idea on the market shares over time.

* **[Craft breweries per capita in 2021  in the US](https://datasetsearch.research.google.com/search?src=2&query=U.S.%20craft%20beer%20breweries%20per%20capita%202021%2C%20by%20state&docid=L2cvMTFwd2Y1NzR5NA%3D%3D)** <br>
The number of craft breweries per capita illustrates the involvement of the users in the beer market and reflects the potential bias for their hometown beers.
* **[ Major beer vendor market share in the United States from 2014 to 2021](https://datasetsearch.research.google.com/search?src=2&query=Major%20beer%20vendor%20market%20share%20in%20the%20United%20States%20from%202014%20to%202021&docid=L2cvMTFyOW1iYm5jdw%3D%3D)** <br>
This is to have an idea on the leading beer suppliers in the US overtime.




## Methods :wrench: :hammer:
### Data Handling:
Using pandas to extract the files content and recombine data to obtain matched location dataset.
### EDA:
* **Histogram plots** to visualise and explore the distributions of the number of ratings and number of reviews. We have also plotted the histograms of beer type to evaluate the distributions of beers by style. We noticed that most of the beer brands have 1-2 ratings. As for the beer style, we have noticed that most beers fall into 3-4 most popular categories (e.g. American IPA, American Pale Ale, Farmhouse Ale ...).
* **Statistical moments** : means and medians to study the shape of the distributions. We discovered that the distributions of both the number of reviews and number of ratings with respect to the beer type are long tailed.
bias analysis using transformer  to test our hypothesis 
* **Sentiment Analysis** : In order to analyze the validity of the reviews present in the datasets, we decided to use a sentiment analysis model. We have picked a Transformer model and then evaluated it on random subsets of the beer reviews. As expected, negative reviews (i.e. Bad Overall Score) contained mostly negative words (vice versa for positive reviews (Overall Score = 5)). For the next milestone, we anticipate using this model to confirm whether a given review is legitimate or not.



## Proposed Timeline :hourglass_flowing_sand:

## Team Organization :snake:

