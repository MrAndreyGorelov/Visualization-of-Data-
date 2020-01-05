# Visualization of Loan Data 

This is the last project of the Udacity Course. It focuses on applying all the codes learned into one, and completeing an analysis in order to interpret the findinds. 

# Introduction

In this porject I have deciced to choose the 'Loan Data from Prosper' optional topic to work with. In order to gain access to the data frame, I had to follow the link that immediately started to download the 'prosperLoanData' file for me. In there, I have chosen to analyse the information on the loans data like loan amount, interest rate, borrower rate, the status on the loan, different fees and many others. As the results, the loan data consists of 113,937 loans and 81 variables for each loan. Any information given regarding personal information can be useful. Such information cna be: occupation, the rating in Prosper, the loan status, income of the borrower and etc. Before the project, I completed 7 lessons that taught me how to write visualization code, properly construct it and modify in order to get a better represantion of the given data. I worked on the Project through Jupyther Notebook, and in addition to learned codes beforehand, I used the website 'https://seaborn.pydata.org/index.html' to help me construct better plots. 

# Univariate Exploration

In this part I have to consider :
- How many variables do I have?
- Do I have missing Data?
- What types of variables do I have? 

After that, I have decided to focus my attention on the Borrower APR (Annual Percentage Rate), while using the variables such as : 
- Loan Status
- Employment Status
- Monthly Income
- Original Loan Amount
- Term 
- Prosper Rating (Alpha)

As the result, I found that: 
-The distribution of borrowers APR looks multimodal. Most of the values are at the range of 0.05 and 0.4. There are no unusual points and no need to perform any transformations

- The distribtuion of monthly income is highly right screwed. Most stated monthly incomes are less than 30k, but some of them are incredibly high, like greater than 100k. Most of borrowers with greater than 100k monthly income only loan less than 5k.

- The very large stated monthly income may be made up. Overall, Less than 0.3 percent borrowers have stated monthly income greater than 30k. These can be seemed as outlier for the following analysis, so it is better to remove borrower records with income greater than 30k.

# Bivariate Exploration 

In this part of the project I am comparing the variable attributes. The point is to find the relationship the numerical and categorical, and compares them either to each other or against each other. 

The variables I looked into in this part are from the Univariate Exploration. Firstly, I looked into the heatmap between 'LoanOriginalAmount', 'BorrowerAPR', 'StatedMonthlyIncome' and 'Term', 'ProsperRating (Alpha)','EmploymentStatus'. This shows the correlation between two variables and if it is possitive or negative. Then I looked into the same objective but through sample and fig plot (sometimes also putting a line for those figures in order to better see and understand the relation between the variables). Second, I constructed a box plot to better see the relationship between categorical and numeric data (by putting the variables against each other, organising the plot to be nicely ordered and colored). Last but not least, I used the countplot to compare the categorical vs categorical variables, to see what the relation is and if the graphs would make any sense. 
 
As a result, I found that: 
- Either there is not enough data for Not Available, Not Employed, Part-Time and Retired because compared to Term and Prosper Ratings, or the information is not impactfull enough.
- When comparing Prosper Ratings (Alpha) and Term we can see that there is a connection, especially since rating B and C have a 60 month loan. Even A and D rating are not far behind on the 60 month loan. On the other hand, AA has the least amount of the three month loan types compared to other ratings, not including HR because it only has a 36 month loan.
- The Borrowers APR is negatively correlated with the Loan Original amount, so more APR causes less loan amount and vise versa. On the other hand, the positive correlation is observed with Borrowers APR and Monthly Income since is also logically possible.
- On the other hand, the correlation is actually possitive between thme. I guess the more money you have, the more money you cna loan. When it comes to the categorical variables, I saw when doing the Box Plot that a better Prosper Rating will have higher Income and Loan Original Data. The pure categorical data was also interesting and I explained my opinion about it in the code above.

# Multivariate Exploration 

This part takes a closer look at the variables in multiple amounts compared to each other. In particular, I am looking into Borrower APR and Loan Original Amount and comparing them to variables Term and Prosper Rating (Alpha). Thus, then the plot is constructed (and in my scenario I have decided to construct Pointplot, FacetGrid and Regplot) which allows me to see three variables at the same time and their relation to each other. This further gives us information how one variable can be 'linked' to the other. It also shows a better visual representation (in my opinion) of the relation between varaibles, as you can clearly spot the negative or positive correlations, or an increase or decrease in general amounts. 

As the result, I found that: 
- Borrowers APR goes down as it climbs on the Prosper Ratings in terms of borrow Terms. However, it suddenly improves from negative relation to positive as the Prosper Rating goes from HR level towards AA. (We can see that sudden change in the transition from Rating B to A)
- A constant positive relation with Prosper Rating and Term. However, the relation gets better as well (borrow term amounts) when the Prosper Ratings goes up from HR to AA, which was similarly seen with Borrowers APR.

# Conclusion 

I am sure if I would have taken into accound other variables like Borrower Rate, Prosper Score, Total Prosper Loans, Loan Origination Data I could have found other interesting correlations and relations between variables. However, I decided to stick to those one as in my opinion they demostrate the variables for the plots quite well.

