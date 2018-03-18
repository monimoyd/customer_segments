# Content: Unsupervised Learning
## Project: Creating Customer Segments

### Project Overview
In this project I applied unsupervised learning techniques on product spending data collected for customers of a wholesale distributor in Lisbon, Portugal to identify customer segments hidden in the data. I first explored the data by selecting a small subset to sample and determine if any product categories highly correlate with one another. Afterwards, I preprocess the data by scaling each product category and then identifying (and removing) unwanted outliers. With the good, clean customer spending data, I applied PCA transformations to the data and implement Gaussian Mixture Model (GMM) clustering algorithms to segment the transformed customer data and choose the cluster with best Silhouette Score. Finally, I compared the segmentation found with an additional labeling to verify the clustering done. Also, I suggested A/B testing so as to assist the wholesale distributor with future service schedule from five days a week to 3 days a week. Finally, I suggested a way to use supervised learning algorithm which can be used for the same problem in future.

### Install

This project requires **Python 2.7** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. Make sure that you select the Python 2.7 installer and not the Python 3.x installer. 

### Code

The main code`customer_segments.ipynb` notebook file. You will also be required to use the included `visuals.py` Python file which performs rendering of output. `customers.csv` dataset  440 data points collected on data found from clients of a wholesale distributor in Lisbon, Portugal. Additionally report.html file contains a snapshot of the main code in the jupyter notebook with all code cells executed. 

Thanks to Udacity for some of the code and datasets used in this project
### Run

In a terminal or command window, navigate to the top-level project directory `customer_segments/` (that contains this README) and run one of the following commands:

```bash
ipython notebook customer_segments.ipynb
```  
or
```bash
jupyter notebook customer_segments.ipynb
```

This will open the Jupyter Notebook software and project file in your browser.

## Data

The customer segments data is included as a selection of 440 data points collected on data found from clients of a wholesale distributor in Lisbon, Portugal. More information can be found on the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers).

Note (m.u.) is shorthand for *monetary units*.

**Features**
1) `Fresh`: annual spending (m.u.) on fresh products (Continuous); 
2) `Milk`: annual spending (m.u.) on milk products (Continuous); 
3) `Grocery`: annual spending (m.u.) on grocery products (Continuous); 
4) `Frozen`: annual spending (m.u.) on frozen products (Continuous);
5) `Detergents_Paper`: annual spending (m.u.) on detergents and paper products (Continuous);
6) `Delicatessen`: annual spending (m.u.) on and delicatessen products (Continuous); 
7) `Channel`: {Hotel/Restaurant/Cafe - 1, Retail - 2} (Nominal)
8) `Region`: {Lisbon - 1, Oporto - 2, or Other - 3} (Nominal) 