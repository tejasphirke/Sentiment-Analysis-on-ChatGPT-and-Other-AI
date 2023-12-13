# Sentiment Analysis on ChatGPT and Other-AI
Using Python, analyzed sentiment based on ChatGPT reviews. Reviews were scraped from the google playstore api.

# Defining Hypothesis and Details about Data
## Data Collection 
Data collected from google play store api. The data is analysed till november but it is a real time data where the data. For other AI, we consider Bing for comparing with ChatGPT reviews. Data is collected from August 2022 till November 2023. ChatGPT application itself came in the year 2022 end.

## Data Cleaning 
For Data Cleaning we came up with a function which removes url, phone numbers, emails, numbers or any word which does not make any sense. We used NLP techniques to get the clean data along with that we removed null values. Converting Dates to proper data time format because later it would be helpful to do analysis on date to plot the time trend for the different versions of chatGPT.

## Data Exploration
To get the gist of data and story behind the data is very important, so we analysed data by finding out histogram, summary of the data, value counts. Used Pearson Coefficient as well Point Biseral Coefficient to know the relation between the variables. 

# Techniques used on Data
## NLP
Used TextBlob to get sentiments of the reviews. Used polarity as well to find whether the reviews are positive, negative or neutral. By using TextBlob, I found that people are have positive feedback most of the times. However, there were very few people faced issues while accessing chatgpt. 
So based on the data, we analysed the replyContent(reply given to the user by organization of chatGPT organization)

## Time-Series Analysis
This is based on the different versions of chatgpt. 
- We filtered out different versions which were present in the google playstore api. There were two major versions: 1.0 and 1.2023
- Plotted line graph based on the average sentiment score and date to get the idea of sentiment between two major versions of chatgpt. 

## TF-IDF
We build the word cloud on various columns in the data, we found most of the words are positive. Used LDA to perform the analysis on text and filtered out 5 topics saw the probabilities of most occuring words in those buckets.




