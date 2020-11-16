# machine-learning-challenge
machine-learning-challenge

NASA Model / Linear Regression for Score 
The first model aims to predict the koi_score taking into account the koi_disposition, "koi_fpflag_nt", "koi_fpflag_ss", "koi_fpflag_co","koi_fpflag_ec"," and koi_period". 
A value between 0 and 1 that indicates the confidence in the KOI disposition. For CANDIDATEs, a higher value indicates more confidence in its disposition, while for FALSE POSITIVEs, a higher value indicates less confidence in that disposition. 
By inserting the values of pdisposition: Candidate, False Positive or Not Dispositioned and the rest of the variables flags and period, there is a kpi_score which can be used as a benchmark to confirm such assertion. 
The model is assertive with a MSE of 0.0537 and an R2 of 0.9462.


NASA 2 Model / GridFit for Koi_Disposition classification
The NASA 2 Model tries to predict from known variables such as the flags and the period if the subject of interest can be classified as candidate, confirmed or false positive (koi_disposition values).
Running a GridSearch model we were able to get a best fit model with a C=5 and Gamma = 0.001 with an average accuracy of 0.80. The model is highly accurate to predict false positives, yet it has low power for confirmed cases. Future research for a better fit model could include more variables in our dataset such as time, impact, depth, etc. as well as running the grid-fit with further parameters (C, gamma). 
