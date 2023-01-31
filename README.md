# ML-Project2-Email-Spam-Detector

Project & Goals

The scope of this project is to classify if an email is a spam or not using ML techniques. A data cleaning, preparation and exploration is conducted before conducting several machine learning methods such as Naïve-Bayes Text Classification, KNN and Random Forest Classifications are used to make classifications. Using parameter optimization techniques, confusion matrixes and classification reports, the most optimal machine learning technique is identified.

Methods

I. Naïve Bayes Classification for Text
For the Naïve Bayes Classification, sklearn’s MultinominalNB module is utilized. Alpha value of 1.5 is used. Appendix 8 shows the Classification Report of the Naïve Bayes. The reported accuracy is 0.986, which is very high. After this analysis is completed and an overall accuracy of 0.99 is achieved, it was decided not to pursue any parameter tuning or optimizations.

II. KNN
In order to use the best model for KNN, first the distance metric (Euclidean or Manhattan) must be chosen, in addition to the right value of K (the number of neighbors to classify the text object). To achieve this, two separate Error Rate vs K value plots are plotted.
Using these plot and error rates, the best distance method and K are chosen to further the analysis. Using K value of 2 and a distance metric of Euclidean, best KNN model is constructed, trained, and tested. The confusion matrix shows that the accuracy is 0.950. This proves that the model was a success.

III. Random Forest
Before constructing the random forest model, it was decided to choose the best parameters to tune the model. To achieve that the criterion and number of estimators were used to create different models and test their accuracies to optimize the parameters that will create a higher accuracy model. For the number of estimators parameter: 100, 200 and 500 values; for the criterion parameter: Gini and Entropy indexes were used. Code segment for parameter optimization can be found in Appendix 20.
As a result of this optimization experiment, the best optimization parameters for the random forest model are determined, as n_estimators: 200 and criterion: Gini.
Using the optimized parameters, a Random Forest model is constructed, trained, and tested. Appendix 15 shows the Random Forest Classification Report. The reported accuracy is 0.994.

Conclusion

In conclusion, Random Forest algorithm is found to be the most accurate technique to be used for text classification purpose of the project. The accuracy reported by the Random Forest technique is 0.994. The high accuracy can be linked to the methodology of the Random Forest algorithm. Since it combines different decision tree results to result the best classification, it is proven to be very effective in classifying text.
