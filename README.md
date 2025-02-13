Visualize data with Amazon QuickSight by Shravani Durgi
Let’s use Amazon QuickSight to visualize Netflix data and trends.
Amazon QuickSight helps in analyzing the data and creating the visualizations easily.

Summary:
For this project, we are going to analyze a huge dataset of Netflix shows and movies to create a dashboard that extracts all the insights and we’ll be using Amazon S3 to store and retrieve the data.

Amazon Services we’ll use:
•	Amazon S3
•	Amazon QuickSight

Project:
In just 7 steps, we will be able to visualize the insights.
Step 1: Download the Dataset
•	Download netflix_titles.csv. (right click, and select Save Link As). This file contains all the data we're analysing!
•	Download manifest.json. (right click, and select Save Link As). . It’s important to edit this file because keeping an outdated S3 URI means manifest.json points to the wrong address.
Step 2: Uploading the data into Amazon S3
1.	Open the console and search for S3 and click “Create Bucket”.
2.	Name the bucket and make sure it includes your name
3.	Choose the region closest to you because of two reasons; one is cost and other is latency, as if it is farther away from you its going to take more time to render and will be charged more.
4.	Then click, “Create Bucket”.
5.	Then choose the bucket we have just created and upload the csv file and manifest.json into the bucket.
6.	Copy the S3 URI of the csv file and paste it in the manifest.json file.

 

Step 3: Create your Amazon QuickSight Account
1.	Open the AWS management console and navigate to Amazon QuickSight.
 

2.	Then, sign up for QuickSight. Then, you will find this page select the region near to you.
 
3.	Then give the account name  and in the allow access section click Amazon S3 along with the default resources. In S3 choose the bucket in which your data files are present.
 
4.	Make sure to uncheck the Add Pixel-Perfect Reports.
 
5.	Click finish and then the account will be created in a minute
 

Step 4: Connect your S3 bucket to QuickSight
1.	In the QuickSight menu, navigate to Datasets and click New Dataset.
2.	Then Select s3.
3.	Then enter the source name. I named it as kaggle-netflix-data and copy the S3 URI of the manifest.json from S3.


     

The manifest.json file is like a map that tells Amazon QuickSight where your data files are and how they are organized. It also describes what each piece of data looks like, so QuickSight knows how to understand the data and show it in charts or graphs. Without this, QuickSight might get confused and show the improper data.
4.	Click create and then Visualize.
Step 5: Create your First QuickSight Visualisation.
1.	We can see in the left panel that the data has already been imported
2.	Create first visualization and I chose horizontal bar chart and drag release_year into Y Axis heading.
 
3.	You can create different types of charts. Lets create Donut chart and then you can minimize the chart so that one more chart can be added.

 
4.	Now lets create Horizontal Bar Chart and drag the release_year label to Y-Axis and then drag type to Group.

 
Step 6: Your QuickSight treasure hunt
Explore the dashboard and see if we can add few more visualizations.
 

Step 7: Finalize the touches.
I have added few more visualizations and then clicked File and then click ‘File to PDF’.


