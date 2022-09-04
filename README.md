# Predicting Stock Index Using GDELT v2 Events Daily Average Tone

Big Data and Cloud Computing Course Submission

See full report [HERE](https://github.com/mbdelaresma/stock-index-using-daily-tone/blob/main/FinalReport.ipynb)

# Executive Summary

News headlines serve as flagships for the events that dictate the rise and crash of equity as the stock market is held under the pervasive influence of media. This begs the question of: how we can use the availability of news information to methodically quantify the effect of media on a company’s stock price? Using data freely available from the GDELT project and Yahoo Finance, this study leveraged Amazon Web Services as a platform for Pyspark which the authors utilized to combine company stock price information and an aggregated media tone from several reports coming from different news sources. The Closing Price for several companies was then modelled using the Merlion Time Series DefaultForecaster using an 80% Train and 20% Test split. Tesla Stock produced a MAE of 2.47 when the cumulative sum of the daily media tone from different sources is included as feature and forecasted using the last value of a 3-Day Sliding Prediction Window. When back testing is utilized with the model’s prediction, the study produces a return of -9.64 compared to -61.67 when using moving averages, showing definite improvement. To further refine the results coming from this study, the authors suggest the following: keyword choice augmentation when scraping web articles from the GDELT project, a granular incorporation of long and short range data coming also coming from GDELT, pre-processing steps and hyperparameter tuning for the Time Series models utilized, and finally, company profiling to refine the selection criteria of entities suited for this methodology.

# Contributors

dela Resma, Marvee

La Rosa, Patrick

Pingol, Miguel

Soriano, Chris
