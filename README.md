# Additional Human Evaluations for the Submissions of [WMT 2020](http://www.statmt.org/wmt20/) for English to German and Chinese to English.

The contents of this repository are not an official Google product.

We re-annotated the WMT 2020 English to German and Chinese to English test sets, comprising 1418 segments (130 documents) and 2000 segments (155 documents) respectively. For each set we chose 10 "systems" for annotation, including the three reference translations available for English to German and the two references available for Chinese to English. The MT outputs included all top-performing systems according to the WMT human evaluation, augmented with systems we selected to increase diversity. All raters were professional translators that are native speakers of the target language. We acquired 3 ratings per segment and all segments were evaluated in context.

To ensure maximum diversity in ratings, we assigned documents in round-robin fashion to all 20 different sets of 3 raters from these pools. We chose an assignment order that roughly balanced the number of documents and segments per rater. Each rater was assigned a subset of documents, and annotated outputs from all 10 systems for those documents. Both documents and systems were anonymized and presented in a different random order to each rater. The number of segments per rater ranged from 6,830--7,220 for English to German and from 9,860--10,210 for Chinese to English.

We refer to our paper for more details of the experimental setup.

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


## Types of extra human evaluations ##
### Multidimensional Quality Metric (MQM) ###
To adapt the generic MQM framework for our context, we followed the official [guidelines](http://qt21.eu/downloads/MQM-usage-guidelines.pdf) for scientific research.

Our annotators were instructed to identify all errors within each segment in a document, paying particular attention to document context. Each error was highlighted in the text, and labeled with an error category and a severity. To temper the effect of long segments, we imposed a maximum of five errors per segment, instructing raters to choose the five most severe errors for segments containing more errors.
Our error` hierarchy includes the standard top-level categories Accuracy, Fluency, Terminology, Style, and Locale, each with a specific set of  sub-categories. After an initial pilot run, we introduced a special Non-translation error that can be used to tag an entire segment which is too badly garbled to permit reliable identification of individual errors.Error severities are assigned independent of category, and consist of Major, Minor, and Neutral levels, corresponding respectively to actual translation or grammatical errors, smaller imperfections, and purely subjective opinions about the translation. 

Since we are ultimately interested in scoring segments, we require a weighting on error types. We fixed the weight on Minor errors at 1, and explored a range of Major weights from 1 to 10 (the Major weight recommended in the MQM standard). For each weight combination we examined the stability of system ranking using a resampling technique. We found that a Major weight of 5 gave the best balance between stability and ability to discriminate among systems.

These weights apply to all error categories with two exceptions. We assigned a weight of 0.1 to Minor Fluency/Punctuation errors to reflect their mostly non-linguistic nature. Decisions like the style of quotation mark to use or the spacing around punctuation affect the appearance of a text but do not change its meaning. Unlike other kinds of Minor errors, these are easy to correct algorithmically, so we assign a low weight to ensure that their main role is to distinguish between systems that are equivalent in other respects. Major Fluency/Punctuation errors, which render a text ungrammatical or change its meaning (eg, eliding the comma in “Let’s eat, grandma”), have standard weighting.
The second exception is the singleton Non-translation category, with a weight of 25, equivalent to five Major errors.

### Scalar Quality Metrics (SQM) ###
Similar to the WMT setting, the Scalar Quality Metric (SQM) evaluation collects segment-level scalar ratings with document context. Different from the 0-100 assessment of translation quality used in WMT, SQM uses a 0-6 scale for
translation quality assessment. Another difference is that the sentences were rated by professional translators instead of crowd workers or researchers. We refer to pSQM for SQM labels that were acquired with professional translators.

## Credits ##

If you use this data, please cite the following paper:

```
@misc{freitag2021expert,
      title={Experts, Errors, and Context: A Large-Scale Study of Human Evaluation for Machine Translation},
      author={Markus Freitag, George Foster, David Grangier, Viresh Ratnakar, Qijun Tan, Wolfgang Macherey},
      year={2021},
      eprint={2004.06063},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```