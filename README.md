# Donation-fundraising-campaign_analysis_and_revenue-predictions

## Overview:
The goal of this project is to predict the likelihood of individuals making a donation to a charity fundraising campaign "SJ22" and the amount they are likely to give (in €). By combining these two predictions, an expected revenue can be obtained for each individual. The project aims to recommend the charity to solicit an individual if the expected revenue predicted exceeds the cost of solicitation (2.00 €), as it results in a positive profit. On the other hand, if the expected revenue is less than the cost of solicitation, the recommendation would be not to solicit the individual, as it results in a net loss.

The project assumes that individuals will only make a donation to the campaign if directly solicited by the charity, and donations made under automatic deductions following the campaign will not be included in the data. The main objective of the project is to maximize the financial performance of the campaign for the charity.

Data set
On the last day of data available in the database, the charity has solicited 79,469 donors for their SJ22
campaign. Out of these 79,469 solicited donors, about 4,400 have made a subsequent donation. 

These 74,469 solicited donors have been divided into two batches of approximately equal sizes.
For the first batch (N = 39,674), called the “calibration” data, we have complete information about 
their responses to the fundraising campaign. This batch will be used for calibration.

For the second batch (N = 39,795), called the “prediction” data, we only know that they have been 
solicited, but their actual responses are not known. This batch will be used for performance evaluation.
The dataset contains a table assignment2 with following information:
1. contact_id: The list of individuals who have been solicited by the charity for this 
specific fundraising campaign.
2. calibration: 1 if part of the calibration data, 0 if part of the prediction data.
3. donation: 1 if the donor has made a donation, 0 if the donor has not, NULL if the 
information is unknown to you. By design, the value is set to NULL if 
calibration = 0.
4. amount: The actual donation amount observed, in EUR. The value is NULL if the 
donor has not made any donation (donation = 0) or if (calibration = 0).
