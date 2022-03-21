---
title: "Starbucks Offer Recommendation"
date: 2019-12-23T15:58:10+06:00
type: portfolio
image: "images/projects/project-thumb-one.png"
category: ["Recommendation Engine"]
project_images: ["images/projects/project-details-image-three.png", "images/projects/project-details-image-four.png"]
---

##### GO TO [GITHUB](https://github.com/yejiseoung/Starbucks)


The main goal of the project was to `build a recommendation model` that could guide customers to an appropriate offer. 

The dataset contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink (informational offer) or an actual offer such as a discount or BOGO (buy one get one free). 

Since not all users received the same offer and not all users responded to the offers in the same way, this posed a challenge to solve with the data set. 


To build a recommendation model, I computed purchasing behavior scores (PB scores). Since every offer has a validity period, not all users buy products before the offer expires. Given PB scores, I can see the purchasing path from receiving offers to purchasing products.


Based on PB scores, I made a customers-offers pair matrix which has a lot of NaN values, so I used `FunkSVD` algorithm to build the recommendation model. 
