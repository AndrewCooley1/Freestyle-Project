# Freestyle-Project

Freestyle Project


Group Members:
Vivek Agarwal- vka244@stern.nyu.edu
Emily Hoyland- ech435@stern.nyu.edu
Andrew Cooley- ac8896@stern.nyu.edu

User Needs/Target Segment: 
Investors who need information regarding fluctuation in company perception/news so that they can determine whether they should invest or not at a given time.

Aim: 

The system will pull information from financial news API (finviz.com). This program will help investors who are looking for daily “sentiment” data on stocks of their choosing. They are interested in whether the stocks are referenced in the news as positive, negative or neutral for the day. This will help them decide if they want to buy, sell or hold the security based on overall sentiment. We understand investing has many risks and should involve fundamental analysis as well, however, this web based tool can be used to obtain a quick and general feeling about the stock in question. 

General Thesis of App:
To provide the user with a positive, negative or neutral view on user input securities based on financial news.

Information Inputs: Financial news API (finviz.com), user input of stock name (ticker symbol)

Information Outputs: For an user-entered stock name, a web-based Application will display an output between -1 and 1 to indicate general sentiments about whether the company is trending positive or negative in the news on a given day. The application will use the following scale to indicate sentiment:

-1 to -.51= Negative sentiment
0.5 to -0.50 = Neutral sentiment
0.51 to 1= Positive sentiment.


Motivation - We first started with the idea of using an API for filtering the news of the death of a CEO of a fortune 500 company. Given the small probability of such an event happening on a  regular basis, we pivoted to an idea of using an API to generate a sentiment score for stocks (that a user is interested in). Based on this score the investor would decide, if they want to invest in the stock for the day. 

What will our final product look like? - The final product will be a webapp that allows the user to enter the stock name and generate the scores for the day for the chosen stock. 

Technical Feasibility Analysis
The proposed webapp can be implemented in python using python packages like VADER, FLAIR etc. that provide sentiment scores for the text data. We have researched the methods to use the VADER package (https://github.com/cjhutto/vaderSentiment) to determine the sentiment scores and need to further study in detail about the FLAIR (https://github.com/flairNLP/flair) package. We are still studying sentiment analysis using python packages. 
Feature Prioritization
Are you able to break your system's components up into smaller, more easily manageable pieces, or "features" such that someone could work on one logically-related feature at a time? 
API input 
User input
Look-up function
Data interpretation (given a -1 to 1 rating)
Sentiment Generation (invest or not invest)
Web display
 
Which feature(s) are the most important to implement, and which are the "nice to haves"? 
Important:
API Input
User Input
API Lookup
Data Interpretation
Sentiment Generation and Output
Nice to Have: 
Recap email providing results from user session
Would need to store all user inputs in a list to generate summary (or “receipt”) from session
Email input/Sendgrid 
 
Which features will you implement first, and why? 
The API input must be implemented first, in order to compile data for the user input to be able to provide any lookup function or for a sentiment to be generated. User input and subsequent lookup function must be implemented next in order to ensure that it is pulling the correct corresponding information. User inputs will be entered one at a time and stored in a list to generate an investment analysis in a “receipt” form at the end of use, showing the results for each. Interpretation of data followed by sentiment generation based on that interpretation should come next in order to generate information that will be useful to a user. Lastly, it must be presented in a user-friendly format. 
 
If working in a group, how do you propose to collaborate - for example, will you mostly follow a "pair-programming" strategy or a "divide and conquer" strategy?
Created a repository on Github.com and subsequent system for naming branches to indicate to whom each belongs, as well as content being worked on in each branch. We are planning to do a hybrid or pair-programming and divide and conquer strategies.
