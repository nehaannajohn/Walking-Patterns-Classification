# Walking-Patterns-Classification
Analysis on walking patterns and classification of users

Objective:
The objective was to determine whether individual walking styles can be used to identify each user and thereby, be used as a biometric marker.

Data:
I utilized mobile sensor driven data on accelerations in the x,y and z axes for mutliple users, collected at a frequency of 33 ms. 

Analysis:
I visualized time series plots of mutliple individuals over a span of time and windowed the data, computing summary parameters such as mean, standard deviation and autocorrelation (since lagged acceleration affects current acceleration). 

In order to identify the user, I built a multi class classification algorithm using random forests and observed feature importance of the key features

Key findings:
1. The time series plots indicated that individual walking styles are in fact unique and thereby, a good candidate as a biometric marker.
2. Feature importance showed that mean acceleration in the x axis is more important than z and y axes, while the actual values of acceleration are highest in y axis, followed by z and x axes. This goes to show that although values maybe lower along the x axis, the variation along the x axis tends to be higher and thereby, a more important feature.
3. The Random forest generated an F1 score of 91% on test data after tuning the number of trees, depth and number of features.

Impact
The analysis above proved that individual walking styles can be used as a biometric marker and therefore, can be used for authentication of users, similar to fingerprint and face recognition. Possible applications include identifying patients in healthcare for treatment (combined with heart rate and temperature parameters) and monitoring contractual labour force in manufacturing plants.
