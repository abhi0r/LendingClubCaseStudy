
# Lending Club Case Study

This repository contains a case study on loan data analysis. 
The case study includes exploratory data analysis (EDA) and visualizations to understand the relationships between various loan attributes and the loan status. 
Basic understanding of risk analytics in banking and financial services and to understand how data is used to minimise the risk of losing money while lending to customers.

## Table of Contents

* General Information
* Technologies Used
* Analysis
* Visualizations 
* Conclusions
* Acknowledgements


## General Information

# Background

We assume we work for a consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:

a. If the applicant is likely to pay the loan, not approving such loan will result in loss for the company 
b. If the applicant is likely to default the loan, approving such loan application will also result in loss.

The source data loan.csv contains the information about past loan applicants and whether they ‘defaulted’ or not. We need to perform EDA to understand how consumer attributes and loan attributes infulence the decisioning. In other words, the company wants to understand the driving factors behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.

In this case study, we will use EDA to understand how consumer attributes and loan attributes influence the tendency of default.

When a person applies for a loan, there are two types of decisions that could be taken by the company:

1.Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:
    Fully paid: Applicant has fully paid the loan (the principal and the interest rate).
    Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.
    Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan
2.Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)

# Business Problem

This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface.

Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). The credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.

If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.

## Technologies Used

Python Libraries:
1.pandas
2.numpy
3.seaborn
4.matplotlib.pyplot
5.warnings

## Analysis

The analysis covers the following aspects:
1.Understanding of the given Data
2.Data Preparation(Cleaning, Standardisation, treating outliers)
3.Data Analysis



## Visualizations

The visualizations include count plots, box plots, bar plots, heatmap, scatter plot and more to illustrate the relationships between different loan attributes.

## Conclusion

The analysis provides insights into the factors that may influence the loan status, such as 

1. Loans with higher loan amounts are more prone to default (Charged Off), so all such loans should be scrutinized more than other loans.
   Verification process for such loans should be made more stringent.
   And if possible break that loan into multiple parts which would be passed after retreiving principal of previous part.
   Or it should be passed with higher collateral.
2. All of the following are indicators of possible higher loan amounts - 60 months term, Grades G(E & F), 'Small_Business' as Purpose, Home_Ownership = 'OTHER'.
3. Verification process should be improved because for verified loans the average loan amounts is high, the average interest rates are high and are more prone to being Charged  Off as compared to other types of verification_status.
4. Higher interest rates are more prone to being Charged off, So increasing interest rates should be done only when it is absolutely necessary for business and that loan should be very thoroughly verified.
5. Interest rates increases as the number of installments increases, so loans with higher number installments should be more scruitinized before allowing them and customer should be tried to be convinced to avail a loan with low number of installments to avail low interest rates.


## Acknowledgements
Reference Material
1. UpGrad Material, Live session and recordings
2. Seaborn Libraries 
    https://seaborn.pydata.org/tutorial/categorical.html
    https://seaborn.pydata.org/tutorial/distributions.html
3.Lending Club website
    https://www.lendingclub.com/personal-loan/rates-fees
    https://www.lendingclub.com/resource-center


## Contact
Created by:
1. Abhishek Raghuvanshi
2. Subhrabindu Khuntia





