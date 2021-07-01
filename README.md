# Overview
The purpose of this analysis was to use several learning models to see if any could successfully predict credit risk. 

# Results
All the results for the different models follow, but since there are six models, and a couple of the statistics are similar, I am going to give a review on the precision results for all the models. 
All the models had the same result for low-risk precision and nearly all had the same result for the high-risk precision. The only difference in the high-risk tests were that four of them had a result of 1% and two of them had a result of 2%. While I am surprised that all the tests had similar results, it makes sense that precision is similar when it comes to determining credit risk. Creditors would be more likely to be more precise on determining low risk compared to high risk. Based on the metrics they collected and used as criteria, it is easy for them to determine who is a low risk per their definition.

•	[Naïve Oversampling](Resources/Naive_Oversampling.png)
Naïve Oversampling had fairly good results with 67% accuracy overall. It also had good results with high and low risk recall at 73% and 60% respectively. 

•	[SMOTE Oversampling](Resources/SMOTE.png)
SMOTE Oversampling also had a fairly good accuracy result with 67%. The results for recall balanced each other out where the high risk recall percentage went down compared to Naïve and the low recall went up. The results for high and low risk recall were 65% and 68% respectively. 

•	[Undersampling](Resources/Undersampling.png)
Undersampling had the worst results out of all tests with 53% accuracy overall and 67% and 39% respectively for high and low risk recall. Taking away data points clearly is not the best choice for this important dataset.

•	[Combo Sampling](Resources/Combo_Accuracy_Report.png)
Combo Sampling was a little mixed bag with results. Its accuracy was on par with the top tests so far at 65%. It also had the highest result for high risk recall of any test at 74%, but it also has the second lowest score of low risk recall at 56%. 

•	[Random Forest](Resources/Random_Forest.png)
Random Forest tied for the top spot on accuracy score at 71%. It did have the lowest score on high risk recall at 58%, but it also had the highest score for low risk recall with 83%. 

•	[Easy Ensemble](Resources/Easy_Ensemble_Accuracy_Report.png)
Easy Ensemble had had incredibly similar results as Random Forest. They tied for the top accuracy spot at 71% and their recall numbers were 1% off on each with high and low risk recall at 59% and 82% respectively. 

# Summary

I think it is important to have a good balance in the scores, but in my opinion, I think overall accuracy and high risk recall are the two most important scores from a business standpoint. You want to be able to better pinpoint who your at risk people are so you know how to protect your finances. A good low risk recall benefits those people who are trying to acquire credit as they have a chance to be properly organized in the low risk category.
With that being said, in my opinion, Naïve Oversampling provides the greatest balance on all of the scores and is my choice of learning model to use. It performs well where it needs to and doesn’t have any glaring holes in its abilities. 

