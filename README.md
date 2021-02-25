## README
#### Authored by users @mhubelbank, @conDavis, and @odaily.

This is a clone of the repository for the final DS3000 project of Constance Davis, Eoin Daly, and Mara Hubelbank at Northeastern University. For this project, we set out to perform a wholistic analsis of the speech data of United States presidents; the scope of this project includes data webscraping, preprocessing, linguistic/numerical analysis, hypothesis testing, visualization, and building/testing/tuning a ML model. 

Extracting from an online corpora, we identify such features as the term frequency and Tfidf importance of various social issues, as well as the overall speech linguistic complexity via applying the Flesch-Kincaid readability tests. We also extract the outcome variables of political party, speaker, and time period for each presidential speech.

After visualizing our dataset via scatterplots, pie graphs, line graphs, and word clouds, we identify several hypotheses and questions regarding our dataset. We test our hypotheses (each of which predict a correlation between a social issue feature and an outcome variable) via Pearson correlation and one-way ANOVA, and find that all of our hypotheses are supported. 

We initially construct a value-based ML model based on the DVs and IVs defined above, feeding our models strictly the numeric features extracted from the speech data. After rather disappointing results, we pivot to the construction of a linguistic ML model based on the raw textual speech data, finding the greatest accuracy using the kNN algorithm. We then hypertuned the min-df, n-grams, and stop word-usage parameters of our TfidfVectorizer. Using our model, we were able to successfully predict (>75%) the political party and time period of a given speech, and had moderate success (>60%) with predicting the speaker's identity. 

The final report is presented in as a markdown-documented Jupyter Notebook [here](https://github.com/mhubelbank/ml-presidential-speeches/blob/main/final%20report/final_report.ipynb). You can also view our brief presentation of the project [here](https://youtu.be/xX_li6Z6fUU).
