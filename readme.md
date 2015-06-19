---
title: "Readme"
output: html_document
---

The run_analysis.R script assumes all data from the UCI HAR dataset is in the same folder under a folder called uci_har_dataset.  

The column names are derived from features.txt.

The actions are taken from activity_labels.txt and mapped onto train/y_train.txt and test/y_test.txt files.

The subjects are taken from test/subject_test.txt and train/subject_train.txt.

The data for the train set is loaded from train/X_train.txt using the column names as above.
The data for the test set is loaded from test/X_test.txt using the column names as above.

The two data sets each have two columns added, using the actions and subjects as described above.

The data sets are then merged.
After merging, the relevant columns subject, activity, plus all of the std and mean columns of the features, are then selected.

Finally, the data is sorted, grouped and summarised to give one reading with the mean for each of the selected features per subject and per activity.
