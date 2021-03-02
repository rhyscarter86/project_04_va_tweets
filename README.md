# project_04

# Understanding Activity in Department of Veterans Affairs Twitter Accounts

This effort looks at roughly 50,000 tweets to three Department of Veterans Affairs (VA) accounts, including one for the department as a whole, one for the Veterans Benefits Administration (VBA), and one for the Veterans Health Administration (VHA).

## Description and Data Used

Data from Twitter was collected via the Twint package, going back for a 6 month period, roughly August 2020 through January 2021. Data from each of the three accounts was combined into one master data file, and different masking was used to focus on specific topics of interest, namely Coronavirus activity, Mental Health Risk, and Suicide Prevention related tweets. This amount of data was chosen due to it being sufficiently large enough and covering enough time, without presenting too challenging an initial set of data to work with to achieve a minimally viable product.

## Overall Outcome

*Ultimately a final review of data collected for the period shows a slight increase in activity as Coronavirus Vaccine rollout begins. Mental Health and Suicide Related activity remained steady, albeit for one bump in late November where news reporting highlighted VA efforts around suicide prevention.*

## Features & Techniques Used

* Data was vectorized via Countvectorizer, then Non-negative Matrix Factorization (NMF) with triplet-grams was used to create features for all ~50k tweets

## Tools & Techniques Used

#### *For Data Collection and EDA:*
* Twint Package
* Python Jupyter Notebook
* Pandas and Numpy
* Tableau

#### *For Matrix Factorization and Topic Modeling*
* Scikit-Learn NMF
* TF-IDF
* Countvectorizer

## Workbooks
* File0 - Data Acquisition: Data collection via Twint and initial file pickling for downstream use.
* File1 - Data Cleaning: Pre-processing of tweets, including removing special characters, combining named entities, and removing duplicates.
* File2 - EDA and Prelim Visualizations: Initial EDA, particularly around dates and corresponding visualizations of time series for VA tweets.
* File3 - Vectorization and Topic Modeling: Vectorization and Topic Modeling, with appendix containing other versions of both that were tested prior to settling on final.
* File4 - Reference Scratch Notebook: Draft workbook for reference.

## Analysis Limitations

* **Limited timeframe to ensure speed and limit complexity given time constraints** 6 months of data vs. a whole year was a deliberate decision to try and reduce complexity and ensure completion of efforts. However, doing so did limit the conclusions able to be drawn. An expansion of this analysis is planned to ensure year over year comparisons are possible.

## Possible Impacts & Future Efforts

There are clear implications for gaining a better understanding of the Veteran community's needs and current concerns. While VA may have its messaging, this may or may not align with what Veterans themselves are most concerned with. This effort seeks to bridge that gap. Additionally, gaining an understanding of who the Veterans are currently using Twitter, as well as who may be influential, presents additional opportunities for more targeted Veteran outreach and effective communications.  

#### *Future Efforts:*
Expand the use of not just Twitter data, but other hubs of Veteran communications, including message boards, Reddit threads, and others.
