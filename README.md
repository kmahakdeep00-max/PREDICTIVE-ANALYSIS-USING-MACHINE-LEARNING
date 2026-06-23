# PREDICTIVE-ANALYSIS-USING-MACHINE-LEARNING 
Company Name: CodTech IT Solutions   
Intern Name: Mahakdeep Kaur  
Intern ID: CITS753 
Domain: Data Analytics  
Duration: 8 weeks 

During my internship with CodTech, I worked on a project using the dataset named train.csv. The main goal was simple but exciting: to build a machine learning model that could predict whether a passenger survived the Titanic disaster or not. This task gave me a chance to go through the full cycle of a data science project — from cleaning the data, training the model, checking how well it worked, and even saving the model for future use.

I started by loading the dataset with Pandas and looking at the columns. The data had details like passenger class, sex, age, fare, number of siblings/spouses, parents/children, and port of embarkation. Some values were missing, especially in the Age, Embarked, and Cabin columns. Since Cabin had too many missing entries, I dropped it. For Age, I filled the gaps with the median value, and for Embarked, I used the most common category. This way, the dataset became clean and ready to use.

Next, I had to make the data numeric because machine learning models don’t understand text directly. I converted the Sex column into numbers (male = 1, female = 0) and mapped the Embarked column into codes (C = 0, Q = 1, S = 2). After this step, the dataset was fully numeric, which meant I could train my model without issues.

For the features, I selected the most important ones: Pclass, Sex, Age, Fare, Embarked, SibSp, and Parch. The target column was Survived. These features made sense because they directly affect survival chances. For example, women and children had higher survival rates, and first‑class passengers had better chances compared to third‑class.

I then split the dataset into training and testing sets using train_test_split. I used 80% of the data for training and 20% for testing. The model I chose was Logistic Regression, which is perfect for binary classification problems like this. After training the model, I tested it on the unseen data.

The evaluation part was very important. The model gave me an accuracy of about 81%, which was pretty good. I also created a confusion matrix to see how many predictions were correct and how many were wrong. The heatmap of the confusion matrix made it easy to visualize the results. Along with that, I generated a classification report that showed precision, recall, and F1‑score. These metrics gave me a deeper understanding of how well the model was performing.

To make the project more interactive, I added visualizations. I plotted the confusion matrix as a heatmap using Seaborn and created a bar chart to show predictions for sample passengers. These visuals made the project look professional and easy to understand.

Finally, I did something very practical — I saved the trained model using the joblib library. This created a .pkl file of my Logistic Regression model. The benefit of saving the model is that I don’t need to train it again every time. I can simply load the saved file and start making predictions on new data.

Overall, this project taught me how to handle missing values, encode categorical data, train and evaluate models, and even save them for future use. It gave me confidence in Python, Pandas, Seaborn, Scikit‑learn, and Joblib. More importantly, it showed me how machine learning can be applied to real‑world problems in a structured way.
