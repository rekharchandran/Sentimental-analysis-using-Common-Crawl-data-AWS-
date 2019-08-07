# Sentimental-analysis-using-Common-Crawl-data
### Introduction
Sentiment analysis is a process that filters opinions, emotions from texts, tweets and other sources of natural languages.
### Objective
Using the cloud computing platform provided by Amazon Web Services 
1) Collect and develop a data matrix in the range of 20 thousand instances of relevant web documents from the Common Crawl .
 2) Create a model to predict Sentiment analysis between Iphone and Samsung Galaxy. 
 
 ### Project Background
 •	A government health agency needs to create a suite of smart phone medical apps for use by aid workers in developing countries and these apps will enable the aid workers to manage local health conditions by facilitating communication with medical professionals located elsewhere. 
 
•	The government agency requires that the app suite be bundled with one model of smart phone. 

•	To help them narrow their list down to one device, the project  examine the prevalence of positive and negative attitudes toward these devices on the web. 

### Why AWS
AWS is a reliable, scalable, and inexpensive platform for the use of cloud applications and services and it will give you easy access to web data through one management console. The specific AWS services that you will be employing include Elastic Compute Cloud (EC2), Elastic MapReduce (EMR), and Simple Storage Service (S3). 

The Amazon Elastic Compute Cloud (EC2) is a web-based service that enables you to run application programs in the Amazon computing environment. EC2 can serve as a practically unlimited set of virtual machines. 

### General Overview of the Data
This information has been extracted from the Common Crawl repository through Amazon Web Services , using Hadoop framework and MapReduce technologies. The information extracted was raw sentiment counts from individual web pages.

### Data Preparation
•	Used EMR to collect the web data to analyze the general sentiment towards the smart Phones and complied it into a csv file called the Large Matrix
•	This involved first running the mapper and reducer scripts on one WET file of Common Crawl data in EMR using the EMR console
•	Then ran the scripts in EMR on 255 Common Crawl WET files using the EMR Command Line Interface. 
•	Then using concatenating script to compile the Common Crawl data collected and to create the Large Matrix.

### Predective Models
One optimized model is used to predict the overall sentiment toward iPhones and one optimized model to predict overall sentiment toward Samsung Galaxy handsets. 
The models used are  C5.0, KKNN, SVM  and RandomForest

### Results for iPhone
The random forest tree algorithms provided a good performance compared with other classifiers  approaches such as SVM, KKNN and C50
                      Accuracy : 0.79306  and Kappa : 0.6076 .
                      
### Results for Samsung Galaxy                      
 Like in the case of iPhone, The random forest tree algorithms provided a good performance .
                         Accuracy : 0.8017 and Kappa : 0.60707 
                         
### Conclusions
•	Sentiment distribution indicates that iphone has more good postive reviews.

•	Whilst there are more people with no opinion about iphone and Galaxy.

 An attempt was made to find out out every combination of feature subsets using  RFE function with random forest and the returned final list of recommended features  are as below;
 
   for iphone 
   
 The top 5 variables for Iphone  (out of 11): Iphone, google android,  Samsung galaxy, Iphone dispos, HTC phone.
 
  For Galaxy
  
The top 5 variables  for Galaxy were Iphone, google android, Samsung galaxy, Iphone dispos, Iphone disunc





