---
papersize: a4
documentclass: scrartcl
classoption: DIV=14
colorlinks: true
---

![LSE](images/lse-logo.jpg)
# MY459 Special Topics in Quantitative Analysis: Quantitative Text Analysis

### Lent Term 2018

### Instructors

* [Kenneth Benoit](mailto:k.r.benoit@lse.ac.uk), Department of Methodology.  *Office hours*: Mondays 16-17:00, Thursdays 11-12:00, COL.8.11
* [Pablo Barberà](mailto:P.Barbera@lse.ac.uk), Department of Methodology.  *Office hours*: TBA

### Teaching Assistant
* [Christian Müller](mailto:C.Mueller@lse.ac.uk), Department of Methodology.  *Office hours*: TBA

### Course Information

* Lectures on Mondays 12:00–14:00 in 32.LG.03
* Classes on:
    - Tuesdays 9:00-11:00 TW2.4.02, Weeks 2, 4, 7, 9, 11
    - Wednesdays 9:00-11:00 TW2.4.03, Weeks 2, 4, 7, 9, 11

No lectures or classes will take place during School Reading Week 6.

| **Week** | **Topic**                            | **Week** | **Topic**      |
|:----------:|:--------------------------------------|:----:|:----|
| 1        | [Overview and Fundamentals](#week-1-introduction-to-data)       | 7        | [Exploratory data analysis](#week-7-exploratory-data-analysis)          |
| 2        | [Descriptive methods for text analysis](#week-2-descriptive-statistical-methods-for-text-analysis)                  | 8        | [Exploratory data analysis (cont'd)](#week-8-exploratory-data-analysis-contd) |
| 3        | [Methods for comparing texts](#week-3--quantitative-methods-for-comparing-texts)    | 9        | [Model evaluation](#week-9-model-evaluation)                   |
| 4        | [Using data from the Internet](#week-4-using-data-from-the-internet)       | 10       | [Dimensionality reduction](#week-10-dimensionality-reduction)           |
| 5        | [Working with APIs](#week-5-working-with-apis)                  |  11       | [Graph data visualization](#week11-graph-data-visualization)           |
| 6        | _Reading Week_                       |



### Course Description

The course surveys methods for systematically extracting quantitative
information from political text for social scientific purposes, starting
with classical content analysis and dictionary-based methods, to
classification methods, and state-of-the-art scaling methods and topic
models for estimating quantities from text using statistical techniques.
The course lays a theoretical foundation for text analysis but mainly
takes a very practical and applied approach, so that students learn how
to apply these methods in actual research. The common focus across all
methods is that they can be reduced to a three-step process: first,
identifying texts and units of texts for analysis; second, extracting
from the texts quantitatively measured features---such as coded content
categories, word counts, word types, dictionary counts, or parts of
speech---and converting these into a quantitative matrix; and third,
using quantitative or statistical methods to analyse this matrix in
order to generate inferences about the texts or their authors. The
course systematically covers these methods in a logical progression,
with a practical, hands-on approach where each technique will be applied
using appropriate software to real texts.

### Objectives

The course is also designed to cover many fundamental issues in
quantitative text analysis such as inter-coder agreement, reliability,
validation, accuracy, and precision. It focuses on methods of converting
texts into quantitative matrixes of features, and then analysing those
features using statistical methods. The course briefly covers the
qualitative technique of human coding and annotation but only for the
purposes of creating a validation set for automated approaches. These
automated approaches include dictionary construction and application,
classification and machine learning, scaling models, and topic models.
For each topic, we will systematically cover published applications and
examples of these methods, from a variety of disciplinary and applied
fields but focusing on political science. Lessons will consist of a
mixture of theoretical grounding in content analysis approaches and
techniques, with hands on analysis of real texts using content analytic
and statistical software.

### Prerequisites

Students must have completed Applied Regression Analysis (MY452) or
equivalent.

Students in this course will strongly benefit from prior experience with
the R statistical package. All methods will be implemented in R, using
primarily the (instructor's) R package `quanteda` available from
<http://github.com/kbenoit/quanteda> and from CRAN.

### Assessment

#### Formative coursework

Five lab sessions on the indicated weeks will consist of supervised problem sets, with some questions to be completed outside of class. These will involve
computer exercises applied to texts supplied by the instructor. These
will be submitted via GitHub Classroom prior to the next lecture, and will be
marked to provide 60% of the course grade.

#### Project

A final project of 3,000 words will be due at the end of ST, and form
40% of the course grade. This will be an original analysis of texts
using some of the methods covered in class, and may focus on replicating
or extending a published work. Additional guidelines will be issued
about a third of the way through the class. The final lab will consist
of brief student presentations of their topics.


### Recommended Texts

There is no really good single textbook that exists to cover
computerized or quantitative text analysis, although Ken Benoit is currently
(slowly) writing one, entitled (*The Quantitative Analysis of Textual
Data*).

While not ideally fitting our core purpose, Krippendorf's classic
*Content Analysis* --- just updated --- is a good primer for manual
methods of content analysis and coverage of some of the same
fundamentals faced in quantitative text analysis.

-   Krippendorff, K. (2013). *Content Analysis: An Introduction to Its
    Methodology*. Sage, Thousand Oaks, CA, 3rd edition.

Other readings will consist of articles and book excerpts, which I will
make available on Moodle as pdf files.


### Schedule

#### Week 1. [Overview and fundamentals](https://github.com/lse-my459/lectures/blob/master/week01/)

This session will cover fundamentals, including the continuum from
traditional (non-computer assisted) content analysis to fully automated
quantitative text analysis. We will cover the conceptual foundations of
content analysis and quantitative content analysis, discuss the
objectives, the approach to knowledge, and the particular view of texts
when performing quantitative analysis. We will also discuss issues
including where to obtain textual data; formatting and working with text
files; indexing and meta-data; units of analysis; and definitions of
features and measures commonly extracted from texts, including stemming,
and stop-words.

*Lecture Notes:*

*Reading:*
* Grimmer and Stewart (2013)
* Manning, Raghavan and Schütze (2008, 117–120)

*Further Reading:*
* Manning, Raghavan and Schütze (2008, 117–120)
* [Wikipedia entry on Character](http://en.wikipedia.org/wiki/Text_encoding)
* Browse the different text file formats at <http://www.fileinfo.com/filetypes/text>
* Neuendorf (2002, Chs. 4–7)
* Krippendorff (2013, Ch. 6)

*Exercise:*
* Getting started with **quanteda**


#### Week 2: [Descriptive statistical methods for text analysis]()

Here we focus on quantitative methods for describing texts, focusing on
summary measures that highlight particular characteristics of documents
and allowing these to be compared. These methods include characterizing
texts through concordances, co-occurrences, and keywords in context;
complexity and readability measures; and an in-depth discussion of text
types, tokens, and equivalencies. We will also discuss weighting
strategies for features, such as *tf-idf*.

*Reading:*
* Krippendorff (2013, Chs. 9–10)
* Dunning (1993)
* Däubler et al. (2012)

*Further Reading:*
* DuBay (2004)

*Exercise:*
* Selecting, weighting, and summarizing texts and their features.

#### Week 3: [Quantitative methods for comparing texts]()
------------------------------------------------

Quantitative methods for comparing texts, through concordances and
keyword identification, dissimilarity measures, association models, and
vector-space models.

*Reading:*
* Krippendorff (2013, Ch. 10)
* Lowe et al. (2011)
* Manning, Raghavan and Schütze (2008, Section 6.3)

*Further Reading:*
* Seale, Ziebland and Charteris-Black (2006)

*Exercise:*
* Comparing texts and their features.


#### Week 4: [Automated dictionary methods]()

Automatic dictionary-based methods involve association of pre-defined
word lists with particular quantitative values assigned by the
researcher for some characteristic of interest. This topic covers the
design model behind dictionary construction, including guidelines for
testing and refining dictionaries. Hand-on work will cover commonly used
dictionaries such as LIWC, RID, and the Harvard IV-4, with applications.
We will also review a variety of text pre-processing issues and textual
data concepts such as word types, tokens, and equivalencies, including
word stemming and trimming of words based on term and/or document
frequency.

*Reading:*
* Neuendorf (2002, Ch. 6)
* Laver and Garry (2000)
* Rooduijn and Pauwels (2011)

*Further Reading:*
• Pennebaker and Chung (2008)
• Tausczik and Pennebaker (2010)
• Loughran and McDonald (2011)

*Exercise:*
* Applying, modifying, and creating dictionaries for the analysis of
political texts.

#### Week 5: [Machine Learning for Texts]()

Classification methods permit the automatic classification of texts in a
test set following machine learning from a training set. We will
introduce machine learning methods for classifying documents, including
one of the most popular classifiers, the Naive Bayes model. The topic
also introduces validation and reporting methods for classifiers and
discusses where these methods are applicable.

*Reading:*
* Manning, Raghavan and Schütze (2008, Ch. 13)
* Lantz (2013, Ch. 3–4)
* Evans et al. (2007)

*Further Reading:*
* Lantz (2013, Ch. 10)
* [Statsoft, "Naive Bayes Classifier Introductory Overview."](http://www.statsoft.com/textbook/naive-bayes-classifier)
* An [online article by Paul Graham on classifying spam e-mail](http://www.paulgraham.com/spam.html).
* Bionicspirit.com, 9 Feb 2012, ["How to Build a Naive Bayes Classifier."](http://bionicspirit.com/blog/2012/02/09/howto-build-naive-bayes-classifier.html)
* Yu, Kaufmann and Diermeier (2008)
* Zumel and Mount (2014, Ch. 5–6)

*Exercise:*
* Classifying legal documents and legislative speeches.

#### Week 7: [Supervised Scaling Models for Texts]()

Building on the Naive Bayes classifier, we introduce the "Wordscores" method of
Laver, Benoit and Garry (2003) for scaling latent traits, and show the link
between classification and scaling. We also cover applications of penalized
regression to score and scale texts.

*Reading:*
* Laver, Benoit and Garry (2003)
* Evans et al. (2007)

*Further Reading:*
* Benoit and Nulty (2013)
* Martin and Vanberg (2007)
* Benoit and Laver (2008)
* Lowe (2008)

*Exercise:*
* Scaling legal documents and legislative speeches.

#### Week 8: [Unsupervised Models for Scaling Texts]()

This session continues text scaling using unsupervised scaling methods,
based on parametric approaches modelling features as Bernoulli or
Poisson distributed, and contrasts these methods to other alternatives,
critically examining the assumptions such models rely upon. We also
cover non-parametric methods such as correspondence analysis and discuss
the similarity to parametric (Poisson-scaling) models.

*Reading:*
* Slapin and Proksch (2008)
* Lowe and Benoit (2013)

*Further Reading:*
* Clinton, Jackman and Rivers (2004)

*Exercise:*
* Using "Wordfish" and correspondence analysis to scale documents.


#### Week 9: [Similarity and clustering methods]()

Vector representations of documents, measuring distance and similarity,
hierarchical and k-means clustering. This topic also revisits feature
selection and weighting methods, especially *tf-idf*.

*Reading:*
* Manning, Raghavan and Schütze (2008, Ch. 6)
* Zumel and Mount (2014, Ch. 8)
* Choi, Cha and Tappert (2010)

*Further Reading:*
* Corley and Mihalcea (2005)
* James et al. (2013, Ch. 10.3)

*Exercise:*
* Clustering US presidential speeches; testing sentiment associations in
movie reviews.

#### Week 10: [Topic models]()

Topic extraction using the parametric Latent Dirichlet Allocation (LDA)
model.

*Reading:*
* Blei (2012)
* Blei, Ng and Jordan (2003)
* Beil, Ester and Xu (2002)

*Further Reading:*
* Chang et al. (2009)
* Manning, Raghavan and Schütze (2008, Ch. 16–17)
* Roberts et al. (2014)

*Exercise:*
* Using LDA to estimate document topics in political party programmes.

#### Week 11: [Working with Social Media]()

Social media such as micro-blogging site [Twitter](https://twitter.com) provide a wealth of
spontaneous, distributed, real-time text that can be used to analyze
almost any topic. We introduce the growing literature applying text
analysis techniques to this form of data, with examples for measuring
sentiment, networks, and locational information.

*Reading:*
* [Ginsberg et al. (2008)](http://www.nature.com/nature/journal/v457/n7232/full/nature07634.html)
* Barberá (2015)

*Further Reading:*
* Jürgens and Jungherr (2016)
* [Metaxas, Mustafaraj and Gayo-Avello (2011)](http://cs.wellesley.edu/~pmetaxas/How-Not-To-Predict-Elections.pdf)
* [Lampos, Preotiuc-Pietro and Cohn (2013)](http://staffwww.dcs.shef.ac.uk/people/T.Cohn/pubs/lampos13bilinear.pdf)

*Exercise:*
* Using Twitter to analyze sentiment in political blogs.
