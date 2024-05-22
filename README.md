### Capstone: Perfect Store Impact on Energy Drink Sales Volume in Convenience

Author: Mick Gram
Presented: 5/22/2024

* Readme: [https://github.com/mickgram/Capstone/blob/main/README.md
* Notebook: https://github.com/mickgram/Capstone/blob/main/cenergy.ipynb
* Data: https://github.com/mickgram/Capstone/tree/main/Data/energy.csv

#### Disclaimer

* Restricted Use: This data is not publicly available and may not be used for any purpose without explicit written permission from the author. No part of the findings, data, or any derived information may be disclosed, disseminated, or shared without prior written approval from the author.
* Confidentiality: The names of key accounts, store locations, distributors, and relevant periods have been withheld to ensure confidentiality. The data shared herein is proprietary and confidential.
* Contact Information: For permissions or inquiries regarding this data, please contact the author, Mick Gram, via email at mickgram@hotmail.com.

#### Executive Summary

This study demonstrates the potential to predict sales volume using perfect store data points. The findings represent a significant shift from traditional perceptions, quantifying the volume increase for additional chilled cashier coolers and the impact of brand messaging. Successful peer review of this study could transform how FMCG companies invest in perfect store initiatives, leading to more targeted and transparent business cases for investment.


#### Background

Perfect Store is crucial for winning in retail for any FMCG company. In the competitive US market, brands vie for shelf space, cooler placements, cold-cash spots, strike zones, and brand messaging. Despite yearly audits collecting a range of perfect store data points, there has been no proven relationship between these factors and sales drivers. This research uses actual audit and sales data to reassess what factors truly impact sales.

#### Business Questions Asked

- Is there a relationship between perfect store factors and sales volume?
- WWhich perfect store data points have a significant impact on sales? 
- How much does each of these data points impact sales volume?
- 
#### Findings:
- There is a significant relationship between perfect store factors and sales volume. The research produced a model with 86.77% accuracy in explaining which perfect store data points impact sales volume and by how much.
- The impact of data points differs significantly from traditional beliefs.
- The findings justify discussions with leadership about revising the approach to perfect store investments and measurement.

#### Data Sources

* 392 audits:
   - SKU distribution
   - Shelf space
   - Cooler placement
   - POS and brand communication
   - Pricing conditions
   - Competitor data
* Sales data from stores:
   - Packsize distribution
   - Visit Frequency
  
#### Methodology
* Data cleansing and quality control.
* Exploratory Data Analysis to remove multicollinearity, identify impactful data points, reduce variance, and increase accuracy.
* Evaluation of regression models: Linear Regression, Ridge, and Lasso. 
* Ridge and Lasso had alpha optimized using GridSearchRv.
* Model evaluation through train-test split and cross-validation.

#### Next Steps and Recommendations

To implement changes to the current perfect store approach, consider the following steps:

* Peer Review: Obtain feedback from internal data science teams or external vendors.
* Cost-Benefit Analysis: Document costs of perfect store activities and build cost/benefit analyses related to volume.
* Share Results: Present findings to senior leadership, including SVP of Distribution, SVP of Trade Finance, and SVP of Marketing.
* Customer Feedback: Create a focus group to test some of the results.
* Test Market: Propose a test market for the new approach, running it parallel to a control market to monitor changes.
* Evaluate Results: Assess the test market results and, if successful, seek alignment from senior leadership for wider implementation.
  
##### Contributions:
* Facilitator Savio Saldanha provided feedback after completion of part 2, suggesting dimensionality reduction, which significantly increased accuracy and reduced variance. He also recommended adding cross-validation to the train/test split approach.
  
##### Contact and Further Information
For more information, please contact Mick Gram at mick.gram@redbull.com
