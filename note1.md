# Measuring similarity of sentential arguments
###
* **Facet**: frequently paraphrased propositions, or labels capturing the essence of one particular aspect of an argument.

* **Steps**:
  * extract sentences thata express an argument from raw social media dialogs
  * rank the extracted arguments in terms of their similarity to one another
  
* sets of similar arguments are used to represent argument facets

## Introduction

* dialog excerpts from the 89K sentences about gun control in the IAC 2.0 (Annptt et al. 2016)
* aim: induce and identify facets of an argument across multiple conversations and produce summaries of all the different facets automatically
* to simplify the problem: focus on **SENTENTIAL ARGUMENTS**, 
single sentences that clearly express a particular argument facet in dialog.
    * aim: to use SENTENTIAL ARGUMENTS to produce current social and political topics.

* goals:
    * Task1: **Argument Extraction** how can we extract sentences from dialog that clearly express a particular argument facet?
    * Task2: **Argument Facet Similarity** How can we recognize that two sentential arguments are semantically similar, that they are
    different linguistic realizations of the same facet of the argument?

### AFS (Argument Facet Similarity)
* in previous work, we developed an AFS regressor for predicting the similarity of **human-generated labels** for summaries of dialogic arguments.
* collect 5 human summaries of each dialog, and then use the Pyramid tool and scheme to annotate sentences from these summaries as contributors to (paraphrase of) a particular facet.


## Corpora and Problem Definition
* aim :  produce summaries similar to thse curated summaries, but automatically, and over time, 
    so that as new argument facets arise for a particular topic, we can identify them.
   
* first, create a large sample of high quality sentential arguments
* create a large sample of paired sentential arguments in order to train the model for AFS

### argument quality data
extract all the sentences for all of the posts in each topic to first create a large corpus of topic sorted sentences

* AQ score for each sentence.   
    * reflect how easily the speaker's argument can be understood from the sentence without any context.
    * 0.0 to 1.0
    * easily understandable sentences are assumed to be prime candidates for producing extractive summaries.

many sentences given high AQ scores were very similar, while 
we need a sample that realizes many diverse facets.

then we found that some extracted sentential aruments were not actually high quality.

## Argument Facet Similarity
 
 
 ## Future work
 ROUGE performed very well ,
 suggesting that other machine translation metrics such as Terp
 and Meteor may be useful.
 
 use AFS regressor to cluster and group similar arguments and produce 
 __argument facet summaries__ 
 