### Capstone: Perfect Store Impact on Sales

**Mick Gram**

#### Disclamer
- Periods are not shared to maintain confidentiality.
- The location of the stores, names of key accounts, distributors etc are not shared to maintain confidentiality. 

#### Executive summary

Perfect Store is a critical part of winning in Retail for any FMCG company. In the US the stores are very competitive with all brands fighting over shelf space, cooler placements, cold-cash, strike zone, brand messaging etc.

Most large retailers perform yearly audits and collect a range of perfect store data points, but to my knowledge, there has never been proven a true relationship between these and what actually drives sales. It appears to be very subjective what data points that actually has an impact, and not least what the impact is.

This research will use actual data collected from audits as well as sales data to revisit what actually has what impact.

#### Rationale

FMCG companies have limited spend and resources for Perfect Store activities. The ability to make the right decisions can have an actualy impact on sales and hence be the difference between being profitable or caring a loss. Knowing how the cost of each activity can impact sales is critical. E.g does a it pay off to place a $500 cooler, focusing on adding more shelf space or improve brand messaging.

#### Research Question

What perfect store data points has what impact on sales? Where should we invest more, and where should we invest less according to what has an impact on sales.

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
   - Service Frequency 

Data pulled via a query from our Snowflake data lake. Data points are explained in detail in notebook.

#### Methodology
* EDA
* Linear Regression
* Ridge and Lasso
* RandomForest ???
* Hyperparameter tuning and cross-validation of models.

#### Results

Through rigorous analysis using Linear Regression, Ridge, and Lasso models, our investigation aimed to pinpoint which perfect store elements substantially impact sales volume. Here are the insights drawn from each model:

* Linear Regression** provided a baseline with an MSE of 0.2771 and an R² of 0.5677, and did well in cross validation with Mean R2 of 0.5775 and std R2 of 0.0422
* Ridge, with an optimal alpha of 100, offered a refined view with an improved MSE of 0.2739 and an R² of 0.5728, and also did best in cross-validation with a slight higher Mean R2 of 0.5887 and also tiny bit lower and better std R2 of 0.0410.
* Lasso performed the really well, only having alpha of 0.010, with a MSE of 0.2739 and an R² of 0.5728. Cross-validation was not as good though with a way lower mean R2 of 0.1596 despite having a bit lower std R2.
* Scaling didn't work well generally, and only hot-encoding was used.

Comparing these models, Ridge stood out and is the chosen model.

These findings suggest a potential shift in resource allocation towards [specific strategies] to enhance sales performance effectively. Further details and implications of these results are discussed below.

#### Next steps

Changing the current Perfect Store approach would be ground breaking so I suggest the following:

* Get a pier-review from our internal DS Team to validate results, and maybe add improvements.
* Share results with SVP of Distribution.
* Discuss results with SVP of Trade Finance that manages/allocates POS spend.
* Get input from SVP of Marketing.
* Create a focus group with customers to test some of the results.
* Propose a test market for changed approach, and follow up with new audits and monitor changes in sales. Do it in parallel with another market that continues exising perfect store focus.
* Evaluate results, and if successful, get LT (CEO,CFO,CCO,CMO) alignment on next step for wider implementation.

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information
mickgram@hotmail.com
