# Dataset from Dear Uncle Skinner Project
## Introduction
This repository contains the annotated datasets from my MSc Project and will later host the fully annotated dataset of agony aunt letters according to verbal behaviour theory from my PhD project. To find out more about my project please visit the project website [here](https://dear-uncle-skinner.ch). Website is currently in development.

## Original Dataset
The original MSc Dataset was used to create a predictive model which aimed to predict the subject of a text, the behaviour of concern and predict a behaviour analyst's initial hypothesis about the probable function of the behaviour [1,2,3]. The dataset is the first known dataset of its type used to make hypothetical predictions about behavioural function. The dataset will be regularly updated, when further documents are annotated.

The documents consist of an unstructured corpus which aims to be somewhat reflective of the typical interactions between practitioners and service users. Additionally, in order to train the model a significant dataset is be required. The documents were scrapped from a public source of agony aunt letters. These letter share some of the same lexical, syntactical and grammatical properties of texts encountered by behavioural analytical practitioners in digital communications mediums such as E-Mails, especially in the initial stages of a therapy. In order to obtain this data a web-scrapping programme was used pull the texts of the Guardian Dear Mariella page [4,5]. The programme successfully extracted 813 documents. The documents were then multiplied by four to ensure that each identified subject could be annotated as the main subject at least once. Due to formatting changes on the guardian website overtime, addition text such as replies was also unintentionally extracted. In order to remove any interpretation bias brought about by the agony aunt responses, the replies were removed prior to annotation.

In order to collate the agony aunt letters and build the data set, the python module Beautiful Soup was used [4]. All scripts were completed in the Jupyter Lab IDE. The data was annotated using the software doccano [6]. Doccando provides researchers the possibility to easily complete sequence analysis within a user friendly user interface (UI). The software is created and written in python and provides an API to import data automatically via Jupyter Lab. However, the original UIs simplicity constrains its functionality and it was originally not possible to support nested annotation without making significant changes. As such this was one of the reasons the documents were copied four times. As it allowed for at least 4 iterations of annotations in relation to different behavioural subjects (see Targets).

Recent changes to Doccano allow for relational and nested tagging. As such alleviating the need for the duplication of documents [6].

### Legend of labels
The labels used in the initial MSc dataset are:

**Targets**
- Main Target: *Is defined as the person who is thought to exhibit the behaviour of interest. Annotators are instructed to mark the main target as the person who appears to be the subject of interest by the author*
- Alternative Target 1: *Another subject of interest in the text who exhibits a behaviour*
- Alternative Target 2: *Another subject of interest in the text who exhibits a behaviour*
- Alternative Target 3: *Another subject of interest in the text who exhibits a behaviour*

**Antecedents**
- EO: *Establishing Operation, A notable component/state of a stimulus that increases the effectiveness of some stimulus, object, or event as a reinforcer.*
- AO: *Abolishing Operation, A notable component/state of a stimulus that decreases the effectiveness of some stimulus, object, or event as a reinforcer.*
- SDP: *A stimulus which indicates the probable availability of a punisher for a given behaviour and decreases the immediate likelihood a given behaviour will be evoked*
- SD: *A stimulus which indicates the probable availability of a reinforcer for a given behaviour and increases the immediate likelihood a given behaviour will be evoked*
- S-Delta: *A stimulus which indicates the probable unavailability of a reinforcer for a given behaviour and decreases the immediate likelihood a given behaviour will be evoked*
- Unclassifiable Antecedent: *An Antecedent to a behaviour which function is not clear from the text. However, is noted by the author as being in some way significant*

**Behaviours and Reflexes**
- Operant Behaviour: *Behaviour that appears to be is selected, maintained, and brought under "stimulus control" as through continued presentation of a given consequences. This is learnt behaviour*
- Verbal Behaviour: *In addition to fulfilling the characteristics of an Operant behaviour (appears to be is selected, maintained, and brought under "stimulus control" as through continued presentation of a given consequences. This is learnt behaviour). This behaviour is clearly exhibited for the purpose of communication and there is implicit train group of listeners who can understand and respond to the behaviour* (this is a broad label encompassing all possible verbal operants, this label will be expanded in the PhD project).
- Reflex: *A stimulus–response relation consisting of an antecedent stimulus and the respondent behaviour it elicits. The respondent behaviour is not reinforced and is phylogenic in nature*

**Consequences**
- SR+: *A named primary need (warmth, food, drink) which in the narrative of the document often follows a behaviour and the behaviour is reported to increase overtime.*
- Sr+: *A socially mediated stimulus which in the narrative of the document often follows a behaviour and the behaviour is reported to increase overtime.*
- Sr-: *A socially mediated stimulus which in the narrative of the document is often removed after a behaviour and the behaviour is reported to increase overtime.*
- Positive Punisher: *A  stimulus which in the narrative of the document often follows a behaviour and the behaviour is reported to decreases overtime.*
- Negative Punisher: *A stimulus which in the narrative of the document is often removed after a behaviour and the behaviour is reported to decrease overtime.*
- Non-Response: *The subject of the text was reported to react to a given stimulus (verbal or otherwise) and is reported to no longer respond to the same stimulus*
- Delta Extinction: *A report in the text of a stimulus that has often followed a behaviour and lead to an increase in the behaviour. The stimulus now no longer follows the behaviour and the behaviour decreases (a momentary increase in the targets behaviour with varying topographies and intensities may be reported).*
- Unclassifiable Consequence: *A report in the text of a stimulus that has often followed a behaviour but its effect on the behaviour is unclear.*

**Behavioural Dimension**
- Time: *Duration of the behaviour.*
- Quantifier: *How many times the behaviour occurred or any references to the intensity of the behaviour.*

**Other**
- Mentalism: *An explanation for the behaviour within the text which refers to something within the individual, often outside of their control, a state of being rather than a measurable behaviour explicitly carried out by the individual.*

## Descriptive Statics of MSc. Dataset
**Last updated**: 1st May 2022

<table>
  <thead>
    <tr class="header">
      <th>
      </th>
      <th colspan="4">
        Metric
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <b>
          Target
        </b>
      </td>
      <td>
        <i>
          N
        </i>
      </td>
      <td>
        <i>
          M
        </i>
      </td>
      <td>
        <i>
          SD
        </i>
      </td>
      <td>
        <i>
          SE
        </i>
      </td>
    </tr>
    <tr>
      <td>
        Main Target
      </td>
      <td>
        436
      </td>
      <td>
        6.92
      </td>
      <td>
        6.70
      </td>
      <td>
        0.84
      </td>
    </tr>
    <tr>
      <td>
        Alternative Target 1
      </td>
      <td>
        527
      </td>
      <td>
        8.36
      </td>
      <td>
        6.92
      </td>
      <td>
        0.87
      </td>
    </tr>
    <tr>
      <td>
        Alternative Target 2
      </td>
      <td>
        116
      </td>
      <td>
        1.84
      </td>
      <td>
        2.11
      </td>
      <td>
        0.27
      </td>
    </tr>
    <tr>
      <td>
        Alternative Target 3
      </td>
      <td>
        36
      </td>
      <td>
        0.57
      </td>
      <td>
        0.98
      </td>
      <td>
        0.12
      </td>
    </tr>
    <tr>
      <td>
        <b>Antecedents</b>
      </td>
      <td colspan="4">
      </td>
    </tr>
    <tr>
      <td>
        EO
      </td>
      <td>
        27
      </td>
      <td>
        0.43
      </td>
      <td>
        0.87
      </td>
      <td>
        0.11
      </td>
    </tr>
    <tr>
      <td>
        AO
      </td>
      <td>
        20
      </td>
      <td>
        0.32
      </td>
      <td>
        0.84
      </td>
      <td>
        0.11
      </td>
    </tr>
    <tr>
      <td>
        SDP
      </td>
      <td>
        7
      </td>
      <td>
        0.11
      </td>
      <td>
        0.41
      </td>
      <td>
        0.05
      </td>
    </tr>
    <tr>
      <td>
        SD
      </td>
      <td>
        16
      </td>
      <td>
        0.25
      </td>
      <td>
        0.67
      </td>
      <td>
        0.08
      </td>
    </tr>
    <tr>
      <td>
        S-Delta
      </td>
      <td>
        1
      </td>
      <td>
        0.02
      </td>
      <td>
        0.13
      </td>
      <td>
        0.02
      </td>
    </tr>
    <tr>
      <td>
        Unclassifiable Antecedent
      </td>
      <td>
        9
      </td>
      <td>
        0.14
      </td>
      <td>
        0.53
      </td>
      <td>
        0.07
      </td>
    </tr>
    <tr>
      <td>
        <b>Behaviours and Reflexes</b>
      </td>
      <td colspan="4">
      </td>
    </tr>
    <tr>
    <tr>
      <td>
        Operant behaviour
      </td>
      <td>
        119
      </td>
      <td>
        1.89
      </td>
      <td>
        2.46
      </td>
      <td>
        0.31
      </td>
    </tr>
    <tr>
      <td>
        Verbal behaviour
      </td>
      <td>
        77
      </td>
      <td>
        1.22
      </td>
      <td>
        1.33
      </td>
      <td>
        0.17
      </td>
    </tr>
    <tr>
      <td>
        Reflex
      </td>
      <td>
        2
      </td>
      <td>
        0.03
      </td>
      <td>
        0.18
      </td>
      <td>
        0.02
      </td>
    </tr>
    <tr>
      <td>
        <b>Consequences</b>
      </td>
      <td colspan="4">
      </td>
    </tr>
    <tr>
      <td>
        SR+
      </td>
      <td>
        0
      </td>
      <td>
        0.00
      </td>
      <td>
        0.00
      </td>
      <td>
        0.00
      </td>
    </tr>
    <tr>
      <td>
        Sr+
      </td>
      <td>
        7
      </td>
      <td>
        0.11
      </td>
      <td>
        0.36
      </td>
      <td>
        0.05
      </td>
    </tr>
    <tr>
      <td>
        Sr-
      </td>
      <td>
        2
      </td>
      <td>
        0.03
      </td>
      <td>
        0.17
      </td>
      <td>
        0.02
      </td>
    </tr>
    <tr>
      <td>
        Positive Punisher
      </td>
      <td>
        9
      </td>
      <td>
        0.14
      </td>
      <td>
        0.40
      </td>
      <td>
        0.05
      </td>
    </tr>
    <tr>
      <td>
        Negative Punisher
      </td>
      <td>
        3
      </td>
      <td>
        0.04
      </td>
      <td>
        0.21
      </td>
      <td>
        0.03
      </td>
    </tr>
    <tr>
      <td>
        Non-Response
      </td>
      <td>
        2
      </td>
      <td>
        0.03
      </td>
      <td>
        0.25
      </td>
      <td>
        0.03
      </td>
    </tr>
    <tr>
      <td>
        Delta Extinction
      </td>
      <td>
        4
      </td>
      <td>
        0.06
      </td>
      <td>
        0.40
      </td>
      <td>
        0.05
      </td>
    </tr>
    <tr>
      <td>
        Unclassifiable Consequence
      </td>
      <td>
        8
      </td>
      <td>
        0.13
      </td>
      <td>
        0.38
      </td>
      <td>
        0.05
      </td>
    </tr>
    <tr>
      <td>
        <b>Behavioural Dimensions</b>
      </td>
      <td colspan="4">
      </td>
    </tr>
    <tr>
      <td>
        Time
      </td>
      <td>
        66
      </td>
      <td>
        1.05
      </td>
      <td>
        1.37
      </td>
      <td>
        0.17
      </td>
    </tr>
    <tr>
      <td>
        Quantifier
      </td>
      <td>
        17
      </td>
      <td>
        0.27
      </td>
      <td>
        0.63
      </td>
      <td>
        0.08
      </td>
    </tr>
    <tr>
      <td>
        <b>Other</b>
      </td>
      <td colspan="4">
      </td>
    </tr>
    <tr>
      <td>
        Mentalism
      </td>
      <td>
        112
      </td>
      <td>
        1.78
      </td>
      <td>
        1.73
      </td>
      <td>
        0.22
      </td>
    </tr>
    <tr>
      <td>
        <b>Total</b>
      </td>
      <td>
        1698
      </td>
      <td>
        3.37
      </td>
      <td>
        4.40
      </td>
      <td>
        0.20
      </td>
    </tr>
  </tbody>
</table>

## Doctoral Project

// TODO: Finish section.

## Document types

// TODO: Finish section.

## Annotation system

// TODO: Finish section.

# References
[1] B. F. Skinner, *Science and Human Behavior.* Macmillan.

[2] B. F. Skinner, *Verbal Behavior.* Appleton-Century-Crofts.

[3] J. O. Cooper, T. E. Heron, and W. L. Heward, *Applied Behavior Analysis: Pearson New International Edition PDF eBook.* Pearson Education.

[4] “Beautiful Soup Documentation — Beautiful Soup 4.9.0 documentation.” [Online]. Available: https://www.crummy.com/software/BeautifulSoup/bs4/doc/

[5] “We planned to have sex – then my new boyfriend vanished,” the Guardian. [Online]. Available: http://www.theguardian.com/lifeandstyle/2016/aug/14/my-new-boyfriend-has-vanished-mariella-frostrup

[6] H. Nakayama, T. Kubo, J. Kamura, Y. Taniguchi, and X. Liang, “doccano: Text annotation tool for human,” 2018, software available from https://github.com/doccano/doccano. [Online]. Available: https://github.com/doccano/doccano
