# ICU Delirium Screening: Milestone Two

Notebooks and data for Milestone Two of my Boston University MS in Data Science capstone (Module C). The project is an early warning model for ICU delirium. This milestone covers K nearest neighbors, gradient boosting, K means with silhouette scores, and DBSCAN with hierarchical clustering, all run on two datasets and compared with repeated cross validation.

## Datasets
- MIMIC IV Clinical Database Demo (100 patients, 140 ICU stays): predicts a positive CAM-ICU delirium screen. The feature table is delirium_features.csv, built in the Week 8 notebook from the raw demo tables.
- ECAMS (373 patients, 1189 EEG features): predicts a delirium call from the Confusion Assessment Method. Data from the Brain Data Science Platform (MIT license, see ecams/LICENSE), in the ecams folder.

## Notebooks
- Week8_KNN: k nearest neighbors, distance metrics, scaling
- Week9_GradientBoost: learning rate, rounds, tree depth, regularization, early stopping
- Week10_KMeans: elbow method, silhouette score, scaling, distance metrics
- Week11_DBSCAN_HAC: DBSCAN, linkage methods, dendrograms

The pdf folder has a PDF copy of each notebook and the Milestone Two paper. The figs folder has the figures and result tables the notebooks write.

## Running it
Install pandas, numpy, scikit-learn, scipy, matplotlib, and seaborn, keep the csv files in the same folder structure as shown here, and run the cells in order. Week 8 rebuilds delirium_features.csv from the MIMIC IV demo, which is not included here. Download it from PhysioNet (https://doi.org/10.13026/07hj-2a80) and unzip it next to the notebooks, or skip that cell and use the included delirium_features.csv. Weeks 9 to 11 only need delirium_features.csv and the ecams folder.
