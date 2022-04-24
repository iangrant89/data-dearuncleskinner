# Dataset from Dear Uncle Skinner Project
## Introduction
This repository contains the annotated datasets from my MSc Project and will later host the fully annotated dataset of agony aunt letters according to verbal behaviour theory from my PhD project. To find out more about my project please visit the project website [here](https://dear-uncle-skinner.ch). Website is currently in development.

## Original Dataset
The original MSc Dataset was used to create a predictive model which aimed to predict the subject of a text, the behaviour of concern and predict a behaviour analyst's initial hypothesis about the probable function of the behaviour. The dataset is the first known dataset of its type used to make hypothetical predictions about behavioural function. The dataset will be regularly updated, when further documents are annotated.

The documents consist of an unstructured corpus which aims to be somewhat reflective of the typical interactions between practitioners and service users. Additionally, in order to train the model a significant dataset is be required. The documents were scrapped from a public source of agony aunt letters. These letter share some of the same lexical, syntactical and grammatical properties of texts encountered by behavioural analytical practitioners in digital communications mediums such as E-Mails, especially in the initial stages of a therapy. In order to obtain this data a web-scrapping programme was used pull the texts of the Guardian Dear Mariella page. The programme successfully extracted 813 documents. The documents were then multiplied by four to ensure that each identified subject could be annotated as the main subject at least once. Due to
formatting changes on the guardian website overtime, addition text such as replies was also unintentionally extracted. In order to remove any interpretation bias brought about by the agony aunt responses, the replies were removed prior to annotation.

In order to collate the agony aunt letters and build the data set, the python module Beautiful Soup was used. All scripts were completed in the Jupyter Lab IDE. The data was annotated using the software doccano. Doccando provides researchers the possibility to easily complete sequence analysis within a user friendly user interface (UI). The software is created and written in python and provides an API to import data automatically via Jupyter Lab. However, the original UIs simplicity constrains its functionality and it was originally not possible to support nested annotation without making significant changes. As such this was one of the reasons the document were copied four times. As is allowed for at least 4 iterations of annotations in relation to different behavioural subjects (see Targets).

Recent changes to Doccano allow for relational and nested tagging. As such alleviating the need for the duplication of documents.

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
- SR+:
- Sr+:
- Sr-:
- Positive Punisher:
- Negative Punisher:
- Non-Response:
- Delta Extinction:
- Unclassifiable Consequence:

**Behavioural Dimension**
- Time:
- Quantifier:

**Other**
- Mentalism:

## Descriptive Statics of MSc. Dataset
**Last updated**: 25th April 2022

// TODO: Finish section.

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
    </tr>
    <tr>
      <td>
        Alternative Target 1
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
[] B. F. Skinner, *Verbal Behavior.* Appleton-Century-Crofts.

[] B. F. Skinner, *Science and Human Behavior.* Macmillan.

[] J. O. Cooper, T. E. Heron, and W. L. Heward, *Applied Behavior Analysis: Pearson New International Edition PDF eBook.* Pearson Education.

[] “We planned to have sex – then my new boyfriend vanished,” the Guardian. [Online]. Available: http://www.theguardian.com/lifeandstyle/2016/aug/14/my-new-boyfriend-has-vanished-mariella-frostrup

[] “Beautiful Soup Documentation — Beautiful Soup 4.9.0 documentation.” [Online]. Available: https://www.crummy.com/software/BeautifulSoup/bs4/doc/

[] H. Nakayama, T. Kubo, J. Kamura, Y. Taniguchi, and X. Liang, “doccano: Text annotation tool for human,” 2018, software available from https://github.com/doccano/doccano. [Online]. Available: https://github.com/doccano/doccano
