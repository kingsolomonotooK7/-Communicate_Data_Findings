# Prosper Loan Data Data Exploration and Visualization
## by King Solomon Otoo


## Dataset
This data set contains information on peer to peer loans facilitated by credit company Prosper. There are 113,937 loans 
with 81 variables. For the purpose of this investigation I've taken the following variables: Term, LoanStatus, 
BorrowerRate, ProsperRating (Alpha), ListingCategory (numeric),EmploymentStatus, DelinquenciesLast7Years, 
StatedMonthlyIncome, TotalProsperLoans, LoanOriginalAmount, LoanOriginationDate, Recommendations and Investors.
The dataset can be found in the

##### Data wrangling process:
- created new dataframe which made up of variables of interest from the main dataset and varibles include 'BorrowerRate', 
  'Term', 'Recommendations', 'ProsperRating (Alpha)', 'TotalProsperLoans', 'EmploymentStatus', 'StatedMonthlyIncome', 
  'LoanOriginalAmount', 'ListingCategory (numeric)','LoanOriginationDate','LoanStatus', 'Investors'.

- formated the 'LoanOriginationDate' column to proper date format.

- removed all null values based on 'ProsperRating (Alpha)'. Since Prosper use their own proprietary Prosper Rating only 
  since 2009, we have a lot of missing values in ProsperRating column.

- Created a new LoanStatus variable containiing only Defaulted and Completed values 


## Summary of Findings
The number of borrowers who completed their loans were more than those who defaulted. Borrower having the 'Employed' 
status accounted for borrowers with most loans and followed by 'Full-time' status.
The distribution of the Stated Monthly Income is skewed to the right and having the most income hovering around 5000. 
Also, the borrowers rate is fairly normally distributed considering smalll number of bins.
The  Prosper Rating 'D' accounted for the most defaulted loans and also the most completed loans and the Proper rating 
'AA' has the highest average of investors.
The Employed borrowers acquired the highest loan amount, followed by the Self-employed and also the part-time borrowers 
have acquired the least loan amount.
Loan Amount for both the defaulted and completed loan status spans around an amount of 5000 but defaulted tend to have smaller 
range of amount than completed.
The loan amount associted with the defaulted loan staus tend to be higher for employment status 'other', 'Not employed', 
'Retired' and 'Part-time' than that of the completed except for the employment status 'Employed' and 'Full-time'.
The average loan amount for defaulted loan status tends to larger than that of completed in term of Prosper Ratings and 
most of the defaulted comes from borrwers with Prosper rating 'AA'.


## Key Insights for Presentation
The plots chosen shows distribution of main variables, Loan status, Employment Status, Loan Amount and Prosper rating.
Number of loans completed versus number of loans defaulted and their resective percetages 
Employment Status that acquires more loans. 
Relationship between Loan Status counts  and Proper Rating'
Average Loan Amount varing in term of Proper rating for each Loan Status.
Differnces in the average Loan amounT for Employement status between Defaulted and Completed loans.
The variation in Loan Amount distribution for both Defaulted and Compelted Loan Status
