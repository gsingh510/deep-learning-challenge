# deep-learning-challenge
1.	Overview of the analysis: Explain the purpose of this analysis.
Introduction
The nonprofit foundation Alphabet Soup wants tool for selecting applicants for funding with highest chances of success in their ventures. Utilizing our knowledge of machine learning and neural networks, we will use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.   

Results
Data Preprocessing:
What variable(s) are the target(s) for your model? 
The column from application known as “IS_SUCCESSFUL” is the target variable. Success is what we are trying to predict as it shows effective use of money. 

What variable(s) are the features for your model?
•	EIN and NAME—Identification columns
•	APPLICATION_TYPE—Alphabet Soup application type
•	AFFILIATION—Affiliated sector of industry
•	CLASSIFICATION—Government organization classification
•	USE_CASE—Use case for funding
•	ORGANIZATION—Organization type
•	STATUS—Active status
•	INCOME_AMT—Income classification
•	SPECIAL_CONSIDERATIONS—Special considerations for application
•	ASK_AMT—Funding amount requested
•	IS_SUCCESSFUL—Was the money used effectively
What variable(s) should be removed from the input data because they are neither targets nor features?
•	The columns that should be removed from the input data are “EIN” and “NAME”. These are identical columns that typically provide unique identifiers for each organization. Since these have no direct impact on the target variable they can be dropped, and will not result on any affect with the model’s accuracy. 
Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?

•	In the 1st neural network model, I used a 2-layer construction with a specific choice for neurons, layers, and activation function. 


 


By selecting 80 neurons in the 1st hidden layer, and 30 in the 2nd hidden layer with the ReLU activation function the goal was to create a model with complexity to capture and learn useful patterns in the data. ReLU also helps to introduce non-linearity and allows the model to learn relationships between the input features and target variable. 

	Overall, the model with these options creates a balanced environment to build off of and generate a classification task. 

 
Were you able to achieve the target model performance?
•	Per the screenshot below you can see I was only able to achieve a 73% accuracy rate. Which was not aligned with the target of 75%.

 

What steps did you take in your attempts to increase model performance?
•	The 1st step I took was to add a higher number of neurons. However, as the images show below the accuracy of the data did not increase and still resulted in 73%. 
 
 

•	The 2nd step was to add another layer to the model. Adding layers can provide the model with more capacity to capture and illustrate relationships with the data. However, the result did was still at 73% as seen in the images. 
 
 
•	In the 3rd interaction I decided to increase the neuron and layer count, and double epoch to 200 now. Overall, this resulted in an accuracy score of 73% again as per the images below. Here I believe I have hit a solid wall, and should have run a new activation function to see if that would result a higher accuracy. 
  

 


Conclusion
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

The learning model I created was unable to surpass the 73% accuracy score. Thus, it did not meet the expected accuracy score of 75% or higher. For the future these are a couple of recommendations I could execute for a higher score:

1.	More Data:
	The most important action that could be taken is increasing the dataset. The machine learning model requires a larger and diverse set of data in order to provide a more efficient and accurate prediction. Thus, more data could lead to higher accuracy scores. 
2.	Explore other machine learning algorithms:
	Utilizing different algorithms such as, Decision Tree and Random Forest could lead to a higher accuracy score. For example, Random Forest measures feature value based on how effectively the individual feature contributes to the prediction. Thus, allowing one to focus on only the primary columns that have the most informative features with potential to improve the accuracy. 

To conclude, to reach higher accuracy in the deep learning model we need a bigger data set and exploring another algorithm. Each step would help improve the model’s ability to capture relevant patterns and bypass the unnecessary data, leading to a higher accuracy in the classification problem. With these steps and fine tuning, it is possible to reach 75% or more accuracy. 



![image](https://github.com/gsingh510/deep-learning-challenge/assets/22353592/a37646b3-ea4a-45c2-82b9-a2d7d6b54db6)
