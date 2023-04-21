# Group-5-Project
Please  note the code for the project used:
   - Health_analysis-Final.ipynb
   - Alz_Mortality.ipynb
   - API_Attempt.ipynb is an attempt to use APIs in the future 

This is a project focused on Alzheimer’s disease and related dementias. The primary goal of the study is to identify trends and patterns in the prevalence and incidence of these conditions, as well as to explore potential risk factors and interventions that may help to prevent or mitigate their impact in the U.S.

The project aims to answer several research questions, including whether physical activity prevents Alzheimer’s disease, whether age affects Alzheimer’s severity, whether gender has an effect on the prevalence of Alzheimer’s disease, whether there is significant variance in Alzheimer’s mortality between US regions, and what is the percentage increase in every US state between 2015-2020. Additionally, the project suggests further exploration into the the correlation between physical activity (sport complexes) and AD per state and whether a healthy diet (number of fast-food restaurants in a state) affects AD.

To address these research questions, several datasets were used, including the Alzheimer’s and Aging data CSV, the Alzheimer’s mortality dataset, Census.gov state regions as CSV, and total population per state. The datasets were compiled by the Centers for Disease Control and Prevention (CDC) and include data from several national surveys, including the Behavioral Risk Factor Surveillance System (BRFSS), the National Health and Nutrition Examination Survey (NHANES), and the National Health Interview Survey (NHIS).

One of the challenges faced during the data mining process was that the data related to the hypothesis was hidden under two values in a column. The data frame was filtered by those two question-values, and then two more columns were created from the existing one. These columns were derived from the column called “Data_Value,” and their names were based on the unique values of the filtered column called “Question.” The columns were renamed as “Poor Health” and “Inactive Days,” and they were used to answer one of the questions related to the hypothesis. A scatter plot of “Less Active - Poor Health” showed that when the number of inactive days increased, the percentage of people with Alzheimer’s disease who had poor health also increased. The correlation coefficient was 0.75, which means that there is a strong correlation between inactive days and poor health. The probability (P-value) value was less than 0.05, which provided strong evidence against the null hypothesis.

For the age group testing, a filter was applied to the data set to select individuals aged 50-64 and 65+. As there were two variables with continuous values (Poor Health and Age Group) and Age Group is categorical (50-64 and 65+), t-testing and box plotting were used. The t-test found a significant result in an independent samples t-test, suggesting that there is evidence to support a statistically significant difference between the means of the two groups being compared.

The project also studied the dependence between Age Group and States. As both variables were categorical, a chi-square test was used. To prepare the data for the chi test, a cross-tabulation table of two or more factors was created. It took one or more arrays or Series objects as inputs and produced a table that showed the frequency distribution of the variables. The p-value told us the probability of observing a test statistic as extreme as the one we observed, assuming that the null hypothesis was true. If the p-value was less than the significance level (e.g., 0.05), we rejected the null hypothesis and concluded that there was a significant association between the two categorical variables.

The alzheimers mortality ETL involved cleaning and merging data from two CSV files on state regions and Alzheimer's disease mortalities across five years by state. Rows were dropped and renamed, and merging was successful on the state column using inner join. Aggregate mean mortality rates were taken while grouping within region and then year. Hypothesis The hypothesis tested was that the mortality rates of Alzheimer's disease in the United States are region-dependent. Regional differences in Alzheimer's disease mortality refer to the variations in the number of Alzheimer's disease deaths across different regions in the United States, specifically in this presentation looking at Midwest, Northeast, South, and West. There is strong evidence to support the alternative hypothesis that Alzheimer's disease mortality rates are region-dependent in the United States. We summarized the data of the regional mortality rate averages over the course of 2015 to 2020 into a box and whisker plot Results from the Anova Test: P-Value = 3.75e-12, <.05, supporting the alternative hypothesis Possible explanations for regional differences include differences in lifestyle factors such as diet and exercise, as well as variations in environmental factors such as air pollution or access to healthcare. Implications As the alternative hypothesis suggests, there may be important implications for understanding the underlying causes of Alzheimer's disease and developing effective prevention and treatment strategies. This could lead to further research into the specific factors that contribute to the regional differences in Alzheimer's disease mortality rates in the United States. API Slide To further investigate the specific factors contributing to regional differences, the use of the Geo API to collect data about gyms and fast food across these regions was proposed. Due to API limitations, the approach would require splitting up cities in calls, scaling that out to states, and then eventually regions, to encompassing the entire US. If explored in the future, the approach would start with very small radii rather than state-sized radii to avoid hitting the 500 feature limit. 

In conclusion, the project focused on Alzheimer's disease and related dementias with the primary goal of identifying trends and patterns in the prevalence and incidence of these conditions. The project explored potential risk factors and interventions that may help to prevent or mitigate their impact in the US. To address research questions related to the project, several datasets were used, including the Alzheimer's and Aging data CSV, the Alzheimer's mortality dataset, Census.gov state regions as CSV, and total population per state. One of the challenges faced during the data mining process was that the data related to the hypothesis was hidden under two values in a column.

The project used different statistical methods, such as scatter plots, t-tests, and chi-square tests, to analyze the data and answer research questions. The results of the statistical tests suggested that there is strong evidence to support the alternative hypothesis that Alzheimer's disease mortality rates are region-dependent in the United States. Possible explanations for regional differences include differences in lifestyle factors such as diet and exercise, as well as variations in environmental factors such as air pollution or access to healthcare.

Overall, the project's findings have important implications for understanding the underlying causes of Alzheimer's disease and developing effective prevention and treatment strategies. Further research into the specific factors that contribute to the regional differences in Alzheimer's disease mortality rates in the United States could provide valuable insights for future interventions. The proposed use of the Geo API to collect data about gyms and fast food across these regions could also provide further information about the specific factors contributing to regional differences.




