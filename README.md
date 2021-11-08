# Expert-based Human Evaluations for the Submissions of [WMT 2020](http://www.statmt.org/wmt20/) and [WMT 2021](http://www.statmt.org/wmt21/) for English to German and Chinese to English.

The contents of this repository are not an official Google product.

We re-annotated the WMT English to German and Chinese to English test sets newstest2020, newstest2021, and the TED talks WMT21 test suite with raters that are professional translators and native speakers of the target language.
The resulting human ratings are more reliable than crowd-worker human evaluations. 
We refer to our [paper](https://arxiv.org/pdf/2104.14478.pdf) for more details of the experimental setup.

You can use the [MQM Viewer](https://github.com/google-research/google-research/tree/master/mqm_viewer) web app to open these TSV data files for computing scores as well as for interactively slicing and dicing (details and screenshots presented further down in this documentation).

## Files part of this repository ##

1. [mqm_newstest2020_ende.tsv](newstest2020/ende/mqm_newstest2020_ende.tsv) MQM labels aqcuired for 10 submission of newstest2020 for English-to-German.

2. [psqm_newstest2020_ende.tsv](newstest2020/ende/psqm_newstest2020_ende.tsv) pSQM labels aqcuired for 10 submission of newstest2020 for English-to-German.

3. [mqm_newstest2020_zhen.tsv](newstest2020/zhen/mqm_newstest2020_zhen.tsv) MQM labels aqcuired for 10 submission of newstest2020 for Chinese-to-English.

4. [psqm_newstest2020_zhen.tsv](newstest2020/zhen/psqm_newstest2020_zhen.tsv) pSQM labels aqcuired for 10 submission of newstest2020 for Chinese-to-English.

5. [mqm-newstest2021_ende.tsv](newstest2021/ende/mqm-newstest2021_ende.tsv) MQM labels aqcuired for 15 submission of newstest2021 for English-to-German.

6. [mqm-newstest2021_zhen.tsv](newstest2021/zhen/mqm-newstest2021_zhen.tsv) MQM labels aqcuired for 15 submission of newstest2021 for Chinese-to-English.

7. [mqm-ted_ende.tsv](ted/ende/mqm-ted_ende.tsv) MQM labels aqcuired for 15 submission of TED talks for English-to-German.

8. [mqm-ted_zhen.tsv](ted/zhen/mqm-ted_zhen.tsv) MQM labels aqcuired for 15 submission of TED talks for Chinese-to-English.

## newstest2021 ##

### English to German ###

| System  | expert-based MQM | WMT DA |
| ------------- | ------------- | ------------- |
| ref-C | 0.51(1) | 0.320(3) |
| VolcTrans-GLAT | 1.04(2) | 0.301(6) |
| Facebook-AI | 1.05(3) | 0.378(2) |
| ref-A | 1.22(4) | 0.280(8) |
| Nemo | 1.34(5) | 0.250(10) |
| HuaweiTSC | 1.38(6) | 0.312(4) |
| Online-W | 1.46(7) | 0.391(1) |
| UEdin | 1.51(8) | 0.305(5) |
| eTranslation | 1.70(9) | 0.281(7) |
| VolcTrans-AT | 1.74(10) | 0.280(9) |

### Chinese to English ###

| System  | expert-based MQM | WMT DA |
| ------------- | ------------- | ------------- |
| ref-A | 4.35(1) | 0.019(3) |
| NiuTrans | 4.63(2) | 0.042(1) |
| SMU | 4.84(3) | 0.034(7) |
| MiSS | 4.93(4) | 0.029(5) |
| Borderline | 4.95(5) | 0.023(4) |
| DIDI-NLP | 5.1(6) | 0.031(2) |
| IIE-MT | 5.15(7) | 0.031(6) |
| Facebook-AI | 5.22(8) | 0.037(8) |
| Online-W | 5.57(9) | 0.087(9) |

## TED talks ##

### English to German ###

| System  | expert-based MQM |
| ------------- | ------------- |
| ref.A | 0.91(1) |
| Facebook-AI | 1.06(2) |
| Online-W | 1.12(3) |
| VolcTrans-AT | 1.24(4) |
| metricsystem3 | 1.44(5) |
| VolcTrans-GLAT | 1.49(6) |
| HuaweiTSC | 1.50(7) |
| metricsystem1 | 1.63(8) |
| metricsystem2 | 1.69(9) |
| metricsystem5 | 1.72(10) |
| UEdin | 1.77(11) |
| metricsystem4 | 1.78(12) |
| eTranslation | 1.96(13) |
| Nemo | 2.14(14) |

### Chinese to English ###

| System  | expert-based MQM |
| ------------- | ------------- |
| ref.B | 0.42(1) |
| DIDI-NLP | 1.65(2) |
| metricsystem2 | 1.76(3) |
| metricsystem1 | 1.90(4) |
| MiSS | 1.97(5) |
| IIE-MT | 1.98(6) |
| metricsystem4 | 2.05(7) |
| metricsystem5 | 2.15(8) |
| SMU | 2.202(9) |
| Borderline | 2.40(10) |
| NiuTrans | 2.49(11) |
| Facebook-AI | 2.64(12) |
| Online-W | 2.93(13) |
| metricsystem3 | 2.99(14) |
| ref.A | 5.52(15) |

## newstest2020 ##

### English to German ###

| System  | expert-based MQM | WMT DA |
| ------------- | ------------- | ------------- |
| Human-B | 0.75(1) | 0.57(1) |
| Human-A | 0.91(2) | 0.45(4) |
| Human-P | 1.41(3) | 0.30(10) |
| Tohoku-AIP-NTT | 2.02(4) | 0.47(3) |
| OPPO | 2.25(5) | 0.50(2) |
| eTranslation | 2.33(6) | 0.31(9) |
| Tencent_Translation | 2.35(7) | 0.39(6) |
| Huoshan_Translate | 2.45(8) | 0.33(7) |
| Online-B | 2.48(9) | 0.42(5) |
| Online-A | 2.99(10) | 0.32(8) |

### Chinese to English ###

| System  | expert-based MQM | WMT DA |
| ------------- | -------------  |------------- |
| Human-A | 3.43(1) | - |
| Human-B | 3.62(2) | -0.03(9) |
| VolcTrans | 5.03(3) | 0.10(1) |
| WeChat_AI | 5.13(4) | 0.08(3) |
| Tencent_Translation | 5.19(5) | 0.06(4) |
| OPPO | 5.20(6) | 0.05(7) |
| THUNLP | 5.34(7) | 0.03(8) |
| DeepMind | 5.41(8) | 0.05(6) |
| DiDi_NLP | 5.48(9) | 0.09(2) |
| Online-B | 5.85(10) | 0.06(5) |


## Types of extra human evaluations ##
### Multidimensional Quality Metric (MQM) ###
To adapt the generic MQM framework for our context, we followed the official [guidelines](http://qt21.eu/downloads/MQM-usage-guidelines.pdf) for scientific research.

Our annotators were instructed to identify all errors within each segment in a document, paying particular attention to document context. Each error was highlighted in the text, and labeled with an error category and a severity. To temper the effect of long segments, we imposed a maximum of five errors per segment, instructing raters to choose the five most severe errors for segments containing more errors.
Our error` hierarchy includes the standard top-level categories Accuracy, Fluency, Terminology, Style, and Locale, each with a specific set of  sub-categories. After an initial pilot run, we introduced a special Non-translation error that can be used to tag an entire segment which is too badly garbled to permit reliable identification of individual errors.Error severities are assigned independent of category, and consist of Major, Minor, and Neutral levels, corresponding respectively to actual translation or grammatical errors, smaller imperfections, and purely subjective opinions about the translation. 

Since we are ultimately interested in scoring segments, we require a weighting on error types. We fixed the weight on Minor errors at 1, and explored a range of Major weights from 1 to 10 (the Major weight recommended in the MQM standard). For each weight combination we examined the stability of system ranking using a resampling technique. We found that a Major weight of 5 gave the best balance between stability and ability to discriminate among systems.

These weights apply to all error categories with two exceptions. We assigned a weight of 0.1 to Minor Fluency/Punctuation errors to reflect their mostly non-linguistic nature. Decisions like the style of quotation mark to use or the spacing around punctuation affect the appearance of a text but do not change its meaning. Unlike other kinds of Minor errors, these are easy to correct algorithmically, so we assign a low weight to ensure that their main role is to distinguish between systems that are equivalent in other respects. Major Fluency/Punctuation errors, which render a text ungrammatical or change its meaning (eg, eliding the comma in “Let’s eat, grandma”), have standard weighting.
The second exception is the singleton Non-translation category, with a weight of 25, equivalent to five Major errors.

#### MQM Viewer: interactive analysis tool for MQM evaluations
The [MQM Viewer](https://github.com/google-research/google-research/tree/master/mqm_viewer) web app can be used to see detailed analysis of MQM evaluations. To use it, download the files `mqm-viewer.html`, `mqm-viewer.js`, and `mqm-viewer.css` to your computer:
```
wget https://raw.githubusercontent.com/google-research/google-research/master/mqm_viewer/mqm-viewer.{html,js,css}
```
Then, simply open the `mqm-viewer.html` file in a web browser, and use the "Choose file" button to pick an MQM TSV data file (downloaded to your computer). MQM data spans several columns, so it's best to use a desktop or laptop computer with a wide screen. You can intereactively slice and dice the evaluation results in MQM Viewer by filtering down to specific systems, documents, etc. Here are a couple of screenshot of the tool:

**Screenshot of evaluation metrics in MQM Viewer:**

![mqm-viewer-metrics](https://user-images.githubusercontent.com/86793140/140813203-c6d33dc7-3a27-45ba-9133-628c0f29f338.png)

**Screenshot of examples of rated sentences in MQM Viewer:**

![mqm-viewer-examples](https://user-images.githubusercontent.com/86793140/140813224-3bda536f-1f69-4f68-9b49-24bd058d666f.png)

### Scalar Quality Metrics (SQM) ###
Similar to the WMT setting, the Scalar Quality Metric (SQM) evaluation collects segment-level scalar ratings with document context. Different from the 0-100 assessment of translation quality used in WMT, SQM uses a 0-6 scale for
translation quality assessment. Another difference is that the sentences were rated by professional translators instead of crowd workers or researchers. We refer to pSQM for SQM labels that were acquired with professional translators.

## Credits ##

If you use this data, please cite the following paper:

```
@misc{freitag2021experts,
      title={Experts, Errors, and Context: A Large-Scale Study of Human Evaluation for Machine Translation}, 
      author={Markus Freitag and George Foster and David Grangier and Viresh Ratnakar and Qijun Tan and Wolfgang Macherey},
      year={2021},
      eprint={2104.14478},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```

