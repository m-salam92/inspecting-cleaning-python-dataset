# Inspecting and Cleansing Datasets Using Python 

In order to do well in this course all you need to have is a willingness to learn Python! A little bit of data engineering knowledge helps too. 

# Introduction 

I have over 7 years experience as a Data Scientist in the 'real world' including working for Big Four consulting firms. I started out as a Junior Data Engineer then transitioned to a Data Scientist. Many of my everyday problems I solve revolve around cleansing data. 

Forbes.com did a study in 2016 where they asked a handful of data scientist what their job pertains. This was done to simple show what areas data scientist focus on the most. The results may surprise you... 


![image](https://user-images.githubusercontent.com/83152100/116005886-f8c24e00-a5d6-11eb-833b-e22f036a3307.png)


As you can see in the graphic, 60% of the time Data Scientist are spending cleaning and organizing data! 
Now that I have gotten you really excited to start lets get our hands dirty and get to it!


# Install Python IDE 

You will first need to install Anaconda Navigator to use Python Jupyter Notebooks. Jupyter notebooks is great for Data Analysis, Data Manipulation, Data Cleansing etc. Here is a link to download Anaconda: https://www.anaconda.com/products/individual 


# Install Packages 

Python has many built in modules that allow programmers to perform certain functions. Pandas and Numpy are two of the best packages known for data analysis. You can learn more about python if you visit this link: https://pandas.pydata.org/ 

Below you will find a few lines of code to install and load Pandas package 

![image](https://user-images.githubusercontent.com/83152100/116189529-125ab700-a6f7-11eb-9071-3a56057a96be.png)


# Data Exploration 

I have built a sample Employee Database Dataset consisting of few sample rows. Here are the following Data Attributes. 

- Emp_ID: Unique Employee ID
- First_Name: Employee's First Name
- Last_Name: Employee's Last Name
- Emp_Lvl: Employee's Rank Level
- Emp_Dept: Main Department Employee is assigned to
- Emp_Salary: Employee's Annual Base Salary 
- Emp_State: State Employee resides in


# Assessment 1: Reading a CSV Data File into a Python DataFrame (df)
# Assessment 2: Printing and Inspecting a subset of data 

Now that you have installed and loaded pandas, store your csv file into a python dataframe. You will see the solution below. 

![image](https://user-images.githubusercontent.com/83152100/116191265-07555600-a6fa-11eb-96c1-65c1f1c8ae54.png)

Note: It is a good idea to set encoding = 'unicode_escape'; this uses a string that is suitable as Unicode literal in Python source code in case your csv has other characters. 
df.head() will provide you the first 5 rows of data. 

# Assessment 3: Determining the number of rows/columns into a tabular dataset

We will now try to find how many rows/columns exist in my employee dataset

![image](https://user-images.githubusercontent.com/83152100/116191125-c8270500-a6f9-11eb-86aa-e6a1434cbd76.png)

We first set the length equal to our rows and columns variable then we print it. 
At the bottom of the image you can see: 

Number of Rows= 10
Number of Columns = 7

# Assessment 4: Finding Missing Data 

Now, we will determine whether or not this df has missing values. 
You simply do this by one line of code: df.isnull()

![image](https://user-images.githubusercontent.com/83152100/116191634-ab3f0180-a6fa-11eb-8763-b882c32fa7a5.png)

There is only one 'True' missing value in my dataframe which is the employee level in row 8. 

# Assessment 5: Finding Duplicate Data

We now run a simple command 'df.duplicated()' to show us where there may be duplicated entries, we find one in row 2/3.

![image](https://user-images.githubusercontent.com/83152100/116192151-72535c80-a6fb-11eb-882c-b9845d4bf9d5.png)
 
 We then run the 'df.drop_duplicates()' command to drop the duplicate value 
 
 ![image](https://user-images.githubusercontent.com/83152100/116192307-aaf33600-a6fb-11eb-8897-167e108594f9.png)

Now as you can see, David Jackson is only coming in once! 
 
 # Assessment 6: Data Type and Ensure Data is properly encoded 
 
 Lastly, we want to make sure we know what the data type is coming in for each column. 
 
 We notice that Emp_Salary is coming in as an int.. We want to change that to a float to make sure there is some flexibility as salary can range into decimal numbers so we do that converting it using the code df["Emp_Salary"].astype(float) 
 
 ![image](https://user-images.githubusercontent.com/83152100/116193371-3caf7300-a6fd-11eb-9b6d-8f6af2b0ed10.png)

# Conclusion 

I hope you were able to pick up some basic data manipulation/data cleansing/data ingesting techniques with me. Stay tuned for additional walkthroughs of working with data. I love using the pandas package, it is a very powerful tool that allow for many functions with simple lines of code as you may have seen. 

