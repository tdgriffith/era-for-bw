# era-for-bw
Looking into extraction of modes for QP theory analysis of EEG data. Primarily using the [DEAP data base](https://www.eecs.qmul.ac.uk/mmv/datasets/deap/) right now. 

Primarily exploratory, so I'm not using cookie cutter right now, but will almost surely regret it later. 

## GAF for EEG data
We generally know more about ANN's and image analysis, so is it possible to extract estimators of interest from time series data transformed into images? I considered [recurrence plots](https://en.wikipedia.org/wiki/Recurrence_plot), but found they take a huge amount of RAM if the time series to too long.

[Gramian Angular Fields](https://en.wikipedia.org/wiki/Recurrence_plot) are kinder to compute resources, so trying that here. So far, generally finding the problem to be ill posed. Network is predicting the mean to minimize the loss function. I'm making a mistake somewhere.