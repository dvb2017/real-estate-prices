# Real Estate Prices in King County, WA


## Table of Contents

1. List of files in repository
2. Business Case
3. Data Visualizations
4. Conclusions


## Files in repository  

* `presentation.pdf` - This contains my powerpoint presentation.
* `student.ipynb` - This is my Jupyter Notebook containing my code.
* `README.md` - Markdown file containing this text.
* `charts` - Folder containing all of the charts used in my presentation.
* `kc_house_data.csv` - CSV file containing the data used in my analysis.

## Business Case

My goal for this project was to build a model that is capable of predicting home prices for potential buyers.  More specifically, I was interested in leveraging geographic data in order to maximize cost-effectiveness based on location.  There were three main questions I wanted to address.

* What is the most cost-effective location in King County?
* How much can be saved based solely on location?
* Did any other savings opportunities appear in the data?

## Data Visualizations

Below I've included a few of the data visualizations I used throughout this process.  Since the data set included latitude and longitude values, presenting the data points as a sort of map made sense here.  The first graph shows the various home locations plotted and colored according to the 'price rating' that I assigned that zip code.  I marked the price epicenter with a red 'X'.  In the next graph, I have marked the most cost effective zip code according to the metric I used, as well as drawn a line between it and the epicenter.  The final graph is a bar chart showing the predicted savings for each season vs spring (which was calculated to be the most expensive season).

![all-zips](https://github.com/dvb2017/real-estate-prices/blob/main/charts/zip_map_marked.png)

![winner-zip](https://github.com/dvb2017/real-estate-prices/blob/main/charts/winner_map.png)

![season-savings](https://github.com/dvb2017/real-estate-prices/blob/main/charts/season_savings.png)

## Conclusions

After analyzing	the data and creating a model, I was able to answer each of the three questions.  

> What is the most cost-effective location in King County?

According to the model, the most cost-effective location is the 98023 ZIP code. This ZIP code had the lowest cost associated with its geographic location, and is predicted to be $141602 less expensive than the baseline model. This is where I would recommend purchasing a home for a buyer trying to minimize costs.

> How much can be saved based solely on location?

Quite a bit! The difference between the geographic costs in the 98023 ZIP code (the lowest) and the 98039 ZIP code (the highest) was $466857. This means that all else being equal, the model predicts that this cost difference is entirely derived from location. Due to the much higher price associated with the 98039 ZIP code, I would recommend not purchasing a home there if cost-effectiveness is the goal.

> Did any other savings opportunities appear in the data?

Yes, and it is an easy factor for a home buyer to control. The model predicts that Spring is the most expensive season to buy a home, and one simple way to lower costs is to buy during a different season. Specifically, I would recommend Autumn. This is the season with the highest predicted savings compared to Spring, coming in at approximately $24000.
