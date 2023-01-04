# Google-pagerank-algorithm-on-Wikipedia

## Introduction :-
While searching in Google, have you wondered how Google shows up certain websites at top of the other websites? Well if you haven't wondered, this project covers one of the most  interesting algorithm called ***Pagerank***  which plays crucial role in the **recommendation of websites by Google**. 

### What is Pagerank? :-
It is name of an algorithm in which Google uses it's own formula for ranking websites. The higher is the rank of an website, that much higher is the chance of it appearing at first in reccomendations.

### How is it calculated?:-
* At first a graph is constructed in which main website topic is the source and all the hyperlinks are destination nodes connected to source.
* Next by using the below formula iteratively we will calucate page ranks of all the sources without anu deadends( the nodes from which there is no outgoing edge).

 ![This is an image](https://miro.medium.com/max/1400/1*z6PTV9WxrxcxnLf4eftXEg.png)

***(Here important note is ranks are probabilities of importances, so sum of all ranks will be approxly 1 but not exactly 1 as it depriates iteration after iteration.)***
* After performing iterations the page with highest rank will be displayed first.

## Dataset used :- 
A huge dataset of 40k Wikipedia articles with 1 million hyperlinks ***(which is in dataset.zip)*** are used for output and mini dataset of 2k wikipedia articles with 100k hyperlinks ***(which is in dataset-mini.zip)*** are used for building the model and testing purposes.

## Model implementation and outputs :- 
* How the model is implemented is well documented in code in form of comments.
* Top 25 pages with ranks are displayed as output implying they would appear most often in recommender systems of Google search engine.


