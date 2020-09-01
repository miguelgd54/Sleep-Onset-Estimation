# Sleep Onset-Estimation: Project at NGoggle Diagnostics

This is a sample data science and machine learning project from the work I do at NGoggle Diagnostics Inc. This project uses data from publicly available databases.
The data used is from Sleep-EDF database.

The data gets processed using python and many associated libraries. Channel and feature selection is done on the electroencephalogram data. Data gets cleaned and processed in 30 second epochs, then it gets passed into a pipeline to extract the frequency bands using a power spectral density function as given by Welch's psd implementation. 
After it passes through the power spectrum feature selection function, it then gets passed into an ExtraTrees classifier that performs grid search and k-fold cross validation
with 10 folds.
