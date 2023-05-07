# GCP_professional_data_engineer-notes
GCP PDE important points

GCP_professional_data_engineer-notes
Public
Cannot fork because you own this repository and are not a member of any organizations.
Code
Issues
Pull requests
Actions
Projects
Wiki
Security
Insights
Settings
Beta Try the new code view
GCP_professional_data_engineer-notes/Notes
@v850
v850 Create Notes
Latest commit 6ff3339 now
 History
 1 contributor
51 lines (37 sloc)  1.82 KB
 

Bigtable: NOSQL
  1. time-series, time Range
  2.row-key(keep reasonably short),Hbase
  3.minimum amount of data stored in cloud bigtable is 1TB
  4. use production instance to test
  5. Single-keyed data with low latency
  6. feild promotion =Avoid hotspoting
  
  
cloud storage: 1 TB, gsutil- data transfer from on-premises

tranfer appliance - more than 1 TB- on-premises to cloud

storage tranfer - cloud to cloud

Dataproc: charges for what you use with second by second and a low one minute minimum billing period.
  master mode: HDFS namenode and YARN ResourceManager
  
  *overfitting the model will have extremely low training error but a high testing error
  *underfitting the model will have extremely low testing but a high training error.
  
  Bigquery: Analytics
  By default, BigQuery caches query results for 24 hours,
  When you run a query, a temporary, cached results table is created in a special dataset referred to as an "anonymous dataset."
  can not load data from bigquery into google cloudSQL
  standardSQl prefered query language for BigQuery
  one diff. bet. standardSQL and legacy SQL is how you secify fully qualified name of table.
  partition table, nested repeated feilds and clustering keys
  partition table created only at table creation time
  upload can not be performed from bigquery webUI
  
Machine learning:
weights and bias are adjusted by Nueral network as learning from training data.
cloud ML engine allow you to specify worker and parameter servers type of cluster nodes.
gcloud ml-engine local train 
  command to run on your system using cloud ML engine.
online prediction:
  1. prediction response in return
  2. minimize latency in serving predictions
hyperparameter:
no.of hidden layer
no of nodes in hidden layer

feature engineering:
1. cross feature column
2. bucketization of continuous feature

  
Transferring from another cloud storage provider Use Storage Transfer Service.</br>
1. Transferring less than 1 TB from on-premises Use gsutil. </br>
2. Transferring more than 1 TB from on-premises Use Transfer service for on-premises data. </br>
Transferring less than 1 TB from another Cloud Storage region Use gsutil. </br>
Transferring more than 1 TB from another Cloud Storage region Use Storage Transfer Service </br> 
  
  
