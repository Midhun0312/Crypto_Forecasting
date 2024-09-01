Overview of my model
The characteristics of my model are as follows

Only 'Close' is used.
The model is trained for each coin using a common set of features for all the coins.
The difference between the change of each currency and the change of all currencies is provided as features.
Single model of LightGBM (7-fold CV)
Considering the definition of the forecasting target in this competition, I felt it was necessary to prepare features with information about the entire market. I also thought that some currencies might be affected by the movements of other currencies, so I made it possible to refer to information about other currencies as well. Since I thought that memory and inference time would become more demanding with this kind of processing, I reduced the amount of data to be used. Specifically, I considered 'Close', which is used to calculate the target, to be the most important, so I decided to use only it. Even so, the ensemble could not be performed because of the limited inference time (and lack of coding skill).
