# credit_risk
Create a RESTful API for a machine learning credit model in R

R is the language many data scientists use to create machine learning models but is rarely used by other types of programmers. As a remedy for the problem, I will create a RESTful API using only open source libraries and see that other programming languages can interact with the API. 

To make the example a bit more interesting, I created a machine learning model in the simplest manner possible. I have worked with an online lending company before so I created a model that predicts whether a person is going to pay off a loan using the famous German credit data. Building a predictive model is a sophisticated process of combining arts, science and specialized business knowledge; however, in this example, I will build it without worrying too much about all these details for the sake of simplicity.
  
  
Test to make sure it works
 Issue the following command in a terminal:

	curl -X POST -d '{"Status.of.existing.checking.account": "A11", "Duration.in.month": 24, "Credit.history": "A32", "Savings.account.bonds": "A63"}' -H 'Content-Type: application/json' localhost:7000/predict

You will get:

	{"default.probability":0.6224}
