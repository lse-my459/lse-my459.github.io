---
papersize: a4
documentclass: scrartcl
classoption: DIV=14
colorlinks: true
---

![LSE](images/lse-logo.jpg)
# Lecture materials for MY459 and MY360 - Quantitative Text Analysis 

_Please note that the information on this page is provisional until the 
start of the term._

### Winter Term 2025

### Instructors

* [Ryan Hübert](mailto:r.hubert@lse.ac.uk), Department of Methodology. 
_Course convenor for MY459._
* [Friedrich Geiecke](mailto:f.c.geiecke@lse.ac.uk), Department of 
Methodology. _Course convenor for MY360._

For all office hours, please sign up at 
[StudentHub](https://studenthub.lse.ac.uk/).

### Course Information

* Lectures will take place Mondays 10:00-12:00 in CLM.3.02 during all 
Winter Term weeks except week 6 (LSE Reading Week).
* Seminars will take place every other week, during Weeks 2, 4, 7, 9 
and 11. Please see your course Moodle page for the times and locations 
of the seminars.
* Course Moodle pages: 
[MY459](https://moodle.lse.ac.uk/course/view.php?id=10949), 
[MY360](https://moodle.lse.ac.uk/course/view.php?id=10933)

| **Week** | **Topic**                                                                                                      |
|:--------:|:---------------------------------------------------------------------------------------------------------------|
| 1        | [Overview and Fundamentals](#week-1-overview-and-fundamentals)                                                 |
| 2        | [Descriptive Statistical Methods for Text Analysis](#week-2-descriptive-statistical-methods-for-text-analysis) |
| 3        | [Automated Dictionary Methods](#week-3-automated-dictionary-methods)                                           |
| 4        | [Machine Learning for Texts](#week-4-machine-learning-for-texts)                                               |
| 5        | [Supervised Scaling Models for Texts](#week-5-supervised-scaling-models-for-texts)                             |
| 6        | _Reading Week_                                                                                                 |
| 7        | [Unsupervised Models for Scaling Texts](#week-7-unsupervised-models-for-scaling-texts)                         |
| 8        | [Similarity and Clustering Methods](#week-8-similarity-and-clustering-methods)                                 |
| 9        | [Probabilistic Topic Models](#week-9-probabilistic-topic-models)                                                                           |
| 10       | [Word Embedding Fundamentals](#week-10-word-embedding-fundamentals)                                            |
| 11       | [Neural Network Based Language Models](#week-11-neural-network-based-language-models)                                                      |

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

Students must have completed MY452 (for MY459) or ST107 (for MY360), or
equivalent.

All methods will be implemented in R, often using the R package `quanteda`, 
available from CRAN. 

**We will assume all students have a strong working knowledge of R and 
sufficient experience using it for data analysis. See Moodle for more
detail on how you can prepare.** 

### Assessments

* Formative: there will be one formative problem set during the Winter 
Term.
* Summative: there will be one two-hour exam during Spring Term (worth 
100% of your final mark).

### Recommended Texts

Quantitative text analysis encompases a very wide range of methods of 
varying degrees of complexity, so no single textbook can hope to cover 
all topics in the field. However, there are a few textbooks that provide 
nice coverage of many of the concepts and topics we will cover in this 
class:

- Grimmer, Justin, Margaret E. Roberts and Brandon M. Stewart (2022). 
*Text as Data: A New Framework for Machine Learning and the Social Sciences*. 
Princeton University Press, Princeton, NJ. This textbook is a recent survey
of quantitative text analysis as used in the social sciences.
- Krippendorff, K. (2013). *Content Analysis: An Introduction to Its 
Methodology*. Sage, Thousand Oaks, CA, 3rd edition. This textbook is 
a good primer for _manual_ methods of content analysis and coverage of 
some of the same fundamentals faced in quantitative text analysis.
- Jurafsky, Daniel and James H. Martin (2024). *Speech and Language 
Processing: An Introduction to Natural Language Processing, Computational 
Linguistics, and Speech Recognition with Language Models*. 3rd edition. 
Online manuscript released August 20, 2024. Available at 
https://web.stanford.edu/~jurafsky/slp3. This is a great reference book 
for the more technical aspects of quantitative text analysis.

Most readings in the course will consist of articles and book excerpts, 
as listed below, which will either be made available via Moodle or 
through the links below.

### Coding Cheat Sheets

Coding "cheat sheets" contain useful code examples to get you started. 
Please refer to these materials before you book office hours!

- [Quanteda](https://muellerstefan.net/files/quanteda-cheatsheet.pdf)  
- [Regular Expressions](https://github.com/ashchan/cheatsheets/blob/master/misc/regular-expressions-cheat-sheet-v2.pdf)  
- [Glob](https://github.com/begin/globbing/blob/master/cheatsheet.md)

### Credits

A large proportion of the materials were adapted from content developed 
by Kenneth Benoit and Pablo Barbará for previous versions of this course. 
Some of the assignments were developed by Christian Mueller and Akitaka 
Matsuo.

### Provisional Schedule of Topics

**The following course schedule is provisional and subject to revisions 
before the beginning of the Winter Term. Although there will not be major 
changes in the following course content, some of the topics and readings 
may be modified or reorganised.**

*Important note: links to lecture slides and other course materials will 
be updated/added in advance of each week's teaching.*

#### Week 1. [Overview and fundamentals]()<!--(https://github.com/lse-my459/lectures/blob/master/week01/)-->

This session will cover fundamentals, including the continuum from
traditional (non-computer assisted) content analysis to fully automated
quantitative text analysis. We will cover the conceptual foundations of
content analysis and quantitative content analysis, discuss the
objectives, the approach to knowledge, and the particular view of texts
when performing quantitative analysis.

*Reading:*
* Grimmer and Stewart (2013)
* Manning, Raghavan and Schütze (2008, 117–120)

*Further Reading:*
* Browse the different text file formats at <http://www.fileinfo.com/filetypes/text>
* Neuendorf (2002, Chs. 4–7)
* Krippendorff (2013, Ch. 6)

#### Week 2: [Descriptive statistical methods for text analysis]()<!--(https://github.com/lse-my459/lectures/blob/master/week02/)-->

Here we focus on quantitative methods for describing texts, focusing on
summary measures that highlight particular characteristics of documents
and allowing these to be compared. We will also discuss issues
including where to obtain textual data; formatting and working with text
files; indexing and meta-data; units of analysis; and definitions of
features and measures commonly extracted from texts, including stemming,
and stop-words.

*Reading:*
* Krippendorff (2013, Chs. 9–10)
* Dunning (1993)
* Däubler et al. (2012)

*Further Reading:*
* DuBay (2004)

*Seminar Materials:* See the Moodle page for your course (links above).

*Github Reference Materials:* [Click here](https://github.com/lse-my459/lectures/tree/master/github-user-guides)

#### Week 3: [Automated dictionary methods]()<!--(https://github.com/lse-my459/lectures/blob/master/week03/)-->

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
* Young and Soroka (2012)
* Rooduijn and Pauwels (2011)

*Further Reading:*
* Laver and Garry (2000)
* Loughran and McDonald (2011)
* Tausczik and Pennebaker (2010)

#### Week 4: [Machine Learning for Texts]()<!--(https://github.com/lse-my459/lectures/blob/master/week04/)-->

Classification methods permit the automatic classification of texts in a
test set following machine learning from a training set. We will
introduce machine learning methods for classifying documents, including
one of the most popular classifiers, the Naive Bayes model. The topic
also introduces validation and reporting methods for classifiers and
discusses where these methods are applicable.

*Reading:*
* Manning, Raghavan and Schütze (2008, Ch. 13)
* Evans et al. (2007)
* Miller et. al. (2020)

*Further Reading:*
* Lantz (2013, Ch. 4 on Naive Bayes)
* James et al (2013). Chapters 1, 3, and 5.
* Lantz (2013, Ch. 10)
* [Statsoft, "Naive Bayes Classifier Introductory Overview."](http://www.statsoft.com/textbook/naive-bayes-classifier)
* An [online article by Paul Graham on classifying spam e-mail](http://www.paulgraham.com/spam.html).
* Bionicspirit.com, 9 Feb 2012, ["How to Build a Naive Bayes Classifier."](http://bionicspirit.com/blog/2012/02/09/howto-build-naive-bayes-classifier.html)
* Yu, Kaufmann and Diermeier (2008)
* Zumel and Mount (2014, Ch. 5–6)

*Seminar Materials:* See the Moodle page for your course (links above).

#### Week 5: [Supervised Scaling Models for Texts]()<!--(https://github.com/lse-my459/lectures/blob/master/week05/)-->

Building on the Naive Bayes classifier, we introduce the "Wordscores" method of
Laver, Benoit and Garry (2003) for scaling latent traits, and show the link
between classification and scaling.

*Reading:*
* Laver, Benoit and Garry (2003)
* Evans et al. (2007)

*Further Reading:*
* Benoit and Nulty (2013)
* Martin and Vanberg (2007)
* Benoit and Laver (2008)
* Lowe (2008)

#### Week 6: NO LECTURES OR SEMINARS (READING WEEK)

#### Week 7: [Unsupervised Models for Scaling Texts]()<!--(https://github.com/lse-my459/lectures/blob/master/week07/)-->

This session continues text scaling using unsupervised scaling methods,
based on parametric approaches modelling features as Poisson distributed (Wordfish
and Wordshoal) or non-parametric approaches such as correspodence analysis.

*Reading:*
* Slapin and Proksch (2008)
* Lowe and Benoit (2013)

*Further Reading:*
* Lauderdale and Herzog (2016)
* Mikolov et al. (2013)
* Pomeroy et al (2018)
* Schonhardt-Bailey (2008)

*Seminar Materials:* See the Moodle page for your course (links above).

#### Week 8: [Similarity and clustering methods]()<!--(https://github.com/lse-my459/lectures/blob/master/week08/)-->

Vector representations of documents, measuring distance and similarity,
hierarchical and k-means clustering. This topic also revisits feature
selection and weighting methods, especially *tf-idf*.

*Reading:*
* Manning, Raghavan and Schütze (2008, Ch. 6)
* Choi, Cha and Tappert (2010)

*Further Reading:*
* Corley and Mihalcea (2005)
* James et al. (2013, Ch. 10.3)

* Zumel and Mount (2014, Ch. 8)

#### Week 9: [Probabilistic topic models]()<!--(https://github.com/lse-my459/lectures/blob/master/week09/)-->

This session will discuss probabilistic topic models. We will learn how to run the Latent
Dirichlet Allocation (LDA) model and the Structural
Topic Model (STM), which allows researchers to use covariates to learn
about the prevalence and content of topics.

*Reading:*
* Blei (2012)
* Roberts et al. (2014)

*Further Reading:*
* Blei, Ng and Jordan (2003)
* Beil, Ester and Xu (2002)
* Chang et al. (2009)
* Gilardi et al. (2017)
* Lucas et al (2015)
* Manning, Raghavan and Schütze (2008, Ch. 16–17)

*Seminar Materials:* See the Moodle page for your course (links above).

#### Week 10: [Word embedding fundamentals]()<!--(https://github.com/lse-my459/lectures/blob/master/week10/)-->

This week will discuss fundamentals of numerical vector representations for words.

*Reading:*

* Spirling and Rodriguez (2019)
* Caliskan et al (2017)

*Further Reading:*
* Gurciullo and Mikhaylov (2017)
* Mikolov et al (2013)

#### Week 11: [Neural network based language models]()<!--(https://github.com/lse-my459/lectures/blob/master/week11/)-->

This week will give a high level overview of some current neural network based models for text that go beyond the bag-of-words assumption.

*Before the lecture:*

* Please watch the first two of the following videos on neural networks by 3Blue1Brown: <https://www.youtube.com/watch?v=aircAruvnKk&list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi>

*Further materials (optional!):*
* Recent overview talk on LLMs by Andrej Karpathy: <https://www.youtube.com/watch?v=zjkBMFhNj_g>
* The Illustrated Transformer by Jay Alammar: <https://jalammar.github.io/illustrated-transformer/>

*Seminar Materials:* See the Moodle page for your course (links above).

### References

Barberá, Pablo. 2015. "Birds of the Same Feather Tweet Together: Bayesian Ideal Point Estimation Using Twitter Data." _Political Analysis_ 23(1):76--91. doi: [`10.1093/pan/mpu011`](https://doi.org/10.1093/pan/mpu011).

Beauchamp, N. 2017. "[Predicting and Interpolating State‐Level Polls Using Twitter Textual Data.](http://onlinelibrary.wiley.com/doi/10.1111/ajps.12274/full)" American Journal of Political Science, 61(2), 490-503.

Beil, F, M Ester and X Xu. 2002. Frequent term-based text clustering. In _Eighth ACM SIGKDD international conference on Knowledge discovery and data mining_. pp. 436–442.

Benoit, K. and M. Laver. 2008. “Compared to What? A Comment on ‘A Robust Transformation
Procedure for Interpreting Political Text’ by Martin and Vanberg.” _Political Analysis_ 16(1):101–111. doi: [`10.1093/pan/mpm020`](https://doi.org/10.1093/pan/mpm020).

Benoit, Kenneth and Paul Nulty. 2013. “Classification Methods for Scaling Latent Political Traits.” Presented at the Annual Meeting of the Midwest Political Science Association, April 11–14, Chicago.

Blei, David M. 2012. “Probabilistic topic models.” _Communications of the ACM_ 55(4):77. doi: [`10.1145/2133806.2133826`](https://doi.org/10.1145/2133806.2133826).

Blei, D.M., A.Y. Ng and M.I. Jordan. 2003. “Latent dirichlet allocation.” _The Journal of Machine Learning Research_ 3:993–1022.

Caliskan, A., Bryson, J.J., and Narayanan, A. 2017. "[Semantics derived automatically from language corpora contain human-like biases](http://science.sciencemag.org/content/356/6334/183/tab-figures-data)", _Science_.

Chang, J., J. Boyd-Graber, S. Gerrish, C. Wang and D. Blei. 2009. Reading tea leaves: How humans interpret topic models. In _Neural Information Processing Systems._

Choi, Seung-Seok, Sung-Hyuk Cha and Charles C. Tappert. 2010. “A Survey of Binary Similarity and Distance Measures.” _Journal of Systemics, Cybernetics and Informatics_ 8(1):43–48.

Clinton, J., S. Jackman and D. Rivers. 2004. “The statistical analysis of roll call voting: A unified approach.” _American Journal of Political Science_ 98(2):355–370. doi: [`10.1017/s0003055404001194`](https://doi.org/10.1017/s0003055404001194).

Corley, Courtney and Rada Mihalcea. 2005. Measuring the semantic similarity of texts. In _Proceedings of the ACL Workshop on Empirical Modeling of Semantic Equivalence and Entailment - EMSEE ’05_.

Däubler, Thomas, Kenneth Benoit, Slava Mikhaylov and Michael Laver. 2012. “Natural Sentences as Valid Units for Coded Political Texts.” _British Journal of Political Science_ 42(4):937–951. doi: [`10.1017/S0007123412000105`](https://doi.org/10.1017/S0007123412000105).

DuBay, William. 2004. The Principles of Readability. Costa Mesa, California. <http://www.impact-information.com/impactinfo/readability02.pdf>.

Dunning, Ted. 1993. “Accurate methods for the statistics of surprise and coincidence.” _Computational Linguistics_ 19:61–74.

Evans, Michael, Wayne McIntosh, Jimmy Lin and Cynthia Cates. 2007. “Recounting the Courts?
Applying Automated Content Analysis to Enhance Empirical Legal Research.” _Journal of Empirical Legal Studies_ 4(4):1007–1039.

Gilardi, F., Shipan, C. R., & Wueest, B. 2017. "[Policy Diffusion: The Issue-Definition Stage.](https://www.fabriziogilardi.org/resources/papers/policy-diffusion-issue-definition.pdf)" Working paper, University of Zurich.

Ginsberg, Jeremy, Matthew H Mohebbi, Rajan S Patel, Lynnette Brammer, Mark S Smolinski and Larry Brilliant. 2008. “Detecting influenza epidemics using search engine query data.” _Nature_ 457(7232):1012–1014.

Grimmer, Justin and Brandon M. Stewart. 2013. “Text as Data: The Promise and Pitfalls of Automatic Content Analysis Methods for Political Texts.” _Political Analysis_ 21(3):267–297. doi: [`10.1093/pan/mps028`](https://doi.org/10.1093/pan/mps028).

Grimmer, Justin, Margaret E. Roberts and Brandon M. Stewart. 2022. *Text as Data: A New Framework for Machine Learning and the Social Sciences*. Princeton University Press, Princeton, NJ. 

Gurciullo, S. and Mikhaylov, S. 2017. "[Detecting policy preferences and dynamics in the UN general debate with neural word embeddings](https://ieeexplore.ieee.org/document/8253197)", _2017 International Conference on the Frontiers and Advances in Data Science_.

James, Gareth, Daniela Witten, Trevor Hastie and Robert Tibshirani. 2013. _An Introduction to Statistical Learning with Applications in R_. Springer Science & Business Media.

Jürgens, Pascal and Andreas Jungherr. 2016. “A Tutorial for Using Twitter Data in the Social Sciences: Data Collection, Preparation, and Analysis.”

Klašnja, M., Barberá, P., Beauchamp, N., Nagler, J., & Tucker, J. 2016. "[Measuring public opinion with social media data.](http://www.oxfordhandbooks.com/view/10.1093/oxfordhb/9780190213299.001.0001/oxfordhb-9780190213299-e-3)" In The Oxford Handbook of Polling and Survey Methods.

Krippendorff, Klaus. 2013. _Content Analysis: An Introduction to Its Methodology_. 3rd ed. Thousand Oaks, CA: Sage.

Lampos, Vasileios, Daniel Preotiuc-Pietro and Trevor Cohn. 2013. A user-centric model of voting intention from Social Media. In _Proceedings of the 51st Annual Meeting of the Association for Computational Linguistics (ACL)_.

Lantz, Brett. 2013. _Machine Learning with R._ Packt Publishing Ltd.

Laver, M. and J. Garry. 2000. “Estimating policy positions from political texts.” _American Journal of Political Science_ 44(3):619–634. doi: [`10.2307/2669268`](https://doi.org/10.2307/2669268).

Laver, Michael, Kenneth Benoit and John Garry. 2003. “Estimating the policy positions of political actors using words as data.” _American Political Science Review_ 97(2):311–331. doi: [`10.1017/S0003055403000698`](https://doi.org/10.1017/S0003055403000698).

Loughran, Tim and Bill McDonald. 2011. “When Is a Liability Not a Liability? Textual Analysis, Dictionaries, and 10-Ks.” _The Journal of Finance_ 66(1):35–65.

Lowe, W. 2008. “Understanding Wordscores.” _Political Analysis_ 16(4):356–371. doi: [`10.1093/pan/mpn004`](https://doi.org/10.1093/pan/mpn004).

Lowe, William and Kenneth Benoit. 2013. “Validating Estimates of Latent Traits From Textual Data Using Human Judgment as a Benchmark.” _Political Analysis_ 21(3):298–313. doi: [`10.1093/pan/mpt002`](https://doi.org/10.1093/pan/mpt002).

Lowe, William, Kenneth Benoit, Slava Mikhaylov and Michael Laver. 2011. “Scaling Policy Preferences From Coded Political Texts.” _Legislative Studies Quarterly_ 26(1):123–155. doi: [`10.1111/j.1939-9162.2010.00006.x`](https://doi.org/10.1111/j.1939-9162.2010.00006.x).

Lucas, C., Nielsen, R. A., Roberts, M. E., Stewart, B. M., Storer, A., & Tingley, D. 2015. "[Computer-assisted text analysis for comparative politics.](http://scholar.princeton.edu/sites/default/files/bstewart/files/comparativepoliticstext.pdf)" Political Analysis, 23(2), 254-277.

Manning, C. D., P. Raghavan and H. Schütze. 2008. _Introduction to Information Retrieval_. Cambridge University Press.

Martin, L. W. and G. Vanberg. 2007. “A robust transformation procedure for interpreting political text.” _Political Analysis_ 16(1):93–100. doi: [`10.1093/pan/mpm010`](https://doi.org/10.1093/pan/mpm010).

Metaxas, Panagiotis T., Eni Mustafaraj and Daniel Gayo-Avello. 2011. How (not) to predict elections. In _Privacy, security, risk and trust (PASSAT), 2011 IEEE third international conference on social computing (SocialCom)_.

Mikolov, T., Chen, K., Corrado, G., & Dean, J. 2013. "Efficient estimation of word representations in vector space." [arXiv preprint arXiv:1301.3781.](https://arxiv.org/pdf/1301.3781.pdf)

Neuendorf, K. A. 2002. _The Content Analysis Guidebook_. Thousand Oaks CA: Sage.

Pennebaker, J. W. and C. K. Chung. 2008. Computerized text analysis of al-Qaeda transcripts. In _The Content Analysis Reader_, ed. K. Krippendorf and M. A. Bock. Thousand Oaks, CA: Sage.

Pomeroy, C, Dasandi, N. and S. Mikhaylov. 2018. ["Disunited Nations? A Multiplex Network Approach to Detecting Preference Affinity Blocs using Texts and Votes"](https://arxiv.org/pdf/1802.00396.pdf)

Roberts, Margaret E, Brandon M Stewart, Dustin Tingley, Christopher Lucas, Jetson Leder-Luis, Shana Kushner Gadarian, Bethany Albertson and David G Rand. 2014. “Structural Topic Models for Open-Ended Survey Responses.” _American Journal of Political Science_ 58(4):1064–1082. doi: [`10.1080/01621459.2016.1141684`](https://doi.org/10.1080/01621459.2016.1141684).

Rooduijn, Matthijs and Teun Pauwels. 2011. “Measuring Populism: Comparing Two Methods of
Content Analysis.” _West European Politics_ 34(6):1272–1283.

Ruths, D., & Pfeffer, J. 2014. "[Social media for large studies of behavior.](http://science.sciencemag.org/content/346/6213/1063.full)" Science, 346(6213), 1063-1064.

Schonhardt-Bailey, C. (2008). The congressional debate on partial-birth abortion: Constitutional gravitas and moral passion. British journal of political science, 38(3), 383-410.

Seale, Clive, Sue Ziebland and Jonathan Charteris-Black. 2006. “Gender, cancer experience and internet use: A comparative keyword analysis of interviews and online cancer support groups.” _Social Science & Medicine_ 62(10):2577–2590.

Slapin, Jonathan B. and Sven-Oliver Proksch. 2008. “A Scaling Model for Estimating Time-Series Party Positions from Texts.” _American Journal of Political Science_ 52(3):705–722. doi: [`10.1111/j.1540-5907.2008.00338.x`](10.1111/j.1540-5907.2008.00338.x).

Spirling, A. and Rodriguez, P.L. 2019. "[Word Embeddings. What works, what doesn't, and how to tell the difference for applied research.](https://github.com/ArthurSpirling/EmbeddingsPaper/blob/master/Paper/Embeddings_SpirlingRodriguez.pdf)".

Steinert-Threlkeld, Z. 2018. "[Twitter as Data.](https://www.cambridge.org/core/elements/twitter-as-data/27B3DE20C22E12E162BFB173C5EB2592)" Cambridge University Press.

Tausczik, Y R and James W Pennebaker. 2010. “The Psychological Meaning of Words: LIWC and
Computerized Text Analysis Methods.” _Journal of Language and Social Psychology_ 29(1):24–54.

Young, L., and Soroka, S. 2012. "[Affective news: The automated coding of sentiment in political texts.](http://www.tandfonline.com/doi/abs/10.1080/10584609.2012.671234)" Political Communication, 29(2), 205-231.

Yu, B., S. Kaufmann and D. Diermeier. 2008. “Classifying Party Affiliation from Political Speech.” _Journal of Information Technology and Politics_ 5(1):33–48.

Zumel, Nina and John Mount. 2014. _Practical Data Science with R_. Manning Publications.
