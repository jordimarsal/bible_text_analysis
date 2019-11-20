# Bible Text Analysis
# NLP + Statistical Analysis Project
# by Jordi Marsal

*Ironhack's Data Part-Time | Barcelona | November 2019*

Bible analysis: scrapping - nltk - LDA - Sentiment analysis - Hypothesis testing

## Content
- [Project Description](#project-description)
- [Hypotheses / Questions](#hypotheses-/-questions)
- [Dataset](#dataset)
- [Cleaning](#cleaning)
- [LDA](#lda)
- [WordCloud](#wordcloud)
- [Analysis](#analysis)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)



## Project Description
* In this project we take a look about two books of Bible. Genesis vs Revelations.



## Hypotheses / Questions
* It is possible found relations between topics in these books?
* It is the sentiment analysis of Genesis more positive than Revelations? 



## Dataset
* This dataset has been obtained from mybible.com, __scrapping__ these two books:
* Genesis & Revelations
* https://my.bible.com/ca/bible/1637/GEN.1.NVI
* https://my.bible.com/ca/bible/1637/REV.1.NVI

It was dumped in two datasets:
```
    1_GEN.csv (213 KB)
    1483 rows x 5 columns
    
    66_REV.csv (64 KB)
    382 rows x 5 columns
```

| Column name | Description | Type |
| :--- | :--- | :--- |
| book | book of Bible | object |
| chapter | chapter of book | int64 |
| verse | verse | int64 |
| text | text of verse | object |
| version | code of version | object |




## Cleaning
* There are not nulls.
* Separate some fails reading from web.
* Saving cleaned datasets.




## LDA
* Calculate LDA for models.
* Visualizing.
* Saving __Interactive Visualizations__.
* https://presentacioih.000webhostapp.com/ldavisREV.html#topic=0&lambda=0.6&term=
* https://presentacioih.000webhostapp.com/ldavisGEN.html#topic=0&lambda=0.6&term=




## WordCloud
* Calculate Bag of Words.
* Visualizing.

<p align="center">
  <img src="https://presentacioih.000webhostapp.com/gen.png" width="350" title="Genesis Word Cloud" alt="Genesis Word Cloud">
  <img src="https://presentacioih.000webhostapp.com/rev.png" width="350" title="Revelations Word Cloud" alt="Revelations Word Cloud">
</p>



## Sentiment Analysis (Polarity)
* Extracting valorations from Spanish XML' senticon_es lexicon.
* Lexicon: http://journal.sepln.org/sepln/ojs/ojs/index.php/pln/article/view/5041
* Imputate polarity to every verse text to new field ___'opinion'___.




## Analysis
* General Info.
* Boxplots and Histograms for fields opinion in every book.
* QQplot (pairplot) for Normality analysis. 
* Calculations for Highlighted Variables:

      Normality.

      Independence over variables. Levene Test.

      p-value (hypothesis test). T-Student.

* Hypothesis Test for Highlighted Variables.



## Conclusion
* Variables are not __Normal (Gaussian)__
* Variables are independent.
* Results are that one book is more positive in their verses than another.
* No one variable hits same mean value. All H0 has been rebuked.



## Future Work
* This data set can be fullfilled with other complementary data. By example can be extendended to other Bible' books.



## Workflow
* Discovering data:

      ploting pairplots, boxplots and histograms.

      info.

      correlation matrix.


* Testing succes-



## Organization
* Git
* Visual Code
* Jupyter Notebooks



## Links

* [Repository](https://github.com/jordimarsal/bible_text_analysis)  
* [LDA](https://en.wikipedia.org/wiki/Latent_Dirichlet_allocation)  
* [Slides.com](https://slides.com/jordimarsal/ih_final#/) 
