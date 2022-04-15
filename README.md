# MODEL 16 CHALLENGE: Amazon_Vine_Analysis

## Deliverable 1

### Purpose
The purpose of deliverable 1 was to access the web data provided by Amazon reviews and host a server in Amazon Web Services, which can then be accessed via Postgres.  Below area figures of the accessed data, parsed into 4 tables, and queried in Postgres.

### Figure 1: Customers Table
![Figure 1](/Resources/CustomersTable.png)

### Figure 2: Products Table
![Figure 2](/Resources/ProductsTable.png)

### Figure 3: Review Table
![Figure 3](/Resources/ReviewIDTable.png)

### Figure 4: 
![ Figure 4](/Resources/VineTable.png)


## Deliverable 2

### Purpose
The purpose of deliverable 2 was to access customer reviews posted to Amazon for a particular category of product, in my case outdoor gear, and provide an analysis of potential bias in ratings between paid Vine reviewers and unpaid reviewers. For this analysis, a subset of all products with 20 or more total votes and at least 50% of the reviews were considered helpful. Reviews were separated by paid Vine reviewers and unpaid reviewers. For each group of reviewers, the total number of reviews, total number of 5-star reviews, and the percentage of 5-star reviews were calculated.  To determine potential bias between paid and unpaid reviews, a chi-square test of the percentage of 5-star reviews was performed, with a null hypothesis that the percentage of 5-star reviews was the same between both groups of reviewers.

### Results

Figures 5 and 6 report the results of the paid reviews and unpaid reviews respectively.

### Figure 5
![Figure 5 - Paid](/Resources/D2%20Paid.png)

### Figure 6
![Figure 6 - unpaid](/Resources/D2%20Unpaid.png)

For paid Vine reviews, 55 (53.4%) of 103 total reviews were 5-star reviews. For unpaid non-Vine reviews, 19723 (52.8%) of 37372 total reviews were 5-star reviews. Percentage of reviews between groups were not statistically different from one another (53.4% vs 52.8%, P=0.90)

### Figure 7: Chi-square comparison of paid vs unpaid reviews

![Figure 7 - chi sq](/Resources/Deliverable%202%20Chi.png)

### Conclusion
Based on the statistical comparison of paid vs unpaid reviews of outdoor equipment, there does not appear to be a meaningful bias in the number of 5-star reviews.

### Additional analyses
In addition to the proportion of 5-star reviews, and additional analysis to compare the full distribution of ratings between the two groups using a Wilcoxon rank sum test would provide further information on whether a positivity bias exists or not. 