# Clickstream Prediction

IN PROGRESS:  The [Online Shoppers Purchasing Intention Dataset](https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset) has been used in previous research for training models on clickstream data. The data as is contains no missing values, requiring some EDA and cleaning to run with various models. As I have been reading about the various approaches for optimizing models to predict the likelihood a user will make a  purchase, I will be experimenting with some options. The target variable "Revenue" is binary, indicating whether or not a user made a purchase "True" or did not "False". Previous research has used x2 based feature selection, or mutual infomration (MI), and mRMR filters for feature ranking. I will experiment with some other options, including SHAP feature selection. As the target variable is binary, it is suitable for a range of models including log regression, support vector machines (SVM), neural networks, decision trees, and XGBoost. I think this is a great dataset to consider, given the nuances observed in EDA between user behavior and purchasing likelihood. Though, it does include some rather indirect variables, such as "Page Value", which gives you the approximate value of pages though not of the purchase itself. The same can be said for "Revenue", where the price tag of the purchase is omitted. There is also imbalance in the dataset that needs to be considered. The dataset contains 12,350 rows, 10,442 of which are associated with "False" Revenue and 1,908 with "True". The class imbalance includes another factor to consider when determining EDA, data cleaning and model selection. 


## References

Buisson, F. (2021). Behavioral data analysis with R and Python. O'Reilly Media, Inc.

Khandokar, I. A., Islam, A. M., Islam, S., & Shatabda, S. (2023). A gradient boosting classifier for purchase intention prediction of online shoppers. Heliyon, 9(4)..

Sakar, C. O., Polat, S. O., Katircioglu, M., & Kastro, Y. (2019). Real-time prediction of online shoppers’ purchasing intention using multilayer perceptron and LSTM recurrent neural networks. Neural Computing and Applications, 31(10), 6893-6908.

