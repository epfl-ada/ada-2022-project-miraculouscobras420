
The Cobras: Ilker Gul, Mark Tropin, Emna Fendri, Ralph El Haddad.
# Beer :beer:
Or America's latest obsession...

## Data Story Link
Here you can access to our **datastory**:<br>
**[Miraculous Cobras 420 ADA Datastory](https://ralph-elhaddad.github.io/miraculouscobras420-ada/american-beer-heritage)**<br>


## Abstract :page_facing_up:
The sense of belonging has always been an important human factor, whether it’s in opinion formation, judgment, or decision making. Cleveland people, for example, will usually root for their local NFL team, the Browns, even though that same team ends up last pretty much every season! The sense of belonging does not exclusively mean an emotional connection though, it might also express a sort of camaraderie, a sense of mutual support in financial matters. But how does this apply to beers? <br>
Beers are the most social alcoholic drinks out there: whether it’s with friends or coworkers, beers are the usual go-to in outdoor social gatherings. But how easy is it to dissociate one’s opinion about the beer from the memories that come with it? Does the sense of belonging to a group influence our supposedly impartial judgment of the product? In this project, we turn to the datasets provided by 2 major beer rating websites, BeerAdvocate and RateBeer, in search of user bias towards “local” breweries. A brewery is labeled “local” if it is located in the same state as the user, and “outsider” otherwise.



## Research Questions :thinking:
* Does the brewery's location influence users' reviews? <br>
* Do consumers prefer local or foreign beers? <br>
* How important is local support for breweries to increase sales in foreign states? <br>
* How does the burgeoning of craft beer breweries reflect users' bias for their hometown beers? 


## Additional Datasets :books:


* **[beer - worldwide](https://www.statista.com/outlook/cmo/alcoholic-drinks/beer/worldwide)** <br>
Dataset containing world ranking in beer consumption and global beer market shares between 2012 and 2022.

* **[Craft breweries per capita in 2021  in the US](https://datasetsearch.research.google.com/search?src=2&query=U.S.%20craft%20beer%20breweries%20per%20capita%202021%2C%20by%20state&docid=L2cvMTFwd2Y1NzR5NA%3D%3D)** <br>
Dataset containing craft breweries per capita data in the UD in year 2021, could illustrate the involvement of the users in the beer market and reflect potential bias towards their hometown beers.
* **[ Major beer vendor market share in the United States from 2014 to 2021](https://datasetsearch.research.google.com/search?src=2&query=Major%20beer%20vendor%20market%20share%20in%20the%20United%20States%20from%202014%20to%202021&docid=L2cvMTFyOW1iYm5jdw%3D%3D)** <br>
Dataset containing local US beer vendor market shares from 2014 to 2021, could show correlation between local and nation-wide brewery success.

* **[State Population estimation in the US in 2021](https://www.census.gov/data/tables/time-series/demo/popest/2020s-state-total.html)** <br>
Annual estimates of the Resident population for the Unites States regions. Stats displayed in columns and rows.





## Methods :wrench: :hammer:
### Data Handling:
Extract the files content using pandas to recombine data and obtain matched location dataset. The files contain user, brewery, and beer data, as well as .txt files containing user reviews and ratings. We extract the reviews and ratings from txt files and join them to the user and brewery data to obtain a dataframe containing every review's user and brewery location among others. We then split the data in two: one dataframe containing local reviews, another containing outsider reviews.

### Exploratory Data Analysis:
Visualise and explore the distribution of the datasets' different attributes using histograms and map visualizations. Get familiar with the data and ensure feasibility of the project. One notable visualization is the local reviews map shown below:

![map RB](https://user-images.githubusercontent.com/62402657/202795637-a3214126-d35d-46db-bc85-ad5128718104.png)


### Ale vs. Lager:

Ale and Lager are the two main categories of beer that are consumed in the US. Ale was originally brought to the US by the British and the Dutch, while Lager was brought 200 years later by the German immigrants. We decided to analyze whether this historical detail has an effect on beer consumption in the "German belt" today.

To answer this question, we visualize the US map where each state is mapped to a ratio. The ratio is the number of local reviews within a particular state divided by the corresponding state population multiplied by a 1000. Note that we define a "local review" as a review of a beer that was produced in the user's state.

$\frac{\text{No. of local reviews in state A}}{\text{population of state A}} \cdot 1000$

This ratio results in the number of local reviews per 1000 citizens.  

### Traces of Prohibition:

On to a more recent topic. We know the influence of the Prohibition era, which happened 100 years ago, is still prevalent in the way Americans consume beer today, since some states still have dry counties where alcohol is prohibited. 

We believe that ratings of beer in dry states are generally less favorable and are especially unfavorable for beer from wet states. 
Two statistical tests are performed to either support or contradict this claim: a linear regression that forecasts the beer rating given a categorical attribute as input and a separate t-test on the sample means.

### Sentiment Analysis: 
In order to analyze the validity of the reviews present in the datasets, use a sentiment analysis model. We have picked a Transformer model and then evaluated it on random subsets of the beer reviews. As expected, negative reviews (i.e. Bad Overall Score) contained mostly negative words (vice versa for positive reviews (Overall Score = 5)). For the next milestone, we anticipate using this model to confirm whether a given review is legitimate or not.

**ILKER ILKER ILKER**

### Hypothesis testing:
To study the effect of the users location relative to the brewery location, we conduct two types of statistical tests. First, we fit linear models linking these categorical attributes to the beer rating to see if there is any correlation between the two. Second, we generated independent t-tests to check whether the difference between the two datasets is statistically significant.


## Proposed Timeline :hourglass_flowing_sand:
* Week 10: Sentiment Analysis : Check if users are prone to give positive ratings to their homestate beers.
* Week 11: Hypothesis testing : Check whether a review sentiment correlates with proposed user's score.
* Week 12: Debugging + Optimizing implementation.
* Week 13: Visualizations for datastory.
* Week 14: Wrapping up for final submission.

## Team Organization :snake:

* Ralph: Data story, web development, Project Manager
* Emna: Hypothesis testing, data story
* Ilker: Sentiment analysis, data story
* Mark: Hypothesis testing, data story

<img width="397" alt="logo" src="https://user-images.githubusercontent.com/62402657/209407022-4545a95a-57d4-415a-82cd-913f901f1f26.png">

