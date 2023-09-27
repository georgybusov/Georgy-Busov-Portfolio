# WELCOME!

Here we have some of the projects I've been working on in the past couple of months.

Feel free to reach out to me at georgy.busov@gmail.com if you have any questions or comments.


# [Project 1: Sales Predictions](https://github.com/georgybusov/Case-Study-Sales-Prediction)

**INTRO:**

This was a case study for a course I did where we were tasked with predicting sales for a retailer based on their historical sales. 

I loved this project because it prepared me really well for when I actually had to do this for one of my employers, and because it helped me translate my theoretical knowledge of ML in Python into something that offers business value.

**OVERVIEW**

- Loading in the data from csv files
- Data cleaning and wrangling
- Performing some EDA to identify key features and trends
- Feature Engineering
- Finding the right regression model
- Tuning models and comparing results vs baseline
  
I was able to predict weekly sales within 94.5% accuracy with my final tuned model. 


![alt text](https://github.com/bgosha24/Deal-my-car/blob/main/final_prediction.png?raw=true)



# [Project 2: Deal my car](https://github.com/georgybusov/Deal-my-car)

**INTRO:**

Everyone knows that car dealerships (especially used ones) leverage market info against their customers to extract an extremely high profit margin from both their sales and purchases of vehicles.
They will value trade-ins from their customers at no more than around 40% of the car's current market value, and most people will let it go for that price because they think that is their best option.

I decided to take on this project to help people see what price a dealer would try to sell their car for after they accept it as a trade in, so that they can know exactly how much they should ask for when negotiating their trade-in.

Here is an example of a prediction:

![alt text](https://github.com/bgosha24/Deal-my-car/blob/main/dealmycarexample1.jpg?raw=true)

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
