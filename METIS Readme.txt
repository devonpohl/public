This repository is currently being used to host work produced as part of the Intro to Data Science class with Metis.

NOTE: I'm trying to model the 'newvisits' variable in the data file and understand how the newtrans factor variable affects it. Hotel publish year, location, transmonth, and rating should all be factorized.

Project Review Questions:
(1) What data have you gathered, and how did you gather it?

I have gathered visit counts by hotel on Oyster.com’s German (DE) domain. I have gathered data for a period prior to a translation event and after a translation event (machine to human), as well as data for the same periods in the prior year to help account for seasonality. I’ve also gathered data on hotels that did not receive human translations as well as these hotels’ general performance on Oyster.com/Tripadvisor and descriptive data on the hotels (such as country, when reviews were first published, and rating). I have gathered this through querying and pre-processing data on SQL servers.

(2) How have you explored the data and what insights have you gained as a result?
I have explored the data by looking at summary statistics for various important categorical variables and by looking scatterplots of various continuous variables.
Some findings:
- Translations into DE occurred in batches at various times during the year
- Too few high-quality human translations to give insight into their performance
- Data is noisy and relationships are vary non-linear

(3) Will you be able to answer your question with this data, or do you need to gather more data (or adjust your question)?

I want to confirm that there is a relationship between human-translating a hotel review and incremental SEO traffic, and ideally build a model that is reasonably good at predicting that traffic if it exists. I believe that the data I am collecting will allow me to answer this question but still need to identify the best metric to use as my dependent variable.

(4) What modeling approach are you using to answer your question?

I was going to use an ensemble boosted regression model and then manipulate it and look at summary statistics to confirm that translation quality was indeed an important factor in predicting future SEO traffic.

A DS friend of mine recommended looking into ‘panel models’ for this application. Do you know about these models? If so, can I build such a model with Pandas?
