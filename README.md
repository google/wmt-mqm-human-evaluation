# Additional Human Evaluations for the Submissions of [WMT 2020](http://www.statmt.org/wmt20/) for English to German and Chinese to English.

The contents of this repository are not an official Google product.

We re-annotated the WMT 2020 English to German and Chinese to English test sets, comprising 1418 segments (130 documents) and 2000 segments (155 documents) respectively. For each set we chose 10 "systems" for annotation, including the three reference translations available for English to German and the two references available for Chinese to English. The MT outputs included all top-performing systems according to the WMT human evaluation, augmented with systems we selected to increase diversity. All raters were professional translators that are native speakers of the target language. We acquired 3 ratings per segment and all segments were evaluated in context.

To ensure maximum diversity in ratings, we assigned documents in round-robin fashion to all 20 different sets of 3 raters from these pools. We chose an assignment order that roughly balanced the number of documents and segments per rater. Each rater was assigned a subset of documents, and annotated outputs from all 10 systems for those documents. Both documents and systems were anonymized and presented in a different random order to each rater. The number of segments per rater ranged from 6,830--7,220 for English to German and from 9,860--10,210 for Chinese to English.

We refer to our paper for more details of the experimental setup.

## Types of extra human evaluations ##
### Multidimensional Quality Metrics (MQM) ###
The Multidimensional Quality Metrics (MQM) framework was developed in the EU QTLaunchPad and [QT21](www.qt21.eu) projects.
It provides a generic methodology for assessing translation quality that can be adapted to a wide range of evaluation needs. The core idea is to establish a standard hierarchy of translation issues (potential errors) that can be pruned or extended with new issues as required. Annotators identify issues in text at a suitable granularity, and the results are summarized using a procedure that is specific to the application. Please read our paper to see how we adapted MQM to the machine translation use case.

### Scalar Quality Metrics (SQM) ###
Similar to the WMT setting, the Scalar Quality Metric (SQM) evaluation collects segment-level scalar ratings with document context. Different from the 0-100 assessment of translation quality used in WMT, SQM uses a 0-6 scale for
translation quality assessment. Another difference is that the sentences were rated by professional translators instead of crowd workers or researchers. We refer to pSQM for SQM labels that were acquired with professional translators.


## Files part of this repository ##

1. [mqm_newstest2020_ende.tsv](ende/mqm_newstest2020_ende.tsv) MQM labels aqcuired for 10 submission of WMT 2020 for English-to-German.

2. [psqm_newstest2020_ende.tsv](ende/psqm_newstest2020_ende.tsv) pSQM labels aqcuired for 10 submission of WMT 2020 for English-to-German.

3. [mqm_newstest2020_zhen.tsv](zhen/mqm_newstest2020_zhen.tsv) MQM labels aqcuired for 10 submission of WMT 2020 for Chinese-to-English.

4. [psqm_newstest2020_zhen.tsv](zhen/psqm_newstest2020_zhen.tsv) pSQM labels aqcuired for 10 submission of WMT 2020 for Chinese-to-English.


## Individual system included in the re-evaluation ##

### English to German ###
Human-A.0\
Human-B.0\
Human-P.0\
OPPO.1535\
Tohoku-AIP-NTT.890\
Online-B.1590\
Tencent Translation.1520\
Huoshan Translate.832\
Online-A.1574\
eTranslation.737

### Chinese to English ###
Human-A.0\
Human-B.0\
Huoshan Translate.919\
DiDi NLP.401\
WeChat AI.1525\
Tencent Translation.1249\
Online-B.1605\
DeepMind.381\
OPPO.1422\
THUNLP.1498

