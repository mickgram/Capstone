### Capstone: Perfect Store Impact on Sales Volume

By Mick Gram:
* Notebook: https://github.com/mickgram/Capstone/tree/main/cap_energy-042624.ipynb
* Data: https://github.com/mickgram/Capstone/tree/main/Data

#### Disclaimer

* Restricted Use: This data is not publicly available and may not be used for any purpose without explicit written permission from the author. No part of the findings, data, or any derived information may be disclosed, disseminated, or shared without prior written approval from the author.
* Confidentiality: The names of key accounts, store locations, distributors, and relevant periods have been withheld to ensure confidentiality. The data shared herein is proprietary and confidential.
* Contact Information: For permissions or inquiries regarding this data, please contact the author via email at mickgram@hotmail.com.

#### Executive summary

Perfect Store is a critical part of winning in Retail for any FMCG company. In the US the stores are very competitive with all brands fighting over shelf space, cooler placements, cold-cash, strike zone, brand messaging etc.

Most large retailers perform yearly audits and collect a range of perfect store data points, but to my knowledge, there has never been proven a true relationship between these and what actually drives sales. It appears to be very subjective what data points that actually has an impact, and not least what the impact is.

This research will use actual data collected from audits as well as sales data to revisit what actually has what impact.

#### Rationale

FMCG companies have limited spend and resources for Perfect Store activities. The ability to make the right decisions can have an actualy impact on sales and hence be the difference between being profitable or caring a loss. Knowing how the cost of each activity can impact sales is critical. E.g does a it pay off to place a $500 cooler, focusing on adding more shelf space or improve brand messaging.

#### Research Question

What perfect store data points has what impact on sales? 

#### Data Sources

* 1047 audits:
   - Voids and Core SKU 
   - Shelf space
   - Cooler placement
   - POS and brand communication
   - Strike zone 
   - Competitor data
* Sales data:
   - Volume
  
Data pulled via a query from our Snowflake data lake. Data points are explained in detail in notebook.

#### Methodology
* EDA
* Linear Regression
* Ridge and Lasso
* RandomForest or others ???
* Hyperparameter tuning and cross-validation of models.
* Should I add overfitting discussion?
* Should I add feature importance?

#### Results

Through rigorous analysis using Linear Regression, Ridge, and Lasso models, our investigation aimed to pinpoint which perfect store elements substantially impact sales volume. Here are the insights drawn from each model:

* Linear Regression** provided a baseline with an MSE of 0.2996 and an R² of 0.5327, and did well in cross validation with Mean R2 of 0.5596 and std R2 of 0.0246
* Ridge, with an optimal alpha of 100, offered a refined view with a slightly improved MSE of 0.2988 and R² of 0.5339, and also did well in cross-validation with same Mean R2 of 0.5596 but tiny bit lower and better std R2 of 0.0265.
* Lasso did well, but didn't offer any additional value, only having alpha of 0.010, with a MSE of 0.2988 and an R² of 0.5339. Cross-validation was not as good though with a way lower Mean R2 of 0.2864 despite having a bit lower std R2 of 0.0632.

Comparing these models, Ridge stood out and is the chosen model. Closely followed by basic linear regression.

These findings suggest a potential shift in resource allocation towards best performance to enhance sales performance effectively. The visibility into the coefficients and their size for different data point, is enough to at least discuss a change in approach for perfect store. 

#### Next steps

Changing the current Perfect Store approach would be ground breaking so I suggest the following:

* Get a peer review from our internal DS Team to validate results, and maybe add improvements.
* Document costs of Perfect Store activities and build cost/benefit analyis related to volume.
* Share results with SVP of Distribution.
* Discuss results with SVP of Trade Finance that manages/allocates POS spend.
* Get input from SVP of Marketing.
* Create a focus group with customers to test some of the results.
* Propose a test market for changed approach, and follow up with new audits and monitor changes in sales. Do it in parallel with another market that continues exising perfect store focus.
* Evaluate results, and if successful, get LT (CEO,CFO,CCO,CMO) alignment on next step for wider implementation.



##### Contact and Further Information
mickgram@hotmail.com
