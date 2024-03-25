# BUILDING A DEMAND FORECASTING MODEL 
-----------------------------------

![Shopping Cart](https://media.istockphoto.com/id/513984990/vector/young-woman-pushing-supermarket-shopping-cart.jpg?s=612x612&w=0&k=20&c=0j5sgsyfAwjlg4CU2yNngIpoCjjexv1qeyqdqQSssEE=)

Building a demand forcasting model project is used to predict e-commerce product demand using PySpark to answer business questions regarding supply chain efficiency.

**Problem Statement:**

It's simple to buy any product with a click and have it delivered to your door. Online shopping has been rapidly evolving over the last few years, making our lives easier. But behind the scenes, e-commerce companies face a complex challenge that needs to be addressed.

Uncertainty plays a big role in how the supply chains plan and organize their operations to ensure that the products are delivered on time. These uncertainties can lead to challenges such as stockouts, delayed deliveries, and increased operational costs.
You work for the Sales & Operations Planning (S&OP) team at a multinational e-commerce company. They need your help to assist in planning for the upcoming end-of-the-year sales. They want to use your insights to plan for promotional opportunities and manage their inventory. This effort is to ensure they have the right products in stock when needed and ensure their customers are satisfied with the prompt delivery to their doorstep.

**DATA**
-----
The data for this project is [Online Retail.csv](https://app.datacamp.com/workspace/w/2fc84039-008c-468d-8753-ab449d11158e/edit) gotten from the project work space on DataCamp

**Project Applications:**

This project can be applied for the following
  - Inventory Management
  - Production Planning
  - Risk Management
  - Customer Service Optimization

**Insatallation**
`pip install pyspark`

**Project Instructions:**
Analyze the Online Retail.csv dataset and build a forecasting model to predict 'Quantity' of products sold.

Split the data into two sets based on the splitting date, "2011-09-25". All data up to and including this date should be in the training set, while data after this date should be in the test set. Return a pandas DataFrame, pd_daily_train_data, containing, at least, the columns "Country", "StockCode", "InvoiceDate", "Quantity".

Using your test set, calculate the Mean Absolute Error (MAE) for your forecast model for the 'Quantity' sold? Return a double (float) named mae.

How many units are expected to be sold during the week 39 of 2011? Store as an integer variable called quantity_sold_w39.

**PROJECT STEPS**
-----------------------
1. Import Libraries
2. Initiate Spark Session
3. Import Data
4. Data Processing
    - Convert the InvoiceDate to datetime
    - Aggregate the Data into Daily Intervals
5. Split Dataset into train aand test set
6. Feature Engineering
    - Creating indexer for categorical columns
    - Select features columns
7. Build Regression Model
    - Initialize the regressor
    - Create a pipeline for staging the processes
8. Train Model
9. Evaluate Model
10. Inference

**Acknowledement:**
Thanks to I4G for sponsoring  my Datacamp Premium account.

**Challenges:**
- Computational Cost
- PySpark RuntimeError: Java gateway process exited
In order to solve the run time error, check out [Alexandre Warembourg](https://towardsdatascience.com/pyspark-demand-forecasting-data-science-project-dae14b5319cc) post


