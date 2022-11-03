# Final-Project

# Case Study: NLP Language

![real-state-project.jpeg](images/real-state-project.jpeg)


### Index:

* [Scenario](#section1)
* [Objective](#section2)
* [Approach](#section3)
* [First ideas](#section4)
* [In-Depth Analysis](#section5)
* [Conclusions](#section6)
* [Tableau](https://github.com/marimor62/Midtermproject-Housing/tree/main/Tableau)
* [SQL](https://github.com/marimor62/Midtermproject-Housing/tree/main/SQL)


<a id='section1'></a>
### Scenario

In this project we are working as analysts for a consultant company. Our company created a machine learning NLP model to predict whether the sms received is spam or not spam (ham). 
<a id='section2'></a>
### Objective

Short Message Service (SMS) is a text communication platform that allows mobile phone users to exchange short text messages (usually less than 160 7-bit characters) at a low cost. The amount of unsolicited commercial advertisements (spams) over SMS will be bigger since the cost of SMS will decrease.

SMS spam is not familiar compared to mail spam.
![Get and explore the data_ using Pandas library.jpg](images/Get and explore the data_ using Pandas library.jpg)


<a id='section3'></a>
### Approach

The dataset we used consists of information on 22,000 properties and contains historic data of houses sold between May 2014 to May 2015.
Our first approach consisted of:
                                * Importing the data
                                * Exploring the data (EDA Method)
                                * Data wrangling
                                * Data cleaning
                                * Check for multicolinearity

 <a id='section4'></a>
### First ideas

* The dataset for this project is a large text file established by a database of 5574 real text messages from UCI Machine Learning repository gathered in 2012 which contains:

* 425 SMS spam messages from the Grumbletext website (a UK forum in which cell phone users make public claims about SMS spam.
* 3375 SMS non-spam messages from the NUS SMS Corpus (NSC).
* 450 SMS non-spam messages from Caroline Tag's PhD Thesis.
* 1002 SMS non-spam and 322 spam messages from SMS Spam Corpus v.0.1 Big.


<img src="images/bathrooms definition.png"/>

* We decided to extract the month and quarter (not the year) as they will be more interesting for later analysis.

<a id='section5'></a>
### In-Depth Analysis

* We proceeded to realize the first iteration of our Machine Learning Model,
and our accuracy score R2 was relatively close to 1, so the model performs well, but we wanted to improved it.
<img src="images/r1.png"/>
* In the second iteration we did a preprocessing: We went through the standardization using StandardScaler to rescale and OneHotEncoder to process the categoricals. We got a better R2:
<img src="images/r2.png"/>
* We went through a third iteration, this time we did a rescale using the logarithmic method and we normalized the data using the Dummies Encoder
<img src="images/r3.png"/>


<a id='section6'></a>
### Tableau
[Link to tableau story](https://public.tableau.com/profile/marian.moreno#!/vizhome/Book1_16190202108450/Story1)

* Our assignment also included visualization with Tableau. We aimed to visualize our findings in a way that a non-technical audience would understand while maintaning a style that is both pleasing and unequivocal.

<img src="images/tableau1.png"/>



### SQL

By using SQL we tried to reach a deeper understanding of our dataset. We used queries to answer the questions posed by the real estate company. Follow the [link](https://github.com/marimor62/Midtermproject-Housing/blob/69d56c6d43351a4e1fe94910e53ff1ff00e6865f/SQL/proj_luna.sql) to dive into our queries. 
