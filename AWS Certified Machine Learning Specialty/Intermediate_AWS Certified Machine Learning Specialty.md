# AWS Certified Machine Learning Specialty

# Exam 1

### Question 1:
The marketing team at an Enterprise SaaS company has determined that the cost of customer churn is much greater than the cost of customer retention for its existing customer base. To address this issue, the team worked on a classification model to predict if a customer is likely to churn and boiled it down to two model variants. Model A had 92% accuracy with 40 False Negatives (FN) and 100 False Positives (FP) whereas model B also had 92% accuracy with 100 FN and 40 FP. Which of the two models is more cost effective for the company :
* Both Model A and Model B are equally cost effective, as accuracy is same
* None of the Model A and Model B are cost effective. Company needs to try something different.
* Model A
* Model B

### Question 2:
What technique would you use in SageMaker to train a new model using an expanded dataset that contains an underlying pattern that was not accounted for in the previous training and which resulted in poor model performance:
* Beta Testing
* Incremental Training
* Batch Training
* Transfer Learning

### Question 3:
The data science team at a financial services company has created a multi-class classification model to segment the company’s customers into three tiers - Platinum, Gold and Silver. The confusion matrix for the underlying model was reported as follows:
* 0.47
* 0.50
* 0.56
* 0.67

### Question 4:
You want to secure the API calls made to your published Amazon SageMaker model endpoints from your customer VPC. By default, these API calls traverse the public network to the request router. What measures would you take to address this issue:
* Use AWS-SSE for private connectivity between the customer's VPC and the request router to access hosted model endpoints.
* Use Amazon Virtual Private Cloud interface endpoints powered by AWS PrivateLink for private connectivity between the customer's VPC and the request router to access hosted model endpoints.
* Use SSH for private connectivity between the customer's VPC and the request router to access hosted model endpoints.
* Amazon SageMaker ensures that machine learning (ML) model artifacts and other system artifacts are encrypted in transit, so no special measures are required

### Question 5:
As an ML Specialist, you observe that one of the features used in a SageMaker Linear Learner model had 30% missing data. You also believe that this specific feature was somehow related to a few other features in the data-set. Which technique would you use to address the missing data:
* Use multiple imputations approach via a supervised learning technique that uses other features to figure out the imputed value
* Replace the missing values with median
* Replace the missing values with mean
* Drop the missing feature as 30% missing data would severely distort the overall training data

### Question 6:
A ride-hailing company needs to ingest and store certain attributes of real-time automobile health data which is in JSON format. The company does not want to manage the underlying infrastructure and it wants the data to be available for visualization on a near real time basis. As an ML specialist, what is your recommendation:
* Ingest the data using Kinesis Data Streams and use a Lambda function to write the stream into S3. Launch a Glue ETL Job every 15 minutes to select specific attributes from the source data and write the output in another S3 location. Further pipe this processed data into QuickSight for visualizations
* Ingest the data using Kinesis Firehose that uses a Lambda function to write the selected attributes from the input data stream into an S3 location. Further pipe this processed data into QuickSight for visualizations
* Ingest the data into S3 using Kinesis Firehose. Launch a Glue ETL Job every 15 minutes to write S3 data into RDS. Use RDS Connector to visualize this data in QuickSight
* Ingest the data using a Spark Streaming application running on an EMR cluster. The output data with selected attributes is written in JSON format on S3. Further pipe this data as source into QuickSight for visualizations

### Question 7:
An insurance company is building a binary classification model to predict insurance claims. The training data contains 1800 instances of the positive class (customers who did claim insurance) and 100 instances of the negative class (customers who did not claim insurance). The final model has 85% accuracy, but poor precision. How can you improve the model performance (Select three):
* Collect more training data for the negative class
* Collect more training data for the positive class
* Create more samples using algorithms such as SMOTE
* Over-sample from the negative class
* Over-sample from the positive class

### Question 8:
As part of a clinical study, you have processed millions of medical records with hundreds of features and reduced the feature dimensions to just two using a model based on Principal Component Analysis (PCA). The following graph illustrates the distribution from the PCA model output in the form of two distinct classes shown in red and blue dots.
* Support Vector Machine
* Linear Regression
* K-means
* Logistic Regression

### Question 9:
The ML solutions team at a leading ecommerce company wants to build a real time fraud detection system. As an ML Specialist, what is the recommended course of action to build such a system with the least number of components and ease of maintenance:
* Ingest the clickstream data into Kinesis Data Streams, which is then written into Kinesis Data Analytics for real time fraud detection and the processed stream data is finally directly written into S3.
* Ingest the clickstream data into Kinesis Data Streams, which is then written into Kinesis Data Analytics for real time fraud detection using the Random Cut Forest Algorithm. A Lambda function sends an email alert for every fraud detected by the algorithm. The processed stream data is finally sent to Kinesis Data Firehose for subsequent storage in S3.
* Ingest the clickstream data into a Spark Streaming application running on EMR cluster to detect fraud records. The application then writes the data into S3.
* Ingest the clickstream data into Kinesis Data Analytics for real time Fraud Detection and the data is finally sent to Kinesis Data Firehose for subsequent storage in S3.

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

### Question 10:
The data science team at a leading Questions and Answers website wants to improve the user experience and therefore would like to identify duplicate questions based on similarity of the text found in a given question. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* XGBoost
* BlazingText Word2Vec mode
* Factorization Machines
* Object2Vec

# Exam 2

### Question 1:
A media company needs to ingest and store a continuous stream of social media data. The source data is in JSON format. The company does not want to manage the underlying infrastructure and it wants the data to be immediately available for ad-hoc analysis. The solution must be cost efficient and scalable. As an ML specialist, what is your recommendation:
* Ingest the data using Kinesis Firehose that further transforms the data into Parquet format while writing to S3. Use an AWS Glue Crawler to read this data into an Athena table for ad-hoc analysis.
* Ingest the data using Kinesis Data Streams and use a Lambda function to write the stream into S3. Launch a Glue ETL Job every 15 minutes to convert the data from JSON format to Parquet format. Use an AWS Glue Crawler to read this data into an Athena table for ad-hoc analysis.
* Ingest the data into S3 using Kinesis Firehose. Launch a Glue ETL Job every 15 minutes to write S3 data into RDS. Perform ad-hoc query analysis once data is ingested into RDS.
* Ingest the data using a Spark Streaming application running on an EMR cluster. The output data is written in Parquet format on S3. Use an AWS Glue Crawler to read this data into an Athena table for ad-hoc analysis.

### Question 2:
The Machine Learning team at an ecommerce company is analysing the sales data. The data is stored in a highly optimized data compression format and the daily volume of data is around 1TB. The team would like to reduce this volume to one-tenth of its original size without significantly compromising on the quality of data, so that they can complete the classification model training in a much shorter timespan. As an ML Specialist, what solution would you recommend to the team:
* Use a more efficient compression algorithm
* Use dimensionality reduction to reduce the data volume and still preserve a significant variance between observations
* Use clustering to reduce the data volume and still preserve a significant variance between observations
* The team needs to use better hardware to run the classification model training so that the original data can be processed in a short timespan

### Question 3:
Executives at a leading smartphone brand are contemplating the launch of a radical new phone model with never-before-seen features. Given the lack of historical data for this phone model, which AWS SageMaker algorithm can help the executives in predicting the product sales over the next quarter for this innovative phone:
* DeepAR
* XGBoost
* Factorization Machines
* Linear Learner

### Question 4:
Identify the correct statement regarding SageMaker Inference Pipelines:
* Inference Pipelines can neither be used to process batch transforms nor to make real-time predictions
* Inference Pipelines can only be used to make real-time predictions but not to process batch transforms
* Inference Pipelines can only be used to process batch transforms but not to make real-time predictions
* Inference Pipelines can be used to make either real-time predictions or to process batch transforms

### Question 5:
A Silicon Valley startup has introduced a new email service that would completely eradicate spam from the inbox. The data scientists at the startup have prepared the following confusion matrix for the underlying model. What is the F1 score for the underlying model:
* 0.73
* 0.63
* 0.84
* 0.93

### Question 6:
Some supervised learning algorithms on SageMaker require the training data to be in CSV format. Which constraints should the CSV file meet (Select two):
* Target variable should be in the first column
* It should not have a header record
* It should have a header record
* Target variable is in the last column

### Question 7:
An entrepreneur wants to launch the next unicorn business with futuristic Business Intelligence features. The product would allow business managers to gather business insights using a voice based conversational interface rather than typing tedious SQL commands. Which AWS services would you use to build this product with the least amount of time and resources (Select three):
* Translate
* Comprehend
* Polly
* Connect
* Lex

### Question 8:
After training a SageMaker Linear Learner model over a huge training dataset, the data science team observed that it achieved high accuracy on the training data, but had low accuracy on the test data. As an ML specialist, what are the three techniques that you will recommend to help resolve this problem? (Select three):
* Remove regularization from the model
* Use less training data
* Use more training data
* Use more features in the model
* Use less features in the model
* Add regularization to the model

### Question 9:
A data science intern at an Analytics Company is working on creating a binary classification model. He has created a SageMaker notebook instance using its default IAM role and is trying to read the training data from a S3 bucket with the name “model-training-data”. However the data is not accessible in the Jupyter Notebook. How can he resolve this issue (Select two):
* Use a bucket with the word “sagemaker” in its name
* Restart the Jupyter notebook instance and that should resolve the data access issue
* Make the S3 bucket public
* Add a policy to the role that grants the SageMaker service principal S3FullAccess permission

### Question 10:
A sports enthusiast wants to build a mobile app that is able to recognize celebrity athletes. Which AWS service can help him set this up with minimum possible effort:
* Amazon Lex
* Amazon Rekognition
* Amazon Predict
* Amazon Polly

### Question 11:
For production systems based on SageMaker, which version tag should be used in the Registry Paths:
* :-1
* :0
* :latest
* :1

### Question 12:
Tf-idf is a statistical technique frequently used in Machine Learning areas such as text-summarization and classification. Tf-idf measures the relevance of a word in a document compared to the entire corpus of documents. You have a corpus (D) containing the following documents:
* Using tf-idf, the word “fox” is more relevant for document d2 than document d1
* Using tf-idf, the word “fox” is more relevant for document d1 than document d2
* Using tf-idf, the word “fox” is equally relevant for both document d1 and document d2
* Insufficient information has been provided to compute tf-idf

### Question 13:
A company has one year of raw data on demographics and sales for existing customers. The digital marketing executives at the company want to identify potential customers on social media. As the festive season is coming up, the solution needs to be built in the shortest possible time. What is the best course of action for this goal:
* Use K-means to identify groups of customers and then find similar customers on social media.
* Use Recommendation Systems to build the existing customer profiles and then predict the best matching customers from their social media profiles
* Use Linear Regression to predict the best matching customers from their social media profiles
* Use XGBoost to predict the best matching customers from their social media profiles

### Question 14:
Identify the SageMaker algorithm that can be used both as a built-in-algorithm as well as a framework such as Tensorflow:
* Linear Learner
* Object2Vec
* Factorization Machines
* XGBoost

### Question 15:
A Neural Network is tasked with classifying the correct breed from a given pool of ten breeds of dogs for a scientific experiment. Which activation function should be used in the output layer of this Neural Network:
* RELU
* Softmax
* Tanh
* Sigmoid

### Question 16:
You are analyzing the salary trends for Silicon Valley engineers over the last decade. The dataset has information on the age, professional experience in years, skill level from 1 to 10, gender, location (5 distinct locations) and salary. What is the best way to visualize the average annual salary trend at each location over the last decade:
* Bar Chart
* Pie Chart
* Line Chart
* Scatter Plot

### Question 17:
Identify the correct statements regarding the IAM features available to use with Amazon SageMaker (Select two):
* With IAM identity-based policies, you can specify allowed or denied actions and resources as well as the conditions under which actions are allowed or denied for Amazon SageMaker
* Amazon SageMaker supports resource-based policies
* Amazon SageMaker supports service linked roles
* Amazon SageMaker supports authorization based on resource tags

### Question 18:
A bioinformatics company wants to automate the secondary analysis of the raw DNA reads into a complete genomic sequence by comparing the multiple overlapping reads and the reference sequence, as well as potentially reduce data errors caused by incorrect alignment between the reference and the sample. Which AWS service can be used to configure and schedule this secondary analysis:
* AWS Glue
* Amazon CloudWatch
* Amazon SageMaker
* AWS Batch

### Question 19:
How many shards would a Kinesis Data Stream need if the average record size is 500KB and 2 records per second are being written into the Stream application. Additionally, there are 7 consumer applications using this Kinesis Data Stream Application.
* 7
* 3
* 1
* 4

### Question 20:
A medical diagnostics company specializes in cancer detection tests. The data scientists at the company need to focus on which metric for the underlying classification model in order to not miss any cases of cancer (The model’s predicted value of 1 implies that the patient is predicted to have cancer):
* F1-score
* Accuracy
* Precision
* Recall

### Question 21:
Which of the following is correct regarding the model types that Amazon SageMaker Neo supports:
* Neo supports regression models
* Neo supports image classification models.
* Neo supports recommendation system models
* Neo supports dimensionality reduction models

### Question 22:
Identify the three step process for training with the Amazon SageMaker k-nearest neighbors (k-NN) algorithm (Select three):
* One-Hot Encoding
* Sampling
* Index Building
* Data Engineering
* Dimension Reduction

### Question 23:
What are the ideal characteristics of a good dataset for Machine Learning problems (Select two):
* Should have skewed distribution so algorithm can learn the edge cases correctly
* Should have some bias so algorithm can learn the edge cases correctly
* Should have fair sampling with even distribution of outcomes
* Should be representative of the underlying business problem to be solved

### Question 24:
You are developing a multi-class classification model with Sagemaker XGBoost algorithm using the AWS SDK for Python (Boto 3). After calling the create_training_job() method to start the training job, you would like to get a status about the progress of the training job. Which method can be used to get the training job status:
* describe_training_status
* get_training_status
* describe_training_job
* get_training_job

### Question 25:
A SageMaker training job with 1TB of training data is taking too long to run. As an ML specialist, which is the most cost effective course of action that requires the least infrastructure management:
* Convert the training data to recordIO-protobuf file type
* Run the training job on an EMR cluster having Amazon SageMaker Spark Library along with the training container image.
* Add additional storage to the SageMaker Training Instance
* Since time is the limiting resource, upgrade the SageMaker Training Instance type to the highest possible type so that the job runs quickly

### Question 26:
A data preprocessing script uses the sklearn and numpy libraries in Python. Which type of Glue job is needed to support this:
* Zeppelin Shell
* Python Shell
* PySpark
* Jupyter Shell

### Question 27:
You are running a SageMaker training job. You notice that the job has failed but there are no logs on CloudWatch. Identify the possible scenarios behind this issue (Select two):
* S3 location for training data is incorrect
* The default IAM role needs to have the correct permissions in order to write logs into Cloudwatch
* Logs appear on Cloudwatch 15 minutes after the attempted job run
* The training job has the wrong training image

### Question 28:
Which SageMaker unsupervised learning algorithms can be used for Fraud Detection (Select two):
* IP Insights
* Object2Vec
* Random Cut Forest
* Factorization Machines

### Question 29:
The data science team at an Analytics company is working on a dataset with a large number of observations and features. They want to use the SageMaker Principal Component Analysis (PCA) Algorithm to reduce the dimensionality within the dataset. Which mode should be used for using PCA on this dataset:
* Use PCA in regular mode
* PCA is not the right selection for this use-case
* Use PCA in either regular or randomized mode
* Use PCA in randomized mode

### Question 30:
You are creating a classification model using one of the Amazon SageMaker built-in algorithms and you want to use GPUs for both training and inference. Identify the correct steps (Select two):
* Enable GPU support in the docker image for the SageMaker algorithm
* Select the correct instance type that supports GPUs
* Specify gpu=True as the parameter in the create_training_job boto3 API call on Jupyter Notebook
* Select a built-in algorithm that supports GPUs for both training and inference

### Question 31:
Identify the correct statements regarding the Amazon SageMaker logging and monitoring options on CloudWatch and CloudTrail (Select four):
* AWS CloudTrail provides a record of actions taken by a user, role, or an AWS service in Amazon SageMaker. CloudTrail keeps this record for a period of 90 days
* SageMaker monitoring metrics are available on CloudWatch at a 2-minute frequency
* CloudTrail monitors calls to InvokeEndpoint
* CloudWatch keeps the SageMaker monitoring statistics for 15 months. However, the Amazon CloudWatch console limits the search to metrics that were updated in the last 2 weeks.
* CloudTrail does not monitor calls to InvokeEndpoint
* SageMaker monitoring metrics are available on CloudWatch at a 1-minute frequency

### Question 32:
A Silicon Valley startup intends to provide real estate recommendations to millions of homebuyers. The data science team is grappling with thousands of features that could go into the model, so the team wants to consider only the most relevant derived features. As an ML Specialist, what solution would you recommend to get them started:
* Use K-means to identify the most relevant derived features
* Use Latent Dirichlet Allocation to identify the most relevant derived features
* Use Neural Topic Model to identify the most relevant derived features
* Use Principal Component Analysis to identify the most relevant derived features

### Question 33:
The data science team at an investment bank is analyzing the stock price data for blue chip stocks over the last year. Which visualization tools can be used to spot outliers (Select three):
* Line chart
* Histogram
* Heatmap
* Bar chart
* Scatter plot
* Box plot

### Question 34:
A financial services company has the goal of reducing fraud transactions by 10% over the next financial year. In order to achieve this goal, which of the following is the most relevant model evaluation metric that the data scientists at the company need to focus on (the model’s predicted value of 1 implies that the transaction is predicted to be fraud) :
* Recall
* Precision
* Precision-Recall Area-Under-Curve (PR AUC)
* F1-score

### Question 35:
In order to run unsupervised algorithms on SageMaker you need to configure content type parameter. How should you specify the number of label columns in the content type:
* application/csv;label_size=None
* application/csv;label_size=0
* text/csv;label_size=0
* text/csv;label_size=None

### Question 36:
Which SageMaker algorithm comes in both supervised and unsupervised learning modes:
* Blazing Text
* Random Cut Forest
* Latent Dirichlet Allocation
* XGBoost

### Question 37:
The AI research department at a University is collaborating with a consultancy firm. A research assistant at the department would like to allow developers from the consultancy firm to access some of the SageMaker resources created in the AWS account of the research department. What are the recommended ways this access can be granted (Select two):
* Create SageMaker resource based policies to allow this access
* Create a role to delegate access to your resources with the third-party AWS account
* Create a new AWS user account and share the username and password via email
* Provide access to externally authenticated users through identity federation

### Question 38:
An online retail company specializing in fashion wear wants to automate the various categories of fashion wear in their catalog. They have about 50,000 images of their product catalog but none of them have the right labels for the associated categories. As an ML Specialist, what solution will you recommend to build the training data with the correct labels:
* Use AWS Rekognition to create the category labels for the training images
* Use SageMaker Image Classification to create the category labels for the training images
* Use SageMaker Semantic Segmentation to create the category labels for the training images
* Use SageMaker Ground Truth to create the category labels for the training images

### Question 39:
For the upcoming festive season, an ecommerce company is anticipating a major shift in the expected workload for its product recommendation engine hosted on SageMaker. Which solution would you recommend to address this issue:
* Use automatic scaling for the production variants to manage the workload
* Use inference pipelines to manage the workload
* SageMaker hosting has a built-in mechanism to address this issue. Nothing else needs to be done.
* Use elastic inference to manage the workload

### Question 40:
You are analyzing the income data provided in a case study as part of a data science competition. You observe that the data has several outliers. Which techniques you can use to address outliers in the data (Select two):
* Logarithm Transformation
* One-hot encoding
* Normalization
* Standardization

### Question 41:
Identify the correct statement vis-a-vis the difference between a data lake and data warehouse:
* A data warehouse can only store structured data whereas a data lake can store structured, semi-structured and unstructured data
* A data lake can only store structured data whereas a data warehouse can store structured, semi-structured and unstructured data
* Both data lake and data warehouse can store structured, semi-structured and unstructured data
* Both data lake and data warehouse can only store structured data

### Question 42:
The data science team at an email marketing company has created a data lake with raw and refined zones. The raw zone has the data as it arrives from the source, however, the team wants to de-duplicate the data before it is written into the refined zone. What is the best way to accomplish this with the least amount of development time and infrastructure maintenance effort:
* Create an Apache Spark based EMR job and run it once a day to de-duplicate the records from raw zone into refined zone.
* Ingest the raw zone data in Kinesis Data Firehose and process the data using a Lambda function before it is finally dumped into the refined zone.
* Invoke an AWS Glue ML Transforms job when new data arrives into raw zone so that de-duplicated records can be written into the refined zone
* Create a Lambda function with the code to handle all possible data duplication use cases. Trigger a Lambda function when new files arrive in the S3 raw zone.

### Question 43:
Identify the three step process while deploying a model using SageMaker hosted services (Select three)
* Create the endpoint configuration for HTTPS endpoint
* Create the model
* Create the HTTPS endpoint
* Tune model hyperparameters
* Validate the model

### Question 44:
You would like to identify the “global hotspots” for UFO sightings over the last 50 years. The data is available from a globally reputed agency based out of Area 51. Which visualization tool is best suited to bring out these locations on a geographic map:
* Hashmap
* Heatmap
* Mindmap
* Treemap

### Question 45:
After training a SageMaker XGBoost based model over a huge training dataset, the data science team observed that it has low accuracy on the training data as well as low accuracy on the test data. As an ML specialist, what are the two techniques that you will recommend to help resolve this problem? (Select two):
* Remove regularization from the model
* Use more training data
* Use less training data
* Add regularization to the model
* Use less features in the model
* Use more features in the model

### Question 46:
A research agency is developing a robotic submarine to map the marine life forms in the pacific ocean. The robot should be able to classify the images of marine life forms in an autonomous way with low latency. Which Amazon SageMaker architecture would you recommend for this use-case:
* Use Kinesis Video Streams to classify the images of the marine life forms
* Use Kinesis Data Streams to process the video stream and invoke a lambda to infer via a classification model to classify the images of the marine life forms
* Use AWS Rekognition to classify the images of the marine life forms
* Use SageMaker Neo to compile and package the classification model on the underlying runtime infrastructure on the robotic device.

### Question 47:
The data science team at an Email Service Provider has determined that the long term cost of marking a bona fide email as spam is much greater than the cost of marking a spam email as bona fide. To address this issue, the team worked on a classification model to predict if an email is spam and boiled it down to two model variants. Model A had 95% accuracy with 40 False Negatives (FN) and 100 False Positives (FP) whereas model B also had 95% accuracy with 100 FN and 40 FP. Which of the two models is more cost effective for the company :
* None of the Model A and Model B are cost effective. Company needs to try something different.
* Model A
* Both Model A and Model B are equally cost effective, as accuracy is same
* Model B

### Question 48:
The management of a shopping mall wants to predict the number of footfalls next week. They have data for the average number of footfalls over the last 52 weeks. Which probability distribution should they be using for this scenario planning exercise ?
* Poisson distribution
* Binomial distribution
* Normal distribution
* Bernoulli distribution

### Question 49:
A retail organization wants to forecast the sales of its flagship products for the upcoming festive season. They have the last 5 years of sales data for these products. As an ML specialist, which algorithm would you use to implement the forecasting solution:
* Random Cut Forest
* Latent Dirichlet Allocation (LDA)
* Linear Learner
* Semantic Segmentation

### Question 50:
Researchers at a university claim a breakthrough in early cancer detection. The lab results for a series of trials yield the following confusion matrix. What is the recall of the underlying model:
* 80%
* 20%
* 89%
* 50%

### Question 51:
The marketing analytics team at a leading bank has created a multi-class classification model to segment the bank’s customers into three tiers - Platinum, Gold and Silver. The confusion matrix for the underlying model was reported as follows:
* 0.30
* 0.57
* 0.46
* 0.20

### Question 52:
How many containers can a SageMaker Inference Pipeline support (Select two):
* 2
* 1
* 7
* 3

### Question 53:
The data engineering team at a social media company has handed over the cleaned and prepared dataset to the Machine Learning team. The ML team wants to use this dataset for building a regression model based on the SageMaker Linear Learner algorithm. Which is the first step that the ML team needs to do:
* Standardize the dataset
* Create training set, validation set and test set
* Shuffle the dataset
* Normalize the dataset

### Question 54:
AWS Glue jobs can be used to create serverless ETL jobs. Identify the ETL source input type that AWS Glue does not support for ETL jobs:
* PostgreSQL
* DocumentDB
* Timestream
* Oracle

### Question 55:
An FMCG company has 33 shampoo and 37 conditioner variants in its product portfolio. Senior executives are planning to launch a hybrid product with features from its shampoo and conditioner portfolio. Given the lack of reference historical data for this hybrid product, which AWS SageMaker algorithm can help the executives in predicting the product sales over the next financial year:
* Factorization Machines
* DeepAR
* Linear Learner
* XGBoost

### Question 56:
To get inference for an entire dataset, you are developing a batch transform job using Amazon SageMaker High-level Python Library. Which method would you call so that the inferences are available for the entire dataset:
* predict
* transform
* deploy
* fit

### Question 57:
Learning curve is a graph that compares the performance of a model on training andx` validation datasets over a varying number of training instances. Following figure illustrates the learning curve for two separate models:
* Add more features to the model
* Decrease regularization parameters
* Get more training data
* Increase regularization parameters
* Remove features from the model

### Question 58:
You are building a forecasting model using the SageMaker DeepAR algorithm. The following graph captures the Actual vs Forecast comparison from the model output for the revenue data for the last few years:
* The forecast captures the seasonality well but misses the trend
* The forecast captures both the trend and seasonality well
* The forecast captures neither the trend nor the seasonality
* The forecast captures the trend well but misses the seasonality

### Question 59:
While using the K-means SageMaker algorithm, which strategies are available to determine how the initial cluster centers are selected (Select two):
* Random approach
* Within Cluster Sum of Squares
* k-means++
* Euclidean distance

### Question 60:
A data science team is trying to port a legacy binary classification model to Amazon SageMaker. In the legacy workflow, the data engineering component was handled using Apache Spark and scikit-learn based preprocessors. Which feature of Amazon SageMaker can be utilized for seamless integration of the legacy functionality into the new SageMaker model:
* Inference Pipeline
* Elastic Inference
* Batch Transform
* Automatic Scaling

### Question 61:
A bio-technology company has invented a new drug testing procedure that can identify substance abuse from blood samples within a minute. The law stipulates that anyone found indulging in substance abuse faces a steep fine along with a prison term. Identify the metric that the data scientists at the company need to focus on, so that they can analyze the results of the trials for the underlying model (The model’s predicted value of 1 implies that the individual was predicted to have consumed drugs):
* F1-score
* Accuracy
* Specificity
* Recall

### Question 62:
The data engineering team at an ecommerce company is migrating its data architecture from a data lake to a data warehouse. The current data lake is housed in S3. Which is the fastest way to load this data into Amazon Redshift:
* Use the INSERT command to load data from files in S3.
* Use the LOAD command to load data from files in S3.
* Use the UNLOAD command to load data from files in S3.
* Use the COPY command to load data from files in S3.

### Question 63:
The ML team at a research lab have trained a Deep Neural Network using a huge training dataset. After a series of training runs, the team observes that the training error is much lower than the test error. What steps would you recommend to address this issue (Select three) :
* Remove parameter regularization
* Use dropout
* Add parameter regularization
* Use early stopping while training
* Do not use early stopping while training

### Question 64:
Identify the correct definitions for the Latent Dirichlet Allocation algorithm:
* Observations are referred to as documents. The feature set is referred to as vocabulary. A feature is referred to as a word. And the resulting categories are referred to as topics.
* Observations are referred to as topics. The feature set is referred to as word. A feature is referred to as a vocabulary. And the resulting categories are referred to as documents.
* Observations are referred to as words. The feature set is referred to as vocabulary. A feature is referred to as a document. And the resulting categories are referred to as topics.
* Observations are referred to as vocabulary. The feature set is referred to as documents. A feature is referred to as a topic. And the resulting categories are referred to as words.

### Question 65:
An analytics company wants to create a text summarization model based on the SageMaker seq2seq algorithm. However the training data is in the form of 1TB of flat files whereas seq2seq only expects RecordIO-Protobuf format. As an ML Specialist, what solution would you recommend:
* Use Kinesis Data Firehose to transform the data into RecordIO-Protobuf format
* Spin-up an Apache Spark EMR cluster to transform the data from flat files into RecordIO-Protobuf format and save it on S3. This data can be used by seq2seq based model for training
* Use AWS Step function with Lambda to write the data in RecordIO-Protobuf format on S3. This data can be used by seq2seq based model for training
* Use AWS Glue to create an ETL job to write the data in RecordIO-Protobuf format on S3. This data can be used by seq2seq based model for training



# Exam 3

### Question 1:
Which of the following is correct regarding an inference pipeline on Amazon SageMaker:
* Within an inference pipeline model, Amazon SageMaker handles invocations as a sequence of RPC requests.
* Within an inference pipeline model, Amazon SageMaker handles invocations as a sequence of HTTP requests.
* Within an inference pipeline model, Amazon SageMaker handles invocations as a sequence of HTTPS requests.
* Within an inference pipeline model, Amazon SageMaker handles invocations as a sequence of MQTT requests.

### Question 2:
The research team at a University wants to do sentiment analysis of the most famous quotes from the classical english literature over the last 500 years. Some of the sample quotes from the corpus are like so : “All that glitters is not gold”, “Brevity is the soul of wit”, “The lady doth protest too much, methinks.”, “Love all, trust a few, do wrong to none.” As an ML Specialist, what data pre-processing steps would you recommend before the team starts building the model (Select three):
* Create n-gram vector for each word
* Lowercase each word
* Remove stop words
* Create one-hot encoding for each word
* Tokenize each word
* Remove archaic words such as doth and methinks

### Question 3:
You are working on a computer vision application (using Convolutional Neural Networks) to recognize an endangered species of tigers. 70% of the incorrectly classified images from the CNN were in a 90-degrees counter-clockwise rotated state. What corrective action you will take to address this issue:
* Add more hidden layers to the CNN
* Perform rigorous hyperparameter tuning to achieve better classification accuracy
* Procure more training images that are in 90-degrees counter-clockwise rotated state. Retrain the CNN with this new dataset.
* Use Recurrent Neural Network (RNN) for correct classification of all image orientations.

### Question 4:
Identify the criteria on which early stopping works in Amazon SageMaker:
* If the value of the objective metric for the current training job is worse (higher when minimizing or lower when maximizing the objective metric) than the mean value of running averages of the objective metric for previous training jobs up to the same epoch, Amazon SageMaker stops the current training job.
* If the value of the objective metric for the current training job is better (higher when minimizing or lower when maximizing the objective metric) than the mean value of running averages of the objective metric for previous training jobs up to the same epoch, Amazon SageMaker stops the current training job.
* If the value of the objective metric for the current training job is better (higher when minimizing or lower when maximizing the objective metric) than the median value of running averages of the objective metric for previous training jobs up to the same epoch, Amazon SageMaker stops the current training job.
* If the value of the objective metric for the current training job is worse (higher when minimizing or lower when maximizing the objective metric) than the median value of running averages of the objective metric for previous training jobs up to the same epoch, Amazon SageMaker stops the current training job.

### Question 5:
Identify the mandatory hyperparameter for both the Word2Vec (unsupervised) and Text Classification (supervised) modes of the SageMaker BlazingText algorithm:
* epochs
* buckets
* mode
* learning_rate

### Question 6:
An ML specialist is examining the root cause for underperformance of a regression model and has a hunch that it is consistently overestimating the outcome. Which metrics should he track on a chart to help identify any pattern of model overestimation:
* Mean Absolute Error
* RMSE
* Residuals
* AUC

### Question 7:
Identify the three built-in SageMaker algorithms that support incremental training (Select three):
* Image Classification
* Linear Learner
* Semantic Segmentation
* XGBoost
* Object Detection

### Question 8:
Considering the following ROC curve generated for the Amazon SageMaker XGBoost algorithm for a binary classification use-case
* The model represented by the black ROC curve is best at distinguishing the two classes. The model represented by the blue ROC curve is worst at distinguishing the two classes.
* The model represented by the blue ROC curve is best at distinguishing the two classes. The model represented by the black ROC curve is worst at distinguishing the two classes.
* The model represented by the black ROC curve is best at distinguishing the two classes. The model represented by the red ROC curve is worst at distinguishing the two classes.
* The model represented by the red ROC curve is best at distinguishing the two classes. The model represented by the blue ROC curve is worst at distinguishing the two classes.

### Question 9:
The data engineering team at a social media company ingests the clickstream data into the Kinesis Data Stream using the PutRecord API in the source system. Now, the team wants to ingest this data into Kinesis Data Firehose instead and they want to use the PutRecord API for Firehose. Identify the differences between the PutRecord API call for Kinesis Data Stream v/s Kinesis Data Firehose:
* Both Kinesis Data Firehose PutRecord API and Kinesis Data Streams PutRecord API use the name of the delivery stream and the data record
* Kinesis Data Firehose PutRecord API uses name of the stream, a partition key and the data blob whereas Kinesis Data Streams PutRecord API uses the name of the delivery stream and the data record
* Both Kinesis Data Firehose PutRecord API and Kinesis Data Streams PutRecord API use the name of the stream, a partition key and the data blob
* Kinesis Data Streams PutRecord API uses name of the stream, a partition key and the data blob whereas Kinesis Data Firehose PutRecord API uses the name of the delivery stream and the data record

### Question 10:
The ML team at an ecommerce company has trained a SageMaker XGBoost model on a large dataset. The evaluation metric looks good for the training job. However, post production deployment, the team observes that the inference results are not correct. As an ML Specialist, what would you recommend to resolve this issue:
* Replace XGBoost with Linear Learner algorithm
* Use Elastic Inference to improve the inference results
* Make sure that the training data distribution is similar to the expected distribution for the production inference data.
* These variations should be acceptable as part of the model performance

### Question 11:
A marketing analyst wants to group current and prospective customers into 10 groups based on their attributes. He wants to send mailings to prospective customers in the group which has the highest percentage of current customers. As an ML Specialist, which Sagemaker algorithm would you recommend as a solution:
* K-means
* Latent Dirichlet Allocation
* PCA
* KNN

### Question 12:
An analytics company is doing the sentiment analysis of tweets about a leading sports event. The company has prepared the following confusion matrix. What is the precision of the underlying model:
* 50%
* 80%
* 20%
* 89%

### Question 13:
The data science team at an ecommerce company is working on a training dataset for a forecasting model. The dataset represents the sales data for the last 5 years and has the following features : item description, item price, order date, quantity ordered, shipping address, order amount. The team would like to uncover any cyclical sales patterns such as hourly, daily, weekly, monthly, yearly from this data. As an ML Specialist, what solution would you recommend:
* No need for data preprocessing as the underlying algorithm can detect the cyclical patterns on its own
* Preprocess the order date to create new features such as hour of the day, day of the week, week of the month, week of the year, date of the month, month of the year and use these features in one-hot encoded format for training the model
* Preprocess the order date to create new features such as hour of the day, day of the week, week of the month, week of the year, date of the month, month of the year and use these features in label encoded format for training the model
* Preprocess the order date to create new features such as hour of the day, day of the week, week of the month, week of the year, date of the month, month of the year and represent these features as (x,y) coordinates on a circle using sin and cos transformations. This transformed data should then be used to train the model.

### Question 14:
You have disabled direct internet access to your Amazon SageMaker notebook instance while connecting to your VPC in order to prevent unauthorized access to your data. As there is no data access, the notebook instance is not able to train or host models. Which of the following solutions would address this issue when combined together? (Select two):
* Setup NAT gateway for your VPC along with Security Groups for your VPC that allow inbound connections
* Setup NAT gateway for your VPC along with Security Groups for your VPC that allow outbound connections
* Setup S3 gateway for your VPC
* Create a VPC interface endpoint to use PrivateLink for your notebook instance

### Question 15:
The compliance department at a major Financial Services Firm wants to monitor the SageMaker services used by the Data Science team for their ML jobs. Which services can be used to achieve this objective (Select two) :
* Amazon Cloudwatch
* AWS Cloudtrail
* AWS Config
* Amazon Inspector

### Question 16:
You would like to tune the hyperparameters for the Sagemaker XGBoost algorithm. Identify the correct options for the model validation techniques (Select two):
* Validation using a holdout set
* K-fold validation
* Validation using SageMaker Ground Truth
* Validation using training set

### Question 17:
A leading ecommerce company is looking to improve the user experience by recommending the related product categories for its catalog of products. As an ML Specialist, which SageMaker algorithms would you use to develop a solution for this use-case (Select two):
* Factorization Machines
* XGBoost
* Latent Dirichlet Allocation (LDA)
* K-means

### Question 18:
You are creating a computer vision application to recognize truck brands. Your application uses Convolutional Neural Networks (CNN) but you do not have enough data to train the model. However, there are pre-trained third-party image recognition models available for similar tasks. What steps will you take to build your solution in the shortest possible duration:
* Use transfer learning by retraining the pre-trained third-party image recognition model with your own data.
* Use transfer learning in your CNN by using the pre-trained third-party image recognition model as the convolutional base. Then remove the original classifier from the pre-trained model and add the new classifier for recognizing truck brands.
* Use Kinesis Video Streams to identify the truck brand by using image manipulation algorithms and then do a pixel by pixel comparison
* Use transfer learning with Kinesis Video Streams

### Question 19:
The marketing analytics team at a financial services company is working on creating a customer loyalty program targeted at specific groups of customers. Which data analysis technique should be used for this goal:
* Bivariate visualizations
* Dimensionality Reduction
* Clustering
* Multivariate visualizations

### Question 20:
An electronics goods company wants to do sentiment analysis of the customer feedback for its latest product recently launched in France. However, the customer feedback is only available in the form of recorded audio snippets in the French language. As an ML specialist, which AWS AI services can you use to build the simplest solution with the least effort:
* Transcribe -> Translate -> Comprehend
* Translate -> Transcribe -> Comprehend
* Transcribe -> Comprehend
* Transcribe -> Lex -> Comprehend

### Question 21:
Which of the following statements is true for the Sagemaker Linear Learner algorithm:
* When you use automatic model tuning, the linear learner internal tuning mechanism is turned off automatically. This sets the number of parallel models, num_models, to 0
* When you use automatic model tuning, the linear learner internal tuning mechanism is turned off automatically. This sets the number of parallel models, num_models, to 1
* When you use automatic model tuning, the linear learner internal tuning mechanism is turned on automatically. This sets the number of parallel models, num_models, to 1
* When you use automatic model tuning, the linear learner internal tuning mechanism is turned on automatically. This sets the number of parallel models, num_models, to 0

### Question 22:
The data science team at an analytics company is working on a linear regression model and it observes that the training error as well as the test error are high, implying that the model has a bias. Which of the following L1 and L2 regularization optimizations may be done to resolve this issue (Select two):
* Decrease L1 regularization
* Increase L1 regularization
* L1 and L2 regularization are not required, just get more training data
* Use L2 regularization and drop L1 regularization

### Question 23:
A Financial Services company has asked you to finetune its SageMaker model training process. You observe that the company runs the training jobs multiple times in a day with a little tweaking of the training data for each run. Which steps would you recommend to improve the training performance so that the training jobs can complete faster (Select two) :
* Upgrade the training instance to the highest possible type
* Spin up an EMR cluster to process the training job
* Use pipe mode to stream data from S3
* Change the data format to protobuf recordIO format

### Question 24:
The traffic monitoring authorities at a city want to monitor the traffic at busy intersections and take corrective action at the earliest. An ML solutions company has developed a Proof-of-Concept for processing this video data and now it wants to productionalize it to cover all city intersections. What is the recommended solution stack with the LEAST amount of development effort and ongoing maintenance:
* Process the incoming video data using Kinesis Data Streams, trigger a Lambda for each stream and then do frame analysis to detect anomalous traffic situations and alert the authorities
* Process the incoming video data using Kinesis Data Analytics to detect anomalies in real time
* Analyse the incoming video streams using Kinesis Video Streams in real time and then send an alert using a downstream EC2 instance
* Process the incoming video data using Spark Streaming on EMR cluster to detect anomalous traffic situations and alert the authorities

### Question 25:
You are working on a fraud detection model based on SageMaker IP Insights algorithm with a training data set of 1TB in CSV format. Your Sagemaker Notebook instance has only 5GB of space. How would you go about building your model, given these constraints:
* Shuffle the training data and create a 5GB slice of this shuffled data. Build your model on the Jupyter Notebook using this slice of training data. Once the evaluation metric looks good, create a training job on SageMaker infrastructure with the appropriate instance types and instance counts to handle the entire training data.
* Create an AWS Glue job to transform the training data into recordIO-protobuf format. Read the entire transformed data in recordIO-protobuf format from S3 in your Jupyter Notebook instance while training your model.
* Create an AWS Glue job to compress the training data into parquet format using an appropriate compression codec. This should allow you to use the entire compressed training data on your notebook instance.
* Spin-up an EMR Cluster running Apache Spark to transform the CSV data into recordIO-protobuf format. Read the entire transformed data in recordIO-protobuf format from S3 in your Jupyter Notebook instance while training your model.

### Question 26:
As a security policy, the data science team at an ecommerce company does not want Amazon SageMaker to provide external network access to the training or inference containers, so network isolation is enabled for all containers. Identify the Amazon SageMaker containers that do not support network isolation, so the data science team does not use them for modeling (Select three):
* MXNet
* Pytorch
* TensorFlow
* Amazon SageMaker Reinforcement Learning
* Scikit-learn

### Question 27:
You have built a deep learning model and now want to deploy it using the SageMaker Hosting Services. For inference, you want a cost-effective option that guarantees low latency but still comes at a fraction of the cost of using a GPU instance for your endpoint. As an ML Specialist, what would you recommend to use:
* Automatic Scaling
* Elastic Inference
* SageMaker Neo
* Inference Pipeline

### Question 28:
The data science team at an ecommerce company has been tasked to improve the underlying recommendations engine. The team has tried to use both the random search and bayesian search approaches to hyperparameter tuning, but the results have been inconsistent. As an ML Specialist, what would be your suggestion to the team:
* Increase the number of hyperparameters that can be searched to 20
* Increase the number of concurrent hyperparameter tuning jobs to 100
* Increase the maximum run time for a hyperparameter tuning job to 30 days
* Hyperparameter tuning might not improve your model and look at other options such as data engineering or alternate algorithm to improve the model

### Question 29:
A Sports Analytics Company wants to analyse the game-plays for the coming NBA season. They would like to track the movement of each athlete for post-game analysis. Which AWS service can they use to build a solution in the least possible time:
* AWS Rekognition
* Kinesis Video Streams
* SageMaker Image Classification
* Kinesis Data Stream with Lambda based video frame processing

### Question 30:
You are doing topic modeling using the SageMaker Latent Dirichlet Allocation (LDA) algorithm. Which of the following are correct:
* LDA is a "bag-of-words" model, which means that the order of words does not matter
* LDA is a "bag-of-words" model, which means that the order of words does matter
* LDA is a not a "bag-of-words" model, which means that the order of words does matter
* LDA is a not a "bag-of-words" model, which means that the order of words does not matter

### Question 31:
You are pre-processing a training dataset to be used on the Amazon SageMaker Linear Learner algorithm. The dataset has hundreds of features and you need to decide which features to drop. Identify the guidelines that you would follow (Select three):
* Drop a feature if it has low variance
* Drop a feature if it has a few missing values
* Drop a feature if it has a lot of missing values
* Drop a feature if it has a low correlation to the target label
* Drop a feature if it has a high correlation to the target label
* Drop a feature if it has high variance

### Question 32:
You are training a batch transformation job in Amazon SageMaker. You have protected data at rest by using AWS KMS key on S3. Amazon SageMaker ensures that machine learning (ML) model artifacts and other system artifacts are encrypted in transit and at rest. What measures you would take to make sure that the data is protected in-transit even for inter-node training communications:
* Use SSH for inter-node traffic encryption
* Use AWS-SSE for inter-node traffic encryption
* Enable inter-container traffic encryption from the console
* There are no inter-node communications for batch processing, so inter-node traffic encryption is not required

### Question 33:
After training a SageMaker model over a huge training dataset, the data science team observed that it has low accuracy on the training data as well as low accuracy on the test data. What can you say about the model:
* Model is neither underfitting nor overfitting
* Model is underfitting
* Model is overfitting
* The model needs more training data

### Question 34:
An online real estate database company provides information on the housing prices for all states in the US by capturing information such as house size, age, location etc. The company is capturing data for a city where the typical housing prices are around $200K except for some houses that are more than 100 years old with an asking price of about $1 million. These heritage houses will never be listed on the platform. What data processing step would you recommend to address this use-case?
* One-hot encode the data for all houses in this city and then train the model
* Standardize the data for all houses in this city and then train the model
* Drop the heritage houses from the training data and then train the model
* Normalize the data for all houses in this city and then train the model

### Question 35:
You are building a feature for a web application such that when a user attempts to log in from an anomalous IP address, a web login server would trigger a multi-factor authentication system. Which SageMaker algorithm would you use for this feature:
* Random Cut Forest
* Factorization Machines
* XGBoost
* IP Insights

### Question 36:
You want to create an AWS Glue crawler to read the transaction data dumped into an S3 based data lake in the s3://mybucket/myfolder/ location. The transaction data is in CSV format however there are some additional metadata files with .metadata extension in the same location. The metadata needs to be ignored while reading the transaction data via Athena. How would you implement this solution:
* Use exclude pattern **.metadata in the crawler definition to ignore the metadata
* Use exclude pattern .**metadata in the crawler definition to ignore the metadata
* It is not possible to ignore the metadata in crawler. Create a daily ETL job to transfer only the transaction data specific CSV files into a new location and then read this cleansed transaction data into Athena.
* Use exclude pattern .metadata/** in the crawler definition to ignore the metadata

### Question 37:
Researchers at NASA are creating a model on Amazon SageMaker to analyze images for detecting strong gravitational lensing, a phenomenon in which an accumulation of matter in space is dense enough that it bends light waves as they travel around it. The training data contains 200K images of the negative class (images with no gravitational lensing) and only 2000 images of the positive class (images with gravitational lensing). The final model has 85% accuracy, but poor recall. How can you improve the model performance (Select two):
* Collect more training data for the negative class
* Collect more training data for the positive class
* Over-sample from the negative class
* Over-sample from the positive class

### Question 38:
Which is the best evaluation metric for a binary classification model:
* F1-Score
* Accuracy
* Precision
* AUC/ROC

### Question 39:
A leading technology company offers a fast-track leadership program to the best performing executives at the company. At any point in time, more than a thousand executives are part of this leadership program. Which is the best visualization type to analyze the salary distribution for these executives:
* Histogram
* Pie Chart
* Bubble Chart
* Bar Chart

### Question 40:
Which data set should you use for hyperparameter tuning:
* Training Set
* Validation Set
* Any of the Training Set, Validation Set or Test Set can be used.
* Test Set

### Question 41:
The data science team at an analytics company is working on a credit score model using SageMaker Linear Learner algorithm. The training data consists of these fields : name, age, annual salary, gender, employment status and credit score. The model needs to predict the credit score label. Which data preparation steps need to be done before working on the model:
* Drop the age and one-hot-encode name
* Drop the name and one-hot-encode gender and employment status
* Drop the name and one-hot-encode annual salary and credit score
* Drop the age and one-hot-encode name and credit score

### Question 42:
A plumbing company wants to better predict the sales of its flagship copper tubing for the next year. The sales data has copper tubing sizes captured as XS, S, M, L, XL and the retail price of the copper tubing varies with the size. What data preparation steps need to be done for the copper tubing size before it goes into the regression model for prediction:
* Interval Binning
* One-hot Encoding
* Quantile Binning
* Categorical Encoding

### Question 43:
A financial services company wants to migrate its data architecture from a data warehouse to a data lake. It wants to use a solution that takes the least amount of time and needs no infrastructure management. What options would you recommend to transfer the data from AWS Redshift to S3 (Select two):
* Apache Spark ETL script running on EMR cluster
* AWS Glue ETL job
* Lambda functions orchestrated by AWS Step Function
* AWS Data Pipeline

### Question 44:
An analyst is trying to create a box plot for the following data points :
* 10.2
* 15.9
* 16.4
* 14.4
* 14.1
* 15.1

### Question 45:
The data engineering team at an ecommerce company wants to ingest the clickstream data from the source system in a reliable way. The solution should provide built-in performance benefits and ease of use on the client side. Which solution would you implement on the source system:
* Kinesis Producer Library
* Spark Streaming
* Kinesis API
* Kinesis Client Library

### Question 46:
The Training Image and Inference Image Registry Paths used for SageMaker algorithms are of which type:
* City based
* Country based
* Region based
* Global

### Question 47:
You are developing a computer vision system for a factory assembly line. The system can trigger a robotic arm to correct the orientation of the product components whenever it detects a misalignment. Which SageMaker algorithm should be used in the computer vision system?
* Image Classification
* Reinforcement Learning (RL)
* Object Detection
* Semantic Segmentation

### Question 48:
You have launched a new Jupyter Notebook instance and you want to make sure that you don’t lose any files and data when the notebook instance restarts. Where should you save your files and data so that they are not overwritten on restart:
* /home/ec2-user/data
* /home/ec2-user/SageMaker
* /home/ec2-user/model
* /home/ec2-user/code

### Question 49:
You are building a Deep Learning based context-sensitive spelling correction functionality for a consumer facing application. For example, consider the following misspelled food description: “low tat milk”. A traditional spell checker might correct it to “low tar milk”, which is an inappropriate suggestion for the domain of food text, therefore it should be corrected to “low fat milk”. What technique would you use to build your context aware model:
* Word2Vec
* N-grams
* Seq2seq
* Levenstein distance

### Question 50:
A car insurance company wants to automate the claims process. The company wants the customers to upload the video footage of the damaged car. This video footage is then pre-assessed by an Amazon SageMaker model as part of the damage evaluation process. The company has no prior training data to get started on this endeavor. As an ML Specialist, what would you recommend to the company:
* Use AWS Rekognition to create the labels for the training videos. The labeled videos can be used to train the downstream Amazon SageMaker model for the damage evaluation process.
* Use Kinesis Video Streams to create the labels for the training videos. The labeled videos can be used to train the downstream Amazon SageMaker model for the damage evaluation process.
* Use Amazon SageMaker Ground Truth to create the labels for the training videos. The labeled videos can be used to train the downstream Amazon SageMaker model for the damage evaluation process.
* Use an unsupervised learning algorithm to label the videos which can be used in the downstream Amazon SageMaker model for the damage evaluation process

### Question 51:
An upcoming music streaming service wants to build a Minimum Viable Product and would like to have the underlying music recommendation engine developed at the earliest with the least development effort. As an ML Specialist, which AWS service would you suggest for the music recommendation engine:
* Amazon Personalize
* Amazon SageMaker Factorization Machines
* Amazon SageMaker Neural Topic Model
* Amazon SageMaker XGBoost

### Question 52:
A company wants to enhance the existing security procedure at its data center so that only the employees with the required privilege are able to access certain sensitive areas of the facility. The company wants to do a facial match so that only bona fide employees can access these sensitive areas. Which service would you recommend to build this solution with the least possible effort:
* SageMaker Image Classification
* SageMaker Object Detection
* SageMaker Semantic Segmentation
* AWS Rekognition

### Question 53:
An Analytics Consulting Firm wants you to review a Classification Model trained on historical data and deployed about 6 months ago. At the time of deployment the model performance was upto the mark. Post deployment, the model has not been retrained on the incremental data coming in every day. Now the model performance has gone down significantly. As an ML Specialist, what is your recommended course of action:
* Completely retrain the model using the historical data along with the data for the last 6 months.
* Completely retrain the model again using only the historical data
* Change the algorithm behind the model for better performance.
* Completely retrain the model using only the data for the last 6 months

### Question 54:
A marketing manager at an email marketing company is trying to figure out the right content and subject line for emails to be sent to the customers. The manager has access to all the historical responses to mailings from each customer. As an ML Specialist, which SageMaker algorithm would you recommend as a solution:
* Linear Learner
* Blazing Text
* XGBoost
* Factorization Machines

### Question 55:
Amazon Sagemaker models are stored in which format:
* model.tar.gzip
* model.gzip
* model.tar.gz
* model.zip

### Question 56:
A retail organization ingests 100GB of data into S3 from its global storefronts on a daily basis. This data needs to be cleaned, prepared and analyzed daily so that sales reports can be sent out to the business stakeholders. Which option takes the least effort to make this data available for SQL queries:
* Setup a daily Glue job to write the incremental S3 data into RDS and have it available for SQL queries
* Setup a daily Glue job to write the incremental S3 data into Redshift and have it available for SQL queries
* Setup Glue crawlers to initially read the data into Athena tables. Since the data schema does not change, the daily data is readily available for SQL queries in Athena as soon as it arrives
* Setup a daily Glue job to write the incremental S3 data into DynamoDB and have it available for SQL queries

### Question 57:
The data science team at a SaaS CRM company wants to improve its customer support workflow. The team wants to identify duplicate support tickets or route tickets to the correct support queue based on similarity of the text found in a ticket. As an ML Specialist, which SageMaker algorithm would you recommend to help solve this problem:
* Factorization Machines
* Object2Vec
* BlazingText Word2Vec mode
* XGBoost

### Question 58:
An Analytics Consulting Firm would like to capture and analyse the real time metrics for a cab hailing service. The Firm would like to identify “demand hotspots” in real time so that additional cabs can be dispatched to meet the sudden spurt in demand. What is the least effort way of building a real time analytics solution for this use case :
* Ingest the source data directly into Kinesis Data Analytics so that real time analytics can be done without any processing delay. Once processing is done, the streams are dumped into S3 using Kinesis Data Firehose.
* Ingest the data into Kinesis Data Streams that writes the data into a Spark Streaming application running on an EMR cluster. Once the processing is done, the output is written on S3
* Ingest the data into Kinesis Data Firehose and write into S3, which triggers a Lambda that analyses the event data. The Lambda finally writes the output to S3.
* Ingest the data into Kinesis Data Streams and immediately write the stream into Kinesis Data Analytics for SQL based analysis so that appropriate alerts can be sent to the drivers. Once processing is done, the streams are dumped into S3 using Kinesis Data Firehose.

### Question 59:
The data science team at an ecommerce company wants to analyse and visualize the clickstream data as it arrives into the data lake. What combination of AWS serverless services would you recommend for the team:
* S3, Lambda, ElasticSearch, Kibana
* S3, EC2, D3.js
* S3, EMR, ElasticSearch, Kibana
* S3, Glue, Athena, QuickSight

### Question 60:
A Silicon Valley startup has introduced a new email service that aims to address the problem of email spam. The startup wants to be extra sure that genuine emails are not marked as spam. The underlying machine learning model’s predicted value of 1 implies that the model predicts a given email to be spam. The data scientists at the startup would like to analyze the results of the underlying model. Identify the most important evaluation metric for this model:
* Accuracy
* Precision
* F1-score
* Recall

### Question 61:
When you create a training job with the SageMaker API, Amazon SageMaker replicates the entire dataset from S3 to ML compute instances by default. What option would you use to replicate only a subset of the data on each ML compute instance:
* Set the S3DataDistributionType field to ShardedByS3Key
* Set the S3DataType field to ShardedByS3Key
* Set the S3Uri field to ShardedByS3Key
* Set the S3DataDistributionType field to FullyReplicated

### Question 62:
Identify the mandatory hyperparameters for the SageMaker K-means algorithm (Select two):
* epochs
* k
* feature_dim
* mini_batch_size

### Question 63:
An ecommerce company wants to optimize the cost structure for its Redshift data warehouse by moving out some of the infrequently accessed data to S3. What solution would you recommend so that the company can still access this infrequently accessed data from Redshift whenever required:
* Create an EMR based Spark ETL job that writes the data from S3 back into Redshift. The job needs to be triggered every time the data needs to be analysed in Redshift
* Create an AWS Glue ETL job that writes the data from S3 back into Redshift. The job needs to be triggered every time the data needs to be analysed in Redshift
* Create a Glue crawler to read the S3 data via Athena so there is no need to use Redshift
* Use Redshift Spectrum so that the infrequently accessed data in S3 can be queried from Redshift.

### Question 64:
You are working on a click prediction system and you want to capture the underlying click rate patterns when ads from a certain ad-category are placed on pages from a certain page-category. Which SageMaker algorithm can be used to accomplish this:
* Factorization Machines
* XGBoost
* Blazing Text
* Latent Dirichlet Analysis

### Question 65:
As an ML Engineer using Amazon SageMaker, which are the user interface options you can use to train a SageMaker model (Select three) :
* SageMaker Console
* Jupyter Notebook
* AWS Batch
* SageMaker SDK
* AWS Glue

