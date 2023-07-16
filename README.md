# Lending Club Case Study
With this case study, we are trying to solve a real business problem using EDA. 
The given data contains the information about past loan applicants and whether they defaulted or not. 
In this case study, we are using EDA to understand how consumer attributes and loan attributes(by looking at applicant's profile) influence the tendency of default.


## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Contact](#contact)


## General Information
# Case study aim: 
The Landing Club company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment.
 
- Background: 
Lending club: An online loan marketplace facilitating personal loans, business loans, and financing of medical procedures. 

Two types of decisions that could be taken by the company during processing a new loan application:

- Loan accepted: If the company approves the loan, there are 3 possible scenarios described below 
Fully paid: Applicant has fully paid the loan (the principal and the interest rate)
Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.
Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan

- Loan Rejected: If the company does not approve the loan.Based on the right decision taken i.e. whether to accept or reject the loan application, company makes profit.
   Based on the right decision taken i.e. whether to accept or reject the loan application, company makes profit.

- Business Problem:
Lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). The credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. The company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment.

- Dataset: 
Loan Dataset having the following important columns to analyze.

1. loan_amt : loan amount requested by the borrower
2. funded_amnt : The total amount committed to that loan at that point in time by the Lending Club.
3. funded_amnt_inv : The total amount committed by investors for that loan at that point in time.
4. term : term of the loan
5. int_rate : interest rate of the loan
6. grade : grade of loan from A-G in increasing level of risk
7. sub-grade: sub-grade of grades from 1-5 in increasing level of risk
8. emp_length : Employment length in years
9. home_ownership : The home ownership status provided by the borrower during registration
10. annual_inc:The self-reported annual income provided by the borrower during registration.
11. issue_d : The month which the loan was funded
12. loan_status: Current status of the loan. The possible values are Fully Paid & Charged off.
13. purpose : A category provided by the borrower for the loan request.
14. addr_state : The state provided by the borrower in the loan application
15. dti: A ratio calculated using the borrower’s total monthly debt payments on the total debt obligations, excluding mortgage and the requested Lending Club loan, divided by the borrower’s self-reported monthly income.


## Conclusions
Profile of defaulted applicants typically contain following indicators:

- Home ownership
1. Applicants lives on rent or are paying mortgage.
2. Applicants tend to be accept interest rates around 14%.
3. Applicants living on rent and with interest rate above 25% most likely always defaults.

- Grade & sub-grade
- Very rich applicant will most likey default with grade G at an interest rate of 20%.
- Rich applicants tend to apply & default with grades F & G for large number of loan applications.
- High-Very High sanctioned loans from investors have the highest interest rates.
- Median amount sanctioned loans are assigned grades B,C & D and are higher in applications and which have the highest defaults resulting in the maximum credit loss for the company.
- Very poor & Poor* income groups have the highest number of median santioned loan amounts with grades B(sub-grades B3,B4,B5(highest)), C(sub-grades C1,C2,C3) & D(D2,D3). They also tend to default lesser on riskier grades because of lower interest rates.
- Loan sub-grade A1 has the least number of defaulted applicants which is also the least for Very high, Poor and Very poor income groups.

# Term
- Very Poor & Poor income groups have loan term of 36 months.
- Rich & Very Rich income groups have loan term of 60 months.
- Defaults happen at an interest rate of 13% for loan term of 36 months while it is 16% for 60 months.
- Loan term of 60 months have higher interest rates.

# Purpose
- Debt consolidation has the highest defaults with interest rate at 15% in the year 2011 & month December which may be due to after-effects of The Great Recession. This is an event that may repeat during any global event that affects a USA economic cycle.
- Debt consolidation defaults is high for Very Rich & Rich applicants & lowest for Very Poor applicants.
- Very rich applicants tend to default more with credit card loans with an interest rate between 14.5%-15%.
- Very Poor applicants tend to default more with home improvement with higher interest rates of around 14% and least with credit card with interest rates of around 13%.

# Interest rate
- The higher the interest rate, the higher likelihood that applicant defaults.
- The higher the loan sanctioned by the investor, higher is the interest rate.
- The median of interest rate is in the range of 10%-15% for all income groups.
- Very Low & Low sanctioned loan amounts have very high interest rates.
- Higher the DTI, higher is the interest rate.
- Very few applicants had applied for loan with very high rate of interest and the proportion of charged off's is maximum. > > 5.7 For very low and low rate of interest, proportion of charged off's is lesser.

# Employment Length
- Between 2-9 years, with increase in employment length, applicants tend to default less.
With employment length more than or equal to 10 years, there is more likelihood that the applicant defaults.
- Debt consolidation is the major contributer for defaults across all employment lengths.
Annual income increases with increase in employment length.

# States
- CA has maximum number of defaults among all US states followed by NY, FL and TX.


## Technologies Used
- Python 3.10.9
- Jupyter Notebook Server 6.5.2

## Contact
Created by [@shagunp and @andrea-naz7] - feel free to contact us!
