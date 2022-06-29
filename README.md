Portfolio

Welcome to my portfolio! Here are some of the projects I've been working on in the past couple of months.

Feel free to reach out to me at georgy.busov@gmail.com if you have any questions or comments. And yes, this theme is called "hacker".



# [Project 1: Deal my car](https://github.com/georgybusov/Deal-my-car)

**INTRO:**

Everyone knows that car dealerships (especially used ones) leverage market info against their customers to extract an extremely high profit margin from both their sales and purchases of vehicles.
They will value trade-ins from their customers at no more than around 40% of the car's current market value, and most people will let it go for that price because they think that is their best option.

I decided to take on this project to help people see what price a dealer would try to sell their car for after they accept it as a trade in, so that they can know exactly how much they should ask for when negotiating their trade-in.

**OVERVIEW**

- Scraping car data from Kijiji ads posted by dealerships in the Calgary area
- Cleaning the data
- Performing some EDA to identify key features and trends
- Selecting and training a regression model
- Creating a clunky UI for people to see what dealers would price their cars at (will develop a nicer front-end API soon)

Here is an example of a prediction:

![alt text](https://github.com/bgosha24/Deal-my-car/blob/main/dealmycarexample1.jpg?raw=true)



# [Project 2: Predicting House Prices](https://github.com/georgybusov/Predicting-house-prices)


**INTRO:**

In this notebook I went over the Ames Housing Dataset and attempted to create a linear regression model that is able to predict the price of a house with a 
7.85% error.

I later used this notebook for my submission in [this kaggle competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) and was able to score in the top 16.8% of participants.

![alt text](https://github.com/bgosha24/Predicting-house-prices/blob/main/ames.jpg?raw=true)

**OVERVIEW**

- Definitely ranked up my feature engineering skills and showed me the important of domain knowledge for building machine learning models
- Helped me raise my expertise with model selection and particularily the benefits of using GridSearchCV
- Gave me an understanding of what it is like to go from a raw dataset that needs to be heavily processed and manipulated to a ready to deploy model



# [Project 3: Image Recognition with Pytorch](https://github.com/georgybusov/Image-Recognition-with-PyTorch)


**INTRO:**

This is my first run-in with PyTorch. I built a Convolutional Neural Network to predict what digit is being displayed in an image. The dataset used for this is PyTorch's built in MNIST dataset that has 70k images. 

This is what an image looks like, here is the number 9:

![alt text](https://github.com/georgybusov/Image-Recognition-with-PyTorch/blob/main/nine.jpg?raw=true)

**OVERVIEW**
- Create loaders and define layers
- Create a tensor
- Perform first convolution/activation and run pooling layer
- Perform second convolution/activation and run pooling layer
- Preprocessing
- Model creation/training
- Evaluate accuracy and check what images weren't correctly predicted



Here are some of the images that could not be predicted... probably the work of a doctor.

![alt text](https://github.com/georgybusov/Image-Recognition-with-PyTorch/blob/main/badnumbers.jpg?raw=true)



# [Project 4: Fandango vs The People](https://github.com/georgybusov/Fandango-vs-The-People)


**INTRO:**

Would you rather watch a movie with an internet rating of 1.5/5 or 4/5 stars? 

Unless like my brother, you participate in a weekly social event named "Trashy Tuesday" which consists of getting a little "influenced" with a couple of friends and watching the lowest rated movies of all time to laugh at the absurdity of the plot or the bad acting, I would assume you would watch the movie that is 4/5 stars.
And with this assumption, comes the realization that people would rather watch movies with the highest ratings.

But what happens when you are a website that provides movie ratings, and also sell online tickets for those movies? One could say that it would logically makes sense for you to rate movies higher to sell more ticket. This is exactly what a company called Fandango was suspected of doing on their website and I would like to launch a further investigation to prove it.


**OVERVIEW**

- Analyze Fandango's movie ratings through visualization and statistical measures
- Find potential inconsistencies in Fandango's measurement formulas
- Comapre Fandango's movie ratings against other top movie rating sites like RottenTomatoes, IMDB, Metacritic
- Decide whether Fandango is providing inflated movie rating to sell more tickets on their website



**Example:**
*Here are the lowest rated films on each site*

![alt text](https://github.com/bgosha24/Fandango-vs-The-People/blob/main/fandango1.jpg?raw=true)


*Most of Fandango's lowest rated films are 3.75/5 stars... They are clearly inflating their ratings.*


# [Project 5: Predicting Titanic Survivors](https://github.com/georgybusov/Predicting-Titanic-Survivors)

**INTRO:**

In this project I tried out the Titanic competition on Kaggle. My first submission was able to predict survivors with a 75% accuracy which is surprisingly only within the top 85% of results. After playing around with GridSearch and classifiers other than just Logistic Regression I was able to pump up that number to a 77% accuracy and get into the top 60% of all submissions. I was quite unsatisfied with these results and tossed it up to my lack of model tuning expertise. However, even after copying the parameters of a top 2% performer on the leaderboard (83% accuracy) my model's performance only increased to 77.99%. This made me reconsider how big the difference in classifying power is between models and that maybe I need to look at other optimization options.

After reconsidering some features of the dataset I decided to make some changes in my approach to feature engineering. Instead of dropping columns I decided to try to either fill or create new features that would replace them.

**OVERVIEW**

- Data Cleaning
- EDA
- Feature selection and extraction
- Preprocessing
- Model Selection



_**Lessons learned:**_

- Having a clean dataset with thoughtful feature engineering is more important than optimizing models as it yields a larger jump in performance. I tried to use cross_val_score to find models that perform best on this dataset and despite trying lots of different param combinations with GridSearchCV I was only able to get a 2% increase which may take me from the 85th percentile to the 25th on the leaderboard, but definitely doesn't do much for my ability to predict survivors on the Titanic.

- Distributions are very important as they can significantly aid in your model's performance. My final model after perfomring a log1p normalization gave me a top 5% score in this competition

- If a feature seems to be useless or too hard to interpret, it is best to break it up into digestible features. This was the case for me when I changed the Cabin feature into cabin_adv which is cabin letters and cabin_multiple which signifies a passenger with multiple cabins.

- Some features are meant to be paired up as they are heavily correlated. The Sibling/Spouse and Parent/Child features were combined to give room to 2 new features named FamilySize and Alone

- Some numerical features could be used to create categorical features. I used age to determine if a passenger was a child (15 and younger) or an adult.

- Don't rush into model selection and instead explore the dataset and see how you can make it as easy as possible for model to digest.

