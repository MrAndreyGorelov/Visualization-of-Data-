# Visualization-of-Data-

This is the last project of the Udacity Course. It focuses on applying all the codes learned into one, and completeing an analysis in order to interpret the findinds. 

# Introduction

Before the project, I completed 7 lessons that taught me how to write visualization code, properly construct it and modify in order to get a better represantion of the given data. I worked on the Project through Jupyther Notebook, and in addition to learned codes beforehand, I used the website 'https://seaborn.pydata.org/index.html' to help me construct better plots. 

# Main Body 

There are multiple recollections to be made with the given visualization. It breaks down into two parts - Exploratory Data and Explanatory Data. In this project we are working with both of them. 

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

# Bivariate Exploration 

In this part of the project I am comparing the variable attributes. The point is to find the relationship the numerical and categorical, and compares them either to each other or against each other. 

The variables I looked into in this part are from the Univariate Exploration. Firstly, I looked into the heatmap between 'LoanOriginalAmount', 'BorrowerAPR', 'StatedMonthlyIncome' and 'Term', 'ProsperRating (Alpha)','EmploymentStatus'. This shows the correlation between two variables and if it is possitive or negative. Then I looked into the same objective but through sample and fig plot (sometimes also putting a line for those figures in order to better see and understand the relation between the variables). Second, I constructed a box plot to better see the relationship between categorical and numeric data (by putting the variables against each other, organising the plot to be nicely ordered and colored). Last but not least, I used the countplot to compare the categorical vs categorical variables, to see what the relation is and if the graphs would make any sense. 

# Multivariate Exploration 

This part takes a closer look at the variables in multiple amounts compared to each other. In particular, I am looking into Borrower APR and Loan Original Amount and comparing them to variables Term and Prosper Rating (Alpha). Thus, then the plot is constructed (and in my scenario I have decided to construct Pointplot, FacetGrid and Regplot) which allows me to see three variables at the same time and their relation to each other. This further gives us information how one variable can be 'linked' to the other. It also shows a better visual representation (in my opinion) of the relation between varaibles, as you can clearly spot the negative or positive correlations, or an increase or decrease in general amounts. 

# Conclusion 

I am sure if I would have taken into accound other variables like Borrower Rate, Prosper Score, Total Prosper Loans, Loan Origination Data I could have found other interesting correlations and relations between variables. However, I decided to stick to those one as in my opinion they demostrate the variables for the plots quite well.

