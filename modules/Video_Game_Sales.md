## Video Game Sales


In this module, we'll work our way through an example Jupyter notebook that demonstrates how to use a built-in algorithm in SageMaker. More specifically, we'll use SageMaker's version of XGBoost, a popular and efficient open-source implementation of the gradient boosted trees algorithm. 

Gradient boosting is a supervised learning algorithm that attempts to predict a target variable by combining the estimates of a set of simpler, weaker models. XGBoost has done remarkably well in machine learning competitions because it robustly handles a wide variety of data types, relationships, and distributions. It often is a useful, go-to algorithm in working with structured data, such as data that might be found in relational databases and flat files. 

This module also shows how to use SageMaker's built-in algorithms via hosted Jupyter notebooks and the SageMaker console.  To proceed, follow these steps:

1. Download the Video Game csv dataset here (./assets/Video_Games_Sales_as_at_22_Dec_2016.csv)

2. **Exploratory Data Analysis**:  For this part of the module, we'll be using a SageMaker notebook instance to explore and visualize a data set.  

3. Go to the Jupyter homepage from the SageMaker notebook instance.

![Jupyter](./images/jupyter-homepage.png)

4. In the Jupyter homepage, click on the SageMaker Examples tab then **Introduction to appling machine learning** section and click on the **Use** button in **video-game-sales-xgboost.ipynb** row.

![xgboost](./images/xgboost-use.png)

5. In the pop up dialog box, click **Create copy** button to create and launch a copy of the notebook.

6. Click on **Jupyter** icon on the top left screen. 

![xgboost-Jupyter](./images/xgboost-jupyter-icon.png)

6. Click on **video_games_sales_####** folder.

7. Make sure you are in the **video_games_sales_###** folder then click on **upload** button and upload the csv file from step 1. Select the csv file on your computer and then click **upload button** again. 

![xgboost-upload](./images/xgboost-jupyter-upload.png)

8. Click on **video-game-sales-xgboost.ipynb** file and follow the directions in the notebook. Note that you no longer need to download dataset from Kaggle as you have already done so from previous steps so it's perfectly safe to ignore that instruction in the notebook.

6. In the first coding block, find ```bucket = session.default_bucket()``` code line, paste the name of the S3 bucket you created in [**Creating a Notebook Instance**](../NotebookCreation) to replace ```session.default_bucket()```.  The code line should now read similar to ```bucket = 'sagemaker-workshop-john-smith'```.  Do NOT paste the entire path (s3://.......), just the bucket name. 

![xgboost-bucket](./images/xgboost-bucket.png)

7. In addition to the output of training job in Jupyter, you can also check the status of your training jobs in the SageMaker console.  the SageMaker console, click **Jobs** in the left panel to check the status of the training job.  When the job is complete, its **Status** column will change from InProgress to Complete.  As a reminder, duration of this job can last up to about 10 minutes, including time for setting up the training cluster.

- To check the actual training time (not including cluster setup) for a job when it is complete, click the training job name in the jobs table, then examine the **Training time** listed at the top right under **Job Settings**.  

8. When you're finished, return back to [**Introduction to SageMaker**](../Introduction) to move on to the next module.

