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


# Assessment 1: Load Employee CSV File into Python DataFrame (df)

Now that you have installed and loaded pandas, store your csv file into a python dataframe. You will see the solution below. 

![image](https://user-images.githubusercontent.com/83152100/116190217-379bf500-a6f8-11eb-8b59-19b21af8efba.png)

Note: It is a good idea to set encoding = 'unicode_escape'; this uses a string that is suitable as Unicode literal in Python source code in case your csv has other characters. 
df.head() will provide you the first 5 rows of data. 


