# Neural_Network_Charity_Analysis

Berks is ready to put her skills to work to help the foundation predict where to make investments. I will help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

•	EIN and NAME—Identification columns
•	APPLICATION_TYPE—Alphabet Soup application type
•	AFFILIATION—Affiliated sector of industry
•	CLASSIFICATION—Government organization classification
•	USE_CASE—Use case for funding
•	ORGANIZATION—Organization type
•	STATUS—Active status
•	INCOME_AMT—Income classification
•	SPECIAL_CONSIDERATIONS—Special consideration for application
•	ASK_AMT—Funding amount requested
•	IS_SUCCESSFUL—Was the money used effectively

Steps:

The First steps involved data cleaning, such as removing EIN and Name columns: 
application_df = application_df.drop(["EIN", "NAME"], axis=1)
application_df
Once the unique values and application counts were found we were able to plot the information on an initial plot.  
 

A new dataframe was then created for application types, and they were classified for binning. The new information was plotted to create a value count for the classifications. 
 

Once the above steps were done the remainder of the work was done to generate categorical variable lists consisting of: 
	
['APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS']
The new dataframes with encoded variables were created as well as hot- encoded features. We the split our preprocessed data into features and target rays. After a standard scaler was created the next step of compiling, training and evaluated the model was done. The outcome will be discussed the summary.

Summary

One the model was run the ultimate result was a loss of 1.3837… and a accuracy of .6942… I think more analysis could be done to get a higher accuracy score. Given the time constraints, Berks can use this analysis to help the foundation predict where to make investments. I don’t belive the full project is complete and believe there is more to be done to provide clearer analysis. 

