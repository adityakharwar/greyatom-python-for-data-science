### Project Overview

 We have been hired by the stakeholders of Dream Housing Finance company to help them get visual insights on the company's operations. Using the data visualization techniques we learned, we have to help visualise the data and see if we can help the stakeholders arrive at some inference based on the visual plots.


### Learnings from the project

 After completing this project, we have a better understanding of data visualization techniques. In this project, we apply the following concepts:

Bar plotting
Scatter plotting
Kernel Density plotting
Subplot operations
Axes modifications


### Approach taken to solve the problem

 Step 1:

->Let's start with the simple task of visualizing the company's record with respect to loan approvals.

->Save the value counts of Loan_Status in a variable called loan_status using value_counts()

->Plot a bar graph of loan_status

Step 2:

->Group the 'data' dataframe by Property_Area and Loan_Status and store it in a variable called 'property_and_loan'

->Use the .size() method on 'property_and_loan' and then use .unstack() and save it back to 'property_and_loan'

->Plot an unstacked bar plot of property_and_loan (It is similar to creating a stacked bar plot except change the parameter 'stacked' to False)

->Name the x-axis as Property Area

->Name the y-axis as Loan Status

->Rotate the labels of x-axis by 45 degree.

Step 3:

->Group the 'data' dataframe by Education and Loan_Status and store it in a variable called 'education_and_loan'

->Use the .size() method on 'education_and_loan' and then use .unstack() and save it back to 'education_and_loan'

->Plot an stacked bar plot of education_and_loan

->Name the x-axis as Education Status

->Name the y-axis as Loan Status

->Rotate the labels of x-axis by 45 degree.

Step 4:

->Create a dataframe called 'graduate' which is a subset of 'data' dataframe with the condition "data['Education'] == 'Graduate'"

->Create a dataframe called 'not_graduate' which is a subset of 'data' dataframe with the condition "data['Education'] == 'Not Graduate'"

->Plot a density plot LoanAmount of 'graduate' dataframe using "Series.plot()" and pass the parameter kind='density' and label='Graduate'

->Do the same for LoanAmount of 'not_graduate' dataframe but with label='Not Graduate'

Step 5:

->Create three subplots with (nrows = 3 , ncols = 1) and store it in variable's fig ,(ax_1,ax_2,ax_3)

->Since both are continuous variables, plot scatter plot between 'ApplicantIncome' and LoanAmount using ax_1. Set axis title as Applicant Income

->Plot scatter plot between 'CoapplicantIncome' and LoanAmount using ax_2. Set axis title as Coapplicant Income

->Create a new column in the dataframe called 'TotalIncome' which is a sum of the values of columns ApplicantIncome and CoapplicantIncome

-.Plot scatter plot between 'TotalIncome' and LoanAmount using ax_3. Set axis title as Total Income



### Challenges faced

 None


### Additional pointers

 No


