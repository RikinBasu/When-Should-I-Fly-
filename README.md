# When Should I Fly ?
To build recommendation system for users who wish to fly domestically. We hope to simplify the flight booking process for our users by providing insights on flight delays based on certain user flight details.

The dataset we have is for flight delays. It shows that there have been 2201 airplane flights in January 2004, flying from the Washington DC area into the NYC area. The main characteristic of interest (the response) is if a flight has been delayed by more than 15 min (coded as 0 for no delay, and 1 for delay) or not. The explanatory variables include three different arrival airports—John F Kennedy, Newark, and LaGuardia. The three different departure airports are Reagan, Dulles, and Baltimore, along with eight carriers, and a categorical variable for 16 different hours of departure (6 am to 10 pm). The other variables include weather conditions (0 = good/1 = bad) and day of the week (1 for Sunday and Monday and 0 for all other days).

Checking for missing values:

 ![image](https://user-images.githubusercontent.com/127339967/223868296-a23ec07c-8182-4417-ae7e-2a96dee9c18b.png)

As we can see that our dataset has no missing values. 

Variable Selection

Variable selection is an important aspect because it helps in building predictive models free from correlated variables, biases and unwanted noise. The Boruta Algorithm is a feature selection algorithm.


Predictive Analytics Techniques

We will be using the following models for classification problem at hand:

1.	Logistic regression
2.	Support vector machines
3.	Decision tree
4.	Random forest

 We now do a detailed comparison for all 4 models compiled above:
 
![image](https://user-images.githubusercontent.com/127339967/223869244-f1653172-6675-455f-b7fe-9606e4ecf5dc.png)

From the above comparison we can see that Random Forest classifier performs the best out all the 4 models.

We first saved the Random Forest Classifier trained above using the joblib library.
![image](https://user-images.githubusercontent.com/127339967/223869365-75e5bb30-7918-438b-9ad8-97aad52f4092.png)


We now launch the website using the Streamlit API as shown below :

![image](https://user-images.githubusercontent.com/127339967/223869402-84ee0a27-2ba3-4556-b833-7334fca3fb81.png)

Lets get a closer look:

![image](https://user-images.githubusercontent.com/127339967/223870329-5f33a1b9-f52d-4e7f-9b73-909aa11b29ac.png)

