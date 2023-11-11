

# San-Francisco-Crime-Geographical-Clustering_using_Machine_Learning

![](san_francisco.gif)

# SAN FRANCISCO CRIME GEOGRAPHICAL CLUSTER PROJECT

<p>In this lesson, we will perform geographic clustering using the San Francisco crime dataset on Kaggle. You can download the dataset from Kaggle: https://www.kaggle.com/c/sf-crime/data</p>

<p>Please just download train.csv.zip and unzip the file into the same directory as this Python source code.</p>

<p><b>The operation steps of this project are as follows:</b></p>

- 1. Import libraries and prepare the dataset.
- 2. Decide how many clusters we will have using the Elbow Method (we will find the value of K).
- 3. Build the model and perform clustering using the K-Means Machine Learning algorithm.
- 4. Visualize our clustering results in the well-known geographical map system (OpenStreetMap)
- 5. Finally, we will export our resulting geographical map to an html file so that it can be easily found on any website.

<p>We will use only Python for all the above tasks, including geographical map drawing! Before starting our project, you must install the Plotly Python library in your Anaconda 3 environment. # You can plot into your Anaconda Environment using the following command from the Anaconda command prompt:     conda scheduled installation</p>





### STEP 1. Import libraries and prepare the dataset
- Y is latitude and X is longitude...
- Since we will only use Lat, Lng for clustering, we left unnecessary PdDistrict, PdDistrict columns.
- We also reduce properties such as Resolution, Description because we do not need them for clustering

##### dataset includes information from 2003 to 2015. We will only use data from 2014.

- For this purpose, we will now perform year filtering.


- Categorize the dataset by year, otherwise it will be too long to process.
- For this project we will only use 2014 values, but you can easily change this if you wish.
- We scale data for accurate results...
- Y is latitude and X is longitude...
- Any location in the world can be described using Latitude and Longitude geographical coordinate values.
- Please note that since we will be using the original values, we are storing the scaled values in the new columns (X_scaled and Y_scaled).




### STEP 2. Decide how many clusters we will have using the Elbow Method (we will find the value of K).

<p>K is a hyperparameter (the designer needs to decide the value of K). Here K is the number of clusters, we tell the model how many clusters we want.

So how can we decide the value of K? Don't worry, there is a method called the Elbow Method to define the K hyperparameter...

For this purpose we will use the Elbow Method, try K values from 1 to 15 and find the best K value.</p>

### STEP 3. Build the model and perform clustering using K-Means Machine Learning algorithm

- Let's create a K-Means model for #K=5:

### STEP 4. Visualize our clustering results

- Geographic Map Creation using our Machine Learning model results...
- We will use the Plotly library for Geographic Map Drawing.
- You can plot into your Anaconda Environment using the following command from the Anaconda command prompt:
- You can install the plotly module with "conda install plotly" in the Anaconda command prompt.

### STEP 5. Finally we will export our resulting geographic map into a html file so that it can be used in any web site easily

- if you want to use another basemap or use other methods of plotly you can get info using help(px.scatter_mapbox):

