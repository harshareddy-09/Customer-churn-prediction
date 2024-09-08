# Customer-churn-prediction
Customer churn refers to the process of customers discontinuing their use of a product or service. For businesses, especially those in industries such as telecommunications, banking, SaaS, and subscription-based services, predicting customer churn is crucial. It allows them to retain customers by identifying those who are likely to leave and taking proactive measures to improve retention.

## 🔴 Project Overview:

This project aims to develop a machine learning model to predict customer churn based on historical data. The primary goal is to identify customers who are at risk of leaving and to enable businesses to take corrective action. By understanding customer behavior patterns, the model can help businesses reduce churn and improve customer loyalty.

## 🔴 How It Works? 
1)Data Collection: Customer demographic, transactional, and interaction data is collected.
2)Feature Engineering: Key features that influence churn, such as customer activity, service usage, support interactions, and subscription details, are extracted.
3)Modeling: A supervised machine learning model is trained to predict churn. Algorithms like Logistic Regression, Decision Trees, Random Forest, or Gradient Boosting Machines (GBM) can be used.
4)Prediction: The model outputs a probability that a customer will churn, which allows businesses to prioritize retention efforts.

## 🔴 Key Features of the Model:
1)Churn Prediction: Predicts whether a customer is likely to churn or not.
2)Customer Segmentation: Segments customers based on their likelihood to churn.
3)Actionable Insights: Provides actionable insights on why a customer might churn, helping businesses implement targeted retention strategies.

## 🔴 Potential Algorithms:

1)Logistic Regression
2)Random Forest
3)Gradient Boosting
4)Neural Networks

## 🔴 How to Use?
1)Data Preprocessing: Prepare your dataset by cleaning and transforming the data.
2)Train Model: Train the machine learning model using historical data.
3)Predict Churn: Use the model to predict which customers are at risk of churning.
4)Interpret Results: Leverage the predictions to devise strategies for customer retention.

## 🔴 Business Value:
By predicting customer churn, businesses can:

1)Improve customer retention by targeting high-risk customers.
2)Reduce acquisition costs by focusing on keeping existing customers.
3)Increase revenue through better customer relationships and loyalty programs.


In this repository, we have performed the end to end Exploratory Data Analysis, and idenfitied the characteristics of the customers that are more likely to churn, and I have used them wisely to create a model, and lately, have deployed the model.

### 🟢 For EDA, please refer to : Churn Analysis - EDA.ipynb
### 🟢 For Model Building, please refer to: Churn Analysis - Model Building.ipynb
### 🟢 For Model Deployment, please refer to app.py


### 🔵 Creating the flask API

```
app = Flask("__name__")
```

The loadPage method calls our home.html.
```
@app.route("/")
def loadPage():
	return render_template('home.html', query="")
```

The predict method is our POST method, which is basically called when we pass all the inputs from our front end and click SUBMIT.
```
@app.route("/", methods=['POST'])
def predict():
```
  
The run() method of Flask class runs the application on the local development server.
```
app.run()
```


Yay, our model is ready, let’s test our bot.
The above given Python script is executed from Python shell.

Go to Anaconda Prompt, and run the below query.
```
python app.py
```


Below message in Python shell is seen, which indicates that our App is now hosted at http://127.0.0.1:5000/ or localhost:5000
```
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```


HERE'S HOW OUR FRONTEND LOOKS LIKE:

![Customer Retention](https://raw.githubusercontent.com/pik1989/MLProject-Churn-Analysis-And-Prediction-Model/main/images/Telco6.JPG)
