# AWS Certified Machine Learning Specialty Full Practice Exam

# Exam 1

### Question 1:
After training a deep neural network over 100 epochs, it achieved high accuracy on your training data, but lower accuracy on your test data, suggesting the resulting model is overfitting. What are TWO techniques that may help resolve this problem?
* Use more layers in the network
* Use early stopping
* Use dropout regularization
* Employ gradient checking
* Use more features in the training data

### Question 2:
You are training an XGBoost model on SageMaker with millions of rows of training data, and you wish to use Apache Spark to pre-process this data at scale. What is the simplest architecture that achieves this?
* Use Sparkmagic to pre-process your data within a SageMaker notebook, transform the resulting Spark DataFrames into RecordIO format, and then use Spark's XGBoost algorithm to train the model.
* Use sagemaker_pyspark and XGBoostSageMakerEstimator to use Spark to pre-process, train, and host your model using Spark on SageMaker.
* Use Amazon EMR to pre-process your data using Spark, and then use AWS Data Pipelines to transfer the processed training data to SageMaker
* Use Amazon EMR to pre-process your data using Spark, and use the same EMR instances to host your SageMaker notebook.

### Question 3:
Your company wishes to monitor social media, and perform sentiment analysis on Tweets to classify them as positive or negative sentiment. You are able to obtain a data set of past Tweets about your company to use as training data for a machine learning system, but they are not classified as positive or negative. How would you build such a system?
* Use Amazon Machine Learning with a binary classifier to assign positive or negative sentiments to the past Tweets, and use those labels to train a neural network on an EMR cluster.
* Use RANDOM_CUT_FOREST to automatically identify negative tweets as outliers.
* Use SageMaker Ground Truth to label past Tweets as positive or negative, and use those labels to train a neural network on SageMaker.
* Stream both old and new tweets into an Amazon Elasticsearch Service cluster, and use Elasticsearch machine learning to classify the tweets.

### Question 4:
A large news website needs to produce personalized recommendations for articles to its readers, by training a machine learning model on a daily basis using historical click data. The influx of this data is fairly constant, except during major elections when traffic to the site spikes considerably. Which system would provide the most cost-effective and reliable solution?
* Publish click data into Amazon Elasticsearch using Kinesis Firehose, and query the Elasticsearch data to produce recommendations in real-time.
* Publish click data into Amazon S3 using Kinesis Streams, and process the data in real time using Splunk on an EMR cluster with spot instances added as needed. Publish the model's results to DynamoDB for producing recommendations in real-time.
* Publish click data into Amazon S3 using Kinesis Firehose, and process the data nightly using Apache Spark and MLLib using reserved instances in an EMR cluster. Publish the model's results to DynamoDB for producing recommendations in real-time.
* Publish click data into Amazon S3 using Kinesis Firehose, and process the data nightly using Apache Spark and MLLib using spot instances in an EMR cluster. Publish the model's results to DynamoDB for producing recommendations in real-time.

### Question 5:
You are developing a machine learning model to predict house sale prices based on features of a house. 10% of the houses in your training data are missing the number of square feet in the home. Your training data set is not very large. Which technique would allow you to train your model while achieving the highest accuracy?
* Impute the missing values using the mean square footage of all homes
* Impute the missing square footage values using kNN
* Impute the missing values using deep learning, based on other features such as number of bedrooms
* Drop all rows that contain missing data

### Question 6:
Your automatic hyperparameter tuning job in SageMaker is consuming more resources than you would like, and coming at a high cost. What are TWO techniques that might reduce this cost?
* Use inference pipelines
* Use linear scales on your parameter ranges
* Use less concurrency while tuning
* Use more concurrency while tuning
* Use logarithmic scales on your parameter ranges

### Question 7:
You are developing a computer vision system that can classify every pixel in an image based on its image type, such as people, buildings, roadways, signs, and vehicles. Which SageMaker algorithm would provide you with the best starting point for this problem?
* Object2Vec
* Rekognition
* Object Detection
* Semantic Segmentation

### Question 8:
You wish to use a SageMaker notebook within a VPC. SageMaker notebook instances are Internet-enabled, creating a potential security hole in your VPC. How would you use SageMaker within a VPC without opening up Internet access?
* Disable direct Internet access when specifying the VPC for your notebook instance, and use VPC interface endpoints (PrivateLink) to allow the connections needed to train and host your model. Modify your instance's security group to allow outbound connections for training and hosting.
* No action is required, the VPC will block the notebook instances from accessing the Internet.
* Use IAM to restrict Internet access from the notebook instance.
* Uncheck the option for Internet access when creating your notebook instance, and it will handle the rest automatically.

### Question 9:
You are developing an autonomous vehicle that must classify images of street signs with extremely low latency, processing thousands of images per second. What AWS-based architecture would best meet this need?
* Use Amazon Rekognition in edge mode
* Develop your classifier with TensorFlow, and compile it for an NVIDIA Jetson edge device using SageMaker Neo, and run it on the edge with IoT GreenGrass.
* Develop your classifier using SageMaker Object Detection, and use Elastic Inference to accelerate the model's endpoints called over the air from the vehicle.
* Use Amazon Rekognition on AWS DeepLens to identify specific street signs in a self-contained manner.

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

### Question 10:
A system designed to classify financial transactions into fraudulent and non-fraudulent transactions results in the confusion matrix below. What is the recall of this model?

Larger image
* 74%
* 90%
* 66.67%
* 50%

# Exam 2

### Question 1:
An online retailer wishes to predict website traffic over the coming year on an hourly basis. This traffic fluctuates signficantly with both time of day and time of year. Which service could produce these recommendations with the least amount of development and operational overhead?
* Amazon Forecast
* LSTM model deployed to EC2 with a machine learning AMI
* Apache Spark MLLib
* SageMaker DeepAR

### Question 2:
You are ingesting images and text from a social media feed, and wish to label them with the subjects represented by each image or text post. Which services might play a role in this system? (SELECT TWO)
* Amazon Comprehend
* Amazon Transcribe
* Amazon Polly
* Amazon Lex
* Amazon Rekognition

### Question 3:
Your neural network is underfitting, and in response you've added more layers. Upon adding additional layers, your accuracy no longer converges successfully while training. What is the most likely cause?
* The learning rate needs to be increased.
* The additional layers are now causing your model to over-fit.
* Too many training epochs are being used.
* Use of a sigmoid activation function is leading to the "vanishing gradient" problem; ReLU may work better.

### Question 4:
You are training SageMaker's supervised BlazingText using file mode. Which is an example of a properly formatted line within the training file?
* __label__4 Linux ready for prime time, Intel says.
* __label__4 linux ready for prime time, intel says.
* __label4 linux ready for prime time, intel says.
* __label__4 linux ready for prime time , intel says .

### Question 5:
A legacy MapReduce job is running on EMR, and must ingest data that has been moved from HDFS to an S3 data lake. Which is a viable option for connecting the S3 data to MapReduce on EMR?
* MapReduce can talk natively to S3 using the s3a:// prefix
* Use EFS to connect MapReduce to the S3 bucket.
* Use EMRFS to connect MapReduce to S3, using the s3:// file prefix.
* Use Apache Hive as an intermediary between MapReduce and S3

### Question 6:
While training your deep neural network using accuracy as a loss function, its accuracy is evaluated against a validation set at each epoch. The accuracy against the validation set continues to increase with each epoch until the 100th epoch, at which point the accuracy against the validation set begins to decrease while accuracy on the training set continues to increase. What is likely happening?
* This is not an indication of a real problem and may be ignored.
* The model is beginning to overfit after 100 epochs. Early stopping will help.
* The model is beginning to underfit after 100 epochs. Adding more layers to the network will help.
* A different activation function needs to be used.

### Question 7:
You want to create AI-generated music, by training some sort of neural network on existing music and getting it to predict additional notes going forward. What architecture might be appropriate?
* ResNet50
* RNN
* CNN
* MLP

### Question 8:
You are training a Linear Learner model in SageMaker, with normalization enabled. However, your training is failing. What might be a probable cause?
* The data was not shuffled prior to training.
* Normalization should be disabled.
* The data was shuffled prior to training.
* You are attempting to perform classification instead of regression.

### Question 9:
You are training a distributed deep learning algorithm on SageMaker within a private VPC. Sensitive data is being used for this training, and it must be secured in-transit. How would you meet this requirement?
* Enable server-side encryption in the S3 bucket containing your training data
* This isn't an option, and you must train on a single host in this case.
* Use SSE-KMS
* Enable inter-container traffic encryption via SageMaker's console when creating the training job

### Question 10:
Your machine learning system needs to be re-trained nightly on millions of records. The training involves multiple long-running ETL jobs which need to execute in order and complete successfully, prior to being handed off to a machine learning training workflow. Which is the simplest tool to help manage this process?
* AWS Step Functions
* Amazon Simple Workflow Service
* AWS Batch
* Amazon SQS

### Question 11:
You are receiving real-time data streams of raw data containing hundreds of columns of data on each record. Many of these columns are not needed for the machine learning system you are developing, and some of the remaining columns need to be concatenated or transformed in minor ways. What is the simplest and most storage-efficient way to transform this data as it is received?
* Process the data using Kinesis Data Streams and Amazon Kinesis Data Analytics. Within Kinesis Data Analytics, transform the data using SQL commands prior to sending the processed data to your analytics tools.
* Use a Glue ETL job on the streaming data to transform it after it is stored in S3.
* Use the spark-sagemaker library to process the data prior to training.
* Accept all of the data into S3, and drop the unneeded columns as part of preparing data for training.

### Question 12:
You have a large set of encyclopedia articles in text format, but do not have topics already assigned to each article to train with. Which tool allows you to automatically assign topics to articles with a minimum of human effort?
* Random Cut Forest
* Ground Truth
* LDA
* Amazon Translate

### Question 13:
An image recognition model using a CNN is capable of identifying flowers in an image, but you need an image recognition model that can identify specific species of flowers as well. How might you accomplish this effectively while minimizing training time?
* Use transfer learning by training the entire model with new labels
* Use incremental training on Amazon Rekognition
* Train a new CNN from scratch with only your flower species labels
* Use transfer learning by training a new classification layer on top of the existing model

### Question 14:
A recommender engine developed using SageMaker has been deployed using a custom inference model. You've tested an improvement to your model offline, but wish to expose it to production traffic to see how real people respond to it. How might you deploy this new model in a way that minimizes risk and operational effort?
* Write logic within your custom inference model to randomly assign traffic to one underlying model or the other, and ramp up the traffic to the new model over time.
* Deploy the model behind a second SageMaker endpoint, and use a load balancer to ramp up the traffic to the new model over time.
* Deploy the new model as a production variant behind the existing SageMaker endpoint. Increase the amount of traffic to the new model over time via SageMaker.
* This is just a bad idea, and you should evaluate this model offline instead using k-fold validation.

### Question 15:
Your XGBoost model has high accuracy on its training set, but poor accuracy on its validation set, suggesting overfitting. Which hyperparameter would be most likely to improve the situation?
* grow_policy
* booster
* csv_weights
* subsample

### Question 16:
You wish to control access to SageMaker notebooks to specific IAM groups. How might you go about this?
* Use S3 bucket policies to restrict access to the resources needed by the notebooks
* Integrate SageMaker with Active Directory
* Attach tags to the groups of SageMaker resources to be kept private to specific groups, and use ResourceTag conditions in IAM policies.
* Restrict access to the specific EC2 instances used to host the notebooks using IAM

### Question 17:
A dataset representing a clinical trial includes many features, including Mean Arterial Pressure (MAP). The various features are not well correlated, and less than 1% of the data is missing MAP information. Apart from some outliers, the MAP data is fairly evenly distributed. All other features contain complete information. Which is the best choice for handling this missing data?
* Impute the missing values with the median MAP value.
* Drop the MAP column
* Populate the missing MAP values with random noise
* Impute the missing values with the mean MAP value.

### Question 18:
You are using SageMaker and XGBoost to classify millions of videos into genres, based on each video's attributes. Prior to training your model, the video attribute data must be cleaned and transformed into LibSVM format. Which are viable approaches for pre-processing the data? (SELECT TWO)
* Use Kinesis Analytics to transform the data as it is received into LibSVM format, then train with SageMaker.
* Use scikit-learn in your SageMaker notebook to pre-process the data, and then train it.
* Use Spark on EMR to pre-process the data, and store the processed results in an S3 bucket accessible to SageMaker.
* Use Glue ETL to transform the data into LibSVM format, and then train with SageMaker.
* Use PySpark with the XGBoostSageMakerEstimator to prepare the data using Spark, and then pass off the training to SageMaker.

### Question 19:
A convention wishes to install cameras that automatically detect when conference attendees are seen wearing a specific company shirt, as part of a contest. Which is a viable approach?
* Use DeepLens and the DeepLens_Kinesis_Video module to send video streams to a CNN trained with SageMaker using a labeled training set of videos of the company shirts.
* Use DeepLens and the DeepLens_Kinesis_Video module to analyze video in real time using the ImageNet CNN.
* Use RNN's embedded within DeepLens to detect shirts at the edge
* Send raw video feeds into Amazon Rekognition to detect the company shirts

### Question 20:
You wish to use a model built with Tensorflow for training within a SageMaker notebook. To do so, you have created a Dockerfile with which you'll package your model into a SageMaker container, copying your training code with the command COPY train.py /opt/ml/code/train.py. What further needs to be done to define your train.py as the script entrypoint?
* Nothing; the entrypoint must be named train.py and this is assumed.
* Nothing; any script inside /opt/ml/code will be considered the entrypoint automatically.
* Include ENV SAGEMAKER_PROGRAM train.py in the Dockerfile
* Enter train.py as the entrypoint in the SageMaker console

### Question 21:
An e-commerce company needs to pre-process large amounts of consumer behavior data stored in HDFS using Apache Spark on EMR prior to analysis on a daily basis. The volume of data is highly seasonal, and can surge during holidays and big sales. What is the most cost-effective option for handling these sporadic demands, without incurring data loss or needing to terminate the entire cluster?
* Use EC2 Spot instances for core and task nodes, and reserved instances for the master node
* Use reserved instances for task nodes, and spot instances for core nodes.
* Use EC2 spot instances for all node types.
* Use EC2 Spot instances for Spark task nodes only.

### Question 22:
A classifier predicts if insurance claims are fraudulent or not. The cost of paying a fraudulent claim is higher than the cost of investigating a claim that is suspected to be fraudulent. Which metric should we use to evaluate this classifier?
* Specificity
* Recall
* Precision
* F1

### Question 23:
A training dataset contains several columns of features from census data, all of which are correlated in some way. One column, representing a person's age, is missing 10% of its values. What is the best way to handle these missing values to maximize accuracy in the resulting model?
* Drop the column that contains missing values
* Populate the missing values with random values
* Build a separate supervised model that predicts the value of the missing column based on the other columns, and use that to estimate the missing values.
* Impute the missing values based on the mean of the entire column

### Question 24:
A company maintains a large data lake in Amazon S3 containing a combination of structured and unstructured CSV data. Some of this data must be transformed and cleaned as it is received, and analysts within the company wish to analyze it using SQL queries. What solution would require the least amount of development work, lowest cost, and least ongoing maintenance?
* Transform the data using Apache Spark on EMR, and query it with RDS
* Use AWS Glue to transform the data, and query it using Redshift.
* Use AWS Glue to organize the unstructured data and transform it, and Amazon Athena to query the data.
* Tranform the data periodically with SageMaker, and query it with Redshift.

### Question 25:
You are deploying your own custom inference container on Amazon SageMaker. Which of the following are requirements of your container? (SELECT TWO)
* Accept all socket connection requests within 250 ms.
* Respond to both /invocations and /ping on port 80
* Must be compressed in ZIP format
* Respond to GET requests on the /ping endpoint in under 5 seconds.
* Respond to both /invocations and /ping on port 8080

### Question 26:
You have a massive S3 data lake containing clickstream data, and you wish to analyze and visualize this data in order to better understand the cleaning and feature engineering it might require. Which AWS services could be used to analyze and visualize this data, without provisioning individual servers in the process?
* S3, Kinesis, Amazon Elasticsearch
* S3, DMS, RDS
* S3, Glue, Athena, and QuickSight
* S3, EMR, Quicksight

### Question 27:
What is the F1 score of the confusion matrix below?  (columns represent actual values, and rows predicted values)

Larger image
* 0.6
* 0.67
* 0.36
* 0.73

### Question 28:
A large retailer wishes to publish revenue forecasts in a graphical manner for consumption by executives. Historical revenue data contains anomalies, such as spikes due to price drops. What is the simplest solution for providing these forecasts with the least amount of development effort and ongoing maintenance?
* Publish sales data into an RDS database, and produce forecasts and visualizations using Tableau
* Publish sales data into S3, and produce forecasts and visualizations with Amazon QuickSight
* Publish sales data into an EMR cluster, produce forecasts with Spark, and visualize with QuickSight
* Publish sales data into S3, use SageMaker to produce forecasts, and visualize with QuickSight

### Question 29:
A media company wishes to recommend movies to users based on the predicted rating of that movie for each user, using SageMaker and Factorization Machines. What format should the rating data used for training the model be in?
* CSV
* RecordIO / protobuf in integer format
* LibSVM
* RecordIO/ protobuf in float32 format

### Question 30:
You wish to categorize terabytes' worth of articles into topics using SageMaker and LDA, but processing that much data at once is leading to difficulties in storage and training the model reliably. What can be done to improve the performance of the system?
* Convert the articles to RecordIO format, and use Pipe mode
* Configure SageMaker to use multiple GPU's for training LDA
* Convert the articles to CSV format, and use Pipe mode
* Configure SageMaker to use multiple instances for training LDA

### Question 31:
If you wanted to build your own Alexa-type device that converses with customers using speech, which Amazon services might you use?
* Amazon Transcribe -> Amazon Comprehend -> Amazon Polly
* Amazon Comprehend -> Amazon Lex -> Amazon Polly
* Amazon Polly -> Amazon Lex -> Amazon Transcribe
* Amazon Transcribe -> Amazon Lex -> Amazon Polly

### Question 32:
A regression model on a dataset including many features includes L1 regularization, and the resulting model appears to be underfitting. Which steps might lead to better accuracy? (SELECT TWO)
* Increase the L1 regularization term
* Decrease the L1 regularization term
* Remove features
* Use L0 regularization
* Try L2 instead of L1 regularization

### Question 33:
You are running SageMaker training jobs within a private VPC with no Internet connectivity, for security reasons. How can your training jobs access your training data in S3 in a secure manner?
* Use NAT translation to allow S3 access
* Make the S3 bucket containing training data public
* Use bucket policies to restrict access to your VPC
* Create an Amazon S3 VPC Endpoint, and a custom endpoint policy to restrict access to S3

### Question 34:
A financial services company needs to automate the analysis of each day's transaction costs, execution reporting, and market performance. They have developed their own Big Data tools to perform this analysis, which require the scheduling and configuration of their underlying computing resources. Which tool provides the simplest approach for configuring the resources and scheduling the data analytic workloads?
* Amazon SQS
* Amazon Simple Workflow Service
* AWS Batch
* AWS Step Functions

### Question 35:
The graph below plots observations of two distinct classes, represented by blue and green, against two features, represented by the X and Y axes. Which algorithms would be appropriate for learning how to classify additional observations? (SELECT TWO)

Larger image
* PCA
* SVM with a RBF kernel
* SVM with a linear kernel
* Linear regression
* kNN

### Question 36:
The ROC curve below was generated from a classifier. What can we say about this classifier?

Larger image
* The AUC is 1.0
* This model has no discrimination capacity to distinguish between positive and negative classes.
* This model has perfect accuracy
* This model has a perfect measure of separability

### Question 37:
You are training a linear regression model the predicts income based on age, and a few other features. The training data contains several outliers from billionaires. How should these outliers be handled in order to maximize accuracy for the non-billionaires?
* Replace the income labels of the outliers with the median income value.
* Remove the outliers prior to training, identified as being outside some mutliple of a standard deviation from the mean
* Replace the income labels of the outliers with the mean income value.
* Keep all data intact, in order to produce the most accurate model.

### Question 38:
The graph below plots predicted and actual website views over time. Based on this graph, would you say the prediction model:

Larger image
* Captures seasonality and trends poorly
* Captures seasonality and trends well
* Captures seasonality well, but trends poorly
* Captures seasonality poorly, and trends well

### Question 39:
Which are best practices for hyperparameter tuning in SageMaker? (CHOOSE TWO)
* Use linear scales for hyperparameters
* Choose a large number of hyperparameters to tune
* Run only one training job at a time
* Run training jobs on a single instance
* Choose the smallest possible ranges for your hyperparameters

### Question 40:
You are tasked with developing a machine learning system that can detect the presence of your company's logo in an image. You have a large training set of images that do and do not contain your logo, but they are unlabeled. How might you prepare this data prior to training a supervised learning model with it, with the least amount of development effort?
* Use Amazon Rekognition
* Use Amazon SageMaker Ground Truth
* Use Amazon Mechanical Turk
* Use SageMaker Object Detection

### Question 41:
Which probability distribution would describe the likelihood of flipping a coin "heads"?
* Binomial Distribution
* Poisson Distribution
* Polynomial Distribution
* Normal Distribution

### Question 42:
You are analyzing Tweets from some public figure, and want to compute an embedding that shows past Tweets that are semantically similar to each other. Which tool would be best suited to this task?
* SageMaker Object2Vec
* Amazon Transcribe
* SageMaker BlazingText in word2vec mode
* SageMaker Factorization Machines

### Question 43:
You increased the batch size used to train your deep neural network, and found that the accuracy of the model suddenly suffered as a result. What is a likely cause?
* Too many layers are being used
* Shuffling should not be used
* The large batch size caused training to overshoot the true minima
* The large batch size caused training to get stuck in local minima

### Question 44:
Which is a valid approach for determining the optimal value of k in k-Means clustering?
* Use SGD to converge on k
* Use the "elbow method" on a plot of the total within-cluster sum of squares (WSS) as a function of k
* Use k-fold cross validation
* Use the "elbow method" on a plot of accuracy as a function of k

### Question 45:
A medical company is building a model to predict the occurrence of thyroid cancer. The training data contains 900 negative instances (people who don't have cancer) and 100 positive instances. The resulting model has 90% accuracy, but extremely poor recall. What steps can be used to improve the model's performance? (SELECT TWO)
* Collect more data for the positive case
* Generate synthetic samples using SMOTE
* Under-sample instances from the positive (has cancer) class
* Over-sample instances from the negative (no cancer) class
* Use Bagging

### Question 46:
You have created a SageMaker notebook instance using its default IAM role. How is access to data in S3 managed?
* Only S3 buckets with public access enabled are accessible
* Any bucket with "sagemaker" in the name is accessible with the default role
* The default IAM role allows access to any S3 bucket, regardless of name
* No buckets are available by default; you must edit the default IAM role to explicitly allow access.

### Question 47:
Your training data contains hundreds of features, many of which are correlated. You are having difficulty converging on a useful model due to the sparsity caused by hundreds of dimensions. How might you best pre-process this data to avoid this "curse of dimensionality?"
* Apply a factorization machine to the training data
* Drop half of the feature columns
* Concatenate columns together
* Apply PCA to the training data

### Question 48:
An advertising company is receiving a stream of consumer demographic data in JSON format, containing a large number of features such as age, income, location, and more. They wish to query this data and visualize it, in a manner as efficient and cost-effective as possible, without managing any servers in the process. Which would be the best approach to meet these goals?
* Use Kinesis Data Streams to store the data in S3. Use an EMR cluster to convert the data to Parquet format. Use a Glue crawler, Athena, and QuickSight to analyze and visualize the data.
* Stream the data into an Aurora database, where it may be queried directly.Use Aurora's JDBC connectivity to visualize the data with QuickSight.
* Use Kinesis Firehose to store the data in S3 in its original JSON format. Use QuickSight to visualize and analyze the data.
* Use Kinesis Firehose to convert the data to Parquet format and store it in an S3 data lake. Use a Glue crawler, Athena, and QuickSight to analyze and visualize the data.

### Question 49:
An advertising company wants to predict the likelihood of purchase, using a training data set containing hundreds of columns of demographic data such as age, location, and income. The large dimensionality of this data set poses a problem for training the model, and no features that represent broader groups of people are available. What would be a reasonable approach to reduce the dimensionality of the training data?
* Increase the model's learning rate
* Use KNN to cluster individuals into demographic groups used for training
* Apply a factorization machine to the training data
* Use K-Means clustering to cluster the people into demographic groups based on their other attributes, and train based on those groups.

### Question 50:
A random forest classifier was used to classify handwriten digits 0-9 into the numbers they were intended to represent. The confusion matrix below was generated from the results. Based on the matrix, which number was predicted with the least accuracy?

Larger image
* 8
* 6
* 3
* 0

### Question 51:
You are ingesting a data feed of subway ridership in near-real-time. Your incoming data is timestamped by the minute, and includes the total number of riders at each station for that minute. What is the simplest approach for automatically sending alerts when an unusually high or low number of riders is observed?
* Ingest the data with Kinesis Data Firehose, and use Random Cut Forest in Kinesis Data Analytics to detect anomalies. Use AWS Lambda to process the output from Kinesis Data Analytics, and issue an alert via SNS if needed.
* Publish data directly into S3, and use Glue to detect anomalies and pass on alerts to SNS.
* Ingest the data with Kinesis Firehose, and use Amazon CloudWatch to alert when anomalous data is detected.
* Ingest the data with Kinesis Data Streams directly into S3, and use Random Cut Forest in SageMaker to detect anomalies in real-time. Integrate SageMaker with SNS to issue alarms.

### Question 52:
You want to build a "Universal Translator" that can listen to speech in a variety of languages, translate it to English, and speak the translated text back to you. What sequence of AWS services would do this?
* Translate->Polly
* Translate->Transcribe->Polly
* Transcribe->Translate->Polly
* Transcribe->Comprehend->Polly

### Question 53:
A book publisher is ingesting a data feed into S3 containing features of various books coming from various sources. Many of these sources are sending data that is duplicated by other sources, and the S3 data lake where the data is being stored needs to be de-duplicated prior to further processing. What mechanism could achieve this goal with minimal development effort and ongoing maintenance?
* Use a Glue Crawler to identify and eliminate duplicate records as its table structure is being inferred.
* Periodically load the data into a Spark Dataframe on EMR, and use the dropDuplicates() function to remove the duplicates before passing it on for further processing.
* Import the data into Redshift, using a primary key that prevents duplicate records from being entered.
* Use AWS Glue's FindMatches ML Transform to identify and eliminate duplicate records as they are received.

### Question 54:
What is an appropriate choice of an instance type for training XGBoost in SageMaker?
* P2
* C4
* P3
* M4

### Question 55:
You are developing a machine translation model using SageMaker's seq2seq model. What format must your training data be provided in?
* RecordIO-protobuf with floating point tokens
* Text in CSV format
* RecordIO-protobuf format with integer tokens
* Text in JSON format

### Question 56:
Your deep neural network has achieved 99% accuracy on your training data, but only 90% on your test data. Human-level performance for the same task is around 98%. What are some possible conclusions (SELECT TWO)?
* The model is overfitting and failing to generalize. Using fewer layers may help.
* The model is underfitting, and more epochs will help.
* The model is overfitting and failing to generalize. Using dropout regularization may help.
* The model is overfitting and failing to generalize. Using more layers may help.
* The model is underfitting, and broader hidden layers are needed.

### Question 57:
You are building a neural network to estimate medical expenses based on a patient's blood pressure, among other attributes. Blood pressures are reported with two decimal points of precision, but must be encoded into a small number of discrete values for use in the network. Furthermore, the blood pressure values are very unevenly distributed, and we want to ensure low and high blood pressures carry significant weight in the model compared to normal blood pressures. Which technique could address both of these issues?
* Normalization
* Quantile binning
* Boosting
* Interval binning

### Question 58:
You are developing a deep learning model that categorizes handwritten digits 0-9 into the numbers they represent. How should you pre-process the label data?
* Hexadecimal
* Normalization
* Use integer values
* One-hot encoding

### Question 59:
A classifier that predicts if an image is of a cat or a dog results in the confusion matrix below  (columns represent actual values, and rows predicted values). What is the precision of this classifier?

Larger image
* 67%
* 70%
* 75%
* 80%

### Question 60:
A large retail chain receives dumps of sales data from each store on a daily basis into S3. Analysts need to run daily reports covering trends over the past 30 days using this data. After 90 days, the data may be archived. Which architecture allows for fast querying and archiving of this data, with the least cost?
* Copy the data nightly into Redshift, with a table for each day. Run a nightly script to drop tables older than 90 days.
* Organize the data into unique S3 buckets for each date, and use S3 lifecycle policies to archive the data after 90 days.
* Organize the data by prefixes that indicate the day the data covers, and use Glue to create tables partitioned by date. Use S3 lifecycle policies to automatically archive the data to Glacier after 90 days.
* Store all data into a single partition, and use Glue ETL to identify and discard data older than 90 days.

### Question 61:
You are training a regression model using SageMaker's Linear Learner, to predict individual incomes as a function of age and years in school. The training data was gathered from several distinct groups. What pre-processing should be performed to ensure good results? (SELECT TWO)
* Shuffle the input data
* Add some random noise to the training data
* Normalize the feature data to have a mean of zero and unit standard deviation
* Scale the feature data to match the range of income data
* Use SMOTE to impute additional data

### Question 62:
You've set up a camera in Los Angeles, and want to be notified when a known celebrity is spotted. Which services, used together, could accomplish this with the least development effort?
* SageMaker Object Detection, Lambda, and SNS
* SageMaker Semantic Segmentation, SQS, and SNS
* Amazon Rekognition, IAM, and SNS

### Question 63:
When using SageMaker's BlazingText algorithm in Word2Vec mode, which of the following statements are true?
* The order of words doesn't matter, as it uses skip-gram and continuous bag of words (CBOW) architectures.
* The order of words does matter, as it uses skip-gram and continuous bag of words (CBOW) architectures.
* The order of words does not matter, as it uses a CNN internally.
* The order of words matters, because it uses LSTM internally

### Question 64:
You've developed a custom training model for SageMaker using TensorFlow, but a single GPU can't handle the data it needs to train with. How would you go about scaling your algorithm to use multiple GPU's within SageMaker?
* Deploy your model to multiple EC2 P3 instances, and SageMaker will distribute it automatically
* Write your model with the Horovod distributed training framework, which is supported by SageMaker.
* This isn't possible with Tensorflow; use Apache MXNet instead.
* Wrap your Tensorflow code with PySpark, and use sagemaker-spark to distribute it.

### Question 65:
You increased the learning rate on your deep neural network in order to speed up its convergence, but suddenly the accuracy of the model has suffered as a result. What is a likely cause?
* The true minimum of your loss function was overshot while learning
* Too many layers are being used
* Shuffling should not be used
* SGD got stuck in local minima