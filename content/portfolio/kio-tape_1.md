---
title: "UCI Bank Marketing Data Analysis"
date: 2019-12-23T15:44:46+06:00
type: portfolio
image: "images/projects/project-thumb-five.png"
category: ["Classification, Imbalanced, EasyEnsemble"]
project_images: ["images/projects/project-details-image-seven.png", "images/projects/project-details-image-eight.png"]
---

##### GO TO [GITHUB](https://github.com/yejiseoung/BankMarketing)


The main goal of this project is to build a machine learning model that predicts if the client will subscribe to a term deposit (variable y). 

I used bank marketing data which is provided by [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/bank+marketing). It contains 411,888 rows and 20 feature variables, ordered by date (from May 2008 to November 2010).

The data is related with direct marketing campaigns (phone calls) of a Portuguese banking institution. Oftentimes more than one contact to the same client was required in order to assess if the product (bank term deposit) would be 'yes' or 'no' to the subscription.

I used `EasyEnsemble` technique which is an ensemble algorithm that was designed to work with imbalanced datasets. EasyEnsemble showed the best performance compared to under-sampling, over-sampling, and other ensemble methods. 

The final model showed a `0.808 roc-auc score`. 