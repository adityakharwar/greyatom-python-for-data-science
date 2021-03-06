### Project Overview

 Analysis Loan Approval


### Learnings from the project

 Let's check which variable is categorical and which one is numerical so that we get a basic idea about the features of the bank dataset.

* The path for the dataset has been stored in a variable path

* Create dataframe bank by passing the path of the file

* Create the variable 'categorical_var' and using 'df.select_dtypes(include = 'object')' check all categorical values.

* print 'categorical_var'

* Create the variable 'numerical_var' and using 'df.select_dtypes(include = 'number')' check all categorical values.

* print 'numerical_var'

Step 2: Sometimes customers forget to fill in all the details or they don't want to share other details. Because of that, some of the fields in the dataset will have missing values. Now we have to check which columns have missing values and also check the count of missing values each column has. We  get the columns that have missing values, try to fill them.

From the dataframe bank, drop the column Loan_ID to create a new dataframe banks

To see the null values, use "isnull().sum()" function and print it.

Calculate mode for the dataframe banks and store in bank_mode

Fill missing(NaN) values of banks with bank_mode and store the cleaned dataframe back in banks.

Check if all the missing values (NaN) are filled.



Step 3: Now let's check the loan amount of an average person based on 'Gender', 'Married', 'Self_Employed'. This will give a basic idea of the average loan amount of a person.

We will use previously created dataframe banks for this task.

Generate a pivot table with index as 'Gender', 'Married', 'Self_Employed' and values as 'LoanAmount', using mean aggregation

Store the result in a variable called 'avg_loan_amount'



Step 4: Now let's check the percentage of loan approved based on a person's employment type.

We will use the previously created dataframe banks for this task.

Create variable 'loan_approved_se' and store the count of results where Self_Employed == Yes and Loan_Status == Y.

Create variable 'loan_approved_nse' and store the count of results where Self_Employed == No and Loan_Status == Y.



Calculate the percentage of loan approval for self-employed people and store result in variable 'percentage_se'.

Calculate the percentage of loan approval for people who are not self-employed and store the result in variable 'percentage_nse'.


Step 5: A government audit is happening real soon! So the company wants to find out those applicants with long loan amount term.

Use "apply()" function to convert Loan_Amount_Term which is in months to a year and store the result in a variable 'loan_term'.

Find the number of applicants having loan amount term greater than or equal to 25 years and store them in a variable called 'big_loan_term'.

big_loan_term should be 554.

Step 6: Now let's check the average income of an applicant and the average loan given to a person based on their income.

Groupby the 'banks' dataframe by Loan_Status and store the result in a variable called 'loan_groupby'

Subset 'loan_groupby' to include only ['ApplicantIncome', 'Credit_History'] and store the subsetted dataframe back in 'loan_groupby'

Then find the mean of 'loan_groupby' and store the result in a new variable 'mean_values'


### Approach taken to solve the problem

 After completing this project, you will have better grip on working with pandas. In this project you will apply following concepts.

1) Dataframe slicing
2) Dataframe aggregation
3) Pivot table operations


### Challenges faced

 None


### Additional pointers

 No


