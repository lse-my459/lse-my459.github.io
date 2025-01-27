---
papersize: a4
documentclass: scrartcl
classoption: DIV=14
colorlinks: true
---

![LSE](lse-logo.jpg)
# Course Website for MY459 and MY360: Quantitative Text Analysis 

_Please note that the information on this page is provisional until the 
first lecture._

### Winter Term 2025

### Instructors

* [Ryan Hübert](mailto:r.hubert@lse.ac.uk), Department of Methodology. 
_Course convenor for MY459._
* [Friedrich Geiecke](mailto:f.c.geiecke@lse.ac.uk), Department of 
Methodology. _Course convenor for MY360._

All office hours should be booked on [StudentHub](https://studenthub.lse.ac.uk/).

### Course Information

* Lectures will take place Mondays 10:00-12:00 in CLM.3.02 during all 
Winter Term weeks except week 6 (LSE Reading Week).
* Seminars are two hours and will take place every other week, during 
Weeks 2, 4, 7, 9 and 11. Please see the LSE Timetable for times and 
locations of the seminars.
* Course Moodle pages (for announcements and some supplemental materials): 
[MY459](https://moodle.lse.ac.uk/course/view.php?id=10949), 
[MY360](https://moodle.lse.ac.uk/course/view.php?id=10933)

| **Week** | **Topic** | **Instructor** |
| 1 | [Introduction and Foundations](#week-1-introduction-and-foundations) | Ryan Hübert |
| 2 | [Quantifying Texts](#week-2-quantifying-texts) | Ryan Hübert |
| 3 | [Exploiting Word Meanings](#week-3-exploiting-word-meanings) | Ryan Hübert |
| 4 | [Classifying Texts into Categories](#week-4-classifying-texts-into-categories) | Ryan Hübert |
| 5 | [Scaling Latent Traits Using Texts](#week-5-scaling-latent-traits-using-texts) | Ryan Hübert |
| 6 | _Reading Week_ | |
| 7 | [Text Similarity and Clustering](#week-7-text-similarity-and-clustering) | Ryan Hübert |
| 8 | [Probabilistic Topic Models](#week-8-probabilistic-topic-models) | Friedrich Geiecke |
| 9 | [Methods Review and Neural Network Fundamentals](#week-9-methods-review-and-neural-network-fundamentals) | Friedrich Geiecke |
| 10 | [Static Word Embeddings](#week-10-static-word-embeddings) | Friedrich Geiecke |
| 11 | [Large Language Models and Alignment](#week-11-large-language-models-and-alignment) | Friedrich Geiecke |


### Administrative and Course Support

If you are in need of administrative support for this course:

* For auditing, registration, extensions, late assignments and department/school policy questions: 
[methodology.admin@lse.ac.uk](mailto:methodology.admin@lse.ac.uk)
* For questions about course platforms, including Moodle, website or GitHub Classrooms: 
[r.hubert@lse.ac.uk](mailto:r.hubert@lse.ac.uk)
* For other administrative issues related to MY459 or MY559: 
[r.hubert@lse.ac.uk](mailto:r.hubert@lse.ac.uk)
* For other administrative issues related to MY360: 
[f.c.geiecke@lse.ac.uk](mailto:f.c.geiecke@lse.ac.uk)

For all questions about _course content_, please schedule office hours 
with one of the instructors.

### Course Description

The course surveys methods for systematically extracting quantitative
information from texts for social scientific purposes, starting with the 
fundamentals of representing texts as quantitative data, then proceeding 
to explore several methods commonly used to draw social scientific 
lessons from texts. The course concludes with an introduction to the 
methods behind recent advances in large language models that serve as 
the basis of services like ChatGPT. The course lays a theoretical 
foundation for text analysis in the social sciences, but it also takes a 
practical and applied approach so that students learn how to apply these 
methods in research. The common focus across all methods is that they can 
be reduced to a three-step process: first, identifying texts and units of 
texts for analysis; second, extracting from the texts quantitatively 
measured features---such as coded content categories, word counts, word 
types, dictionary counts, or parts of speech---and converting these into 
a quantitative matrix; and third, using quantitative or statistical 
methods to analyse this matrix in order to generate inferences about the 
texts or their authors. The course systematically covers these methods 
in a logical progression, with a practical, hands-on approach where each 
technique will be applied using appropriate software to real texts.

### Prerequisites

Students must have completed MY452 (for MY459) or ST107 (for MY360), or
equivalent.

All methods will be implemented in R, often using the R packages 
in `tidyverse` as well as `quanteda`, all available from CRAN. We may 
also occasionally demonstrate how to do various quantitative text 
analysis tasks in python.

**We will assume all students have access to a computer that is capable 
of performing the quantitative text analysis techniques taught in this 
course, as well as a strong working knowledge of R and sufficient 
experience using it for data analysis. See Moodle for more
detail on how you can prepare.** 

### Assessments

* Formative: there will be one formative problem set during the Winter 
Term.
* Summative: there will be one two-hour exam during Spring Term (worth 
100% of your final mark).

We will provide more details later in WT.

### Recommended Texts

There are a wide range of textbooks on quantative text analysis. Since 
our focus in this course is on social science applications, we will rely 
heavily on a recent (and very good!) textbook on the topic:

- Grimmer, Justin, Margaret E. Roberts and Brandon M. Stewart (2022). 
*Text as Data: A New Framework for Machine Learning and the Social 
Sciences*. Princeton University Press, Princeton, NJ. This textbook is a 
recent survey of quantitative text analysis as used in the social 
sciences.

You may wish to purchase a copy for yourself, especially if you plan to 
pursue quantitative text analysis in future research.

There are many other textbooks covering various topics in quantitative 
text analysis from a variety of academic perspectives. Two of the most 
commonly cited are:

- Krippendorff, K. (2019). *Content Analysis: An Introduction to Its 
Methodology*. Sage, Thousand Oaks, CA, 4th edition. This textbook is 
a good primer for _manual_ methods of content analysis and coverage of 
some of the same fundamentals faced in quantitative text analysis. It
is available through the LSE library 
[here](https://librarysearch.lse.ac.uk/permalink/44LSE_INST/9pddrg/cdi_askewsholts_vlebooks_9781506395678).

- Jurafsky, Daniel and James H. Martin (2024). *Speech and Language 
Processing: An Introduction to Natural Language Processing, Computational 
Linguistics, and Speech Recognition with Language Models*. 3rd edition. 
Online manuscript released August 20, 2024. Available at 
https://web.stanford.edu/~jurafsky/slp3. This is a great reference book 
for the more technical aspects of quantitative text analysis.

Many of the readings listed below are articles, which are typically 
available via the LSE library.

### Coding Cheat Sheets

Coding "cheat sheets" contain useful code examples to get you started. 
Please refer to these materials before you book office hours!

- [`stringr` package](https://github.com/rstudio/cheatsheets/blob/main/strings.pdf)
- [`quanteda` package](https://muellerstefan.net/files/quanteda-cheatsheet.pdf)  
- [Regular Expressions](https://github.com/ashchan/cheatsheets/blob/master/misc/regular-expressions-cheat-sheet-v2.pdf)  

### Credits

A large proportion of the materials were adapted from content developed 
by Kenneth Benoit and Pablo Barbará for previous versions of this course. 
Some of the exercises were developed by Christian Mueller and Akitaka Matsuo.

### Schedule of Topics

*We may make minor modifications to the timing or ordering of topics as 
the term progresses, but we will not make any major revisions to the 
topics we plan to cover in this course.*

**Lecture slides, example code and reading lists will be updated in 
advance of each week's teaching. Please check back regularly.**

#### Week 1. [Introduction and Foundations](https://github.com/lse-my459/lectures/blob/master/week01/)

This lecture will begin with a conceptual overview of the main themes 
covered in this course, including why scholars use quantitative text 
analysis. Then, it will review course logistics and prerequisites, 
and cover core principles of digital text. 

**Coding Resources**
* Github Reference Materials](https://github.com/lse-my459/lectures/tree/master/github-user-guides)

**Primary Reading**
* Grimmer, Roberts and Stewart (2022, chs. 1-2)

**Further Reading**
* Grimmer and Stewart (2013)
* Manning, Raghavan and Schütze (2008, 117–120)
* Browse the different text file formats at <http://www.fileinfo.com/filetypes/text>
* Neuendorf (2002, Chs. 4–7), available through the LSE Library [here](https://librarysearch.lse.ac.uk/permalink/44LSE_INST/9pddrg/cdi_askewsholts_vlebooks_9781506361451)

#### Week 2: [Quantifying Texts](https://github.com/lse-my459/lectures/blob/master/week02/)

This lecture will cover the standard method for quantifying texts (the 
document feature matrix or DFM) and provide a high-level overview of 
the primary analytical approaches used with DFMs.

**Primary Reading**
* Grimmer, Roberts and Stewart (2022, chs. 3-9)

**Further Reading**
* Krippendorff (2019, Ch. 6, 9–10)
* Dunning (1993)
* Däubler et al. (2012)
* DuBay (2004)

**Seminar Materials** are available in the [week 2 directory](https://github.com/lse-my459/lectures/blob/master/week02/) on GitHub


#### Week 3: [Exploiting Word Meanings](https://github.com/lse-my459/lectures/blob/master/week03/)

This lecture will cover methods that use word meanings to learn about 
documents or social science concepts, including automated dictionary and 
discriminating words methods.

**Primary Reading**
* Grimmer, Roberts and Stewart (2022, chs. 11 and 16)

**Further Reading**
* Neuendorf (2002, Ch. 6)
* Young and Soroka (2012)
* Rooduijn and Pauwels (2011)
* Laver and Garry (2000)
* Loughran and McDonald (2011)
* Tausczik and Pennebaker (2010)
* Monroe, Colaresi and Quinn (2008)
* Nelson (2020)

#### Week 4: [Classifying Texts into Categories](https://github.com/lse-my459/lectures/blob/master/week04/)

This lecture will cover machine learning methods for classifying texts 
into a set of meaningful categories.

**Primary Reading**
* Grimmer, Roberts and Stewart (2022, chs. 17-20)

**Further Reading**
* Manning, Raghavan and Schütze (2008, Ch. 13)
* Evans et al. (2007)
* Miller et. al. (2020)
* Lantz (2013, Ch. 4 on Naive Bayes)
* James et al (2013). Chapters 1, 3, and 5.
* Lantz (2013, Ch. 10)
* [Statsoft, "Naive Bayes Classifier Introductory Overview."](http://www.statsoft.com/textbook/naive-bayes-classifier)
* An [online article by Paul Graham on classifying spam e-mail](http://www.paulgraham.com/spam.html).
* Bionicspirit.com, 9 Feb 2012, ["How to Build a Naive Bayes Classifier."](http://bionicspirit.com/blog/2012/02/09/howto-build-naive-bayes-classifier.html)
* Yu, Kaufmann and Diermeier (2008)
* Zumel and Mount (2014, Ch. 5–6)

**Seminar Materials**
* _to be posted_

#### Week 5: [Scaling Latent Traits Using Texts](https://github.com/lse-my459/lectures/blob/master/week05/)

This lecture will cover methods for placing texts on a latent trait 
scale, such as an ideological scale.

**Primary Reading**
* Grimmer, Roberts and Stewart (2022, sections 16.3.1 and 21.2)
* Laver, Benoit and Garry (2003)
* Slapin and Proksch (2008)

**Further Reading**
* Laver, Benoit and Garry (2003)
* Evans et al. (2007)
* Slapin and Proksch (2008)
* Lowe and Benoit (2013)
* Benoit and Nulty (2013)
* Martin and Vanberg (2007)
* Benoit and Laver (2008)
* Lowe (2008)
* Lauderdale and Herzog (2016)
* Mikolov et al. (2013)
* Pomeroy et al (2018)
* Schonhardt-Bailey (2008)


#### Week 6: NO LECTURES OR CLASSES/SEMINARS (READING WEEK)

#### Week 7: [Text Similarity and Clustering](https://github.com/lse-my459/lectures/blob/master/week07/)

This lecture will cover methods to measuring distance and similarity 
between documents, as well as standard approaches for clustering many 
documents into groups of similar documents.

**Primary Reading**
* Grimmer, Roberts and Stewart (2022, secs. 7.1-7.2 and ch. 12)

**Further Reading**
* Manning, Raghavan and Schütze (2008, Ch. 6)
* Choi, Cha and Tappert (2010)
* Corley and Mihalcea (2005)
* James et al. (2013, Ch. 10.3)
* Zumel and Mount (2014, Ch. 8)

**Seminar Materials**
* _to be posted_

#### Week 8: [Probabilistic Topic Models](https://github.com/lse-my459/lectures/blob/master/week08/)

This lecture will discuss probabilistic topic models such as the Latent
Dirichlet Allocation (LDA) model and the Structural Topic Model (STM).

**Primary Reading**
* Grimmer, Roberts and Stewart (2022, ch. 13)

**Further Reading**
* Blei (2012)
* Roberts et al. (2014)
* Blei, Ng and Jordan (2003)
* Beil, Ester and Xu (2002)
* Chang et al. (2009)
* Gilardi et al. (2017)
* Lucas et al (2015)
* Manning, Raghavan and Schütze (2008, Ch. 16–17)

#### Week 9: [Methods Review and Neural Network Fundamentals](https://github.com/lse-my459/lectures/blob/master/week09/)

This lecture will review key mathematical and methodological concepts, 
as well as introduce fundamental neural network architectures for text 
processing. These topics will form the basis for the final three weeks 
of the course.

**Note:** Before the lecture, please watch the first two videos from 
3Blue1Brown's neural networks series: 
<https://www.youtube.com/watch?v=aircAruvnKk&list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi>

**Seminar Materials**
* _to be posted_

#### Week 10: [Static Word Embeddings](https://github.com/lse-my459/lectures/blob/master/week10/)

This lecture will introduce the fundamentals of static word embeddings, 
i.e. fixed numerical vector representations of words.

**Primary Reading**
* Grimmer, Roberts and Stewart (2022, ch. 8)
* Mikolov et al (2013)
* Pennington et al (2014)

**Further Reading**
* Spirling and Rodriguez (2019)
* Caliskan et al (2017)

#### Week 11: [Large Language Models and Alignment](https://github.com/lse-my459/lectures/blob/master/week11/)

This lecture will provide a high level overview of current neural network 
based language models that form the foundation of tools like ChatGPT.

**Further Resources**
* Recent overview talk on LLMs by Andrej Karpathy: 
<https://www.youtube.com/watch?v=zjkBMFhNj_g>
* The Illustrated Transformer by Jay Alammar: 
<https://jalammar.github.io/illustrated-transformer/>

**Seminar Materials**
* _to be posted_

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

Krippendorff, Klaus. 2019. _Content Analysis: An Introduction to Its Methodology_. 4th ed. Thousand Oaks, CA: Sage.

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
