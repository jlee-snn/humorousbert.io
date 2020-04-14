# MIDS UC Berkeley w210: Humorous Bot Study

## Introduction
Given the exponential rate of growth of user created data, it is important to consider ways to automatically detect specific information. Our team is interested in exploring and understanding how specifically humorous content can be detected and created using deep learning based means. Furthermore, our team has shifted focus on understanding the mechanisms of training encoders with humorous text.  The purpose of this project is to build model architecture for detecting humor and examining how encoders such as ALBERT learn humor.


## Objective
Determine how well Natural Language Processing (NLP) can understand humor by: 
1. generating jokes
2. classifying jokes and 
3. by analyzing how the models understand humor 

## Why Humor?
Humor is very contextual and often ambiguous in construction making it harder for a model to understand and predict. This makes it interesting for exploring the boundaries of NLP

## What's new?
Other papers have attempted to understand how well NLP can detect humor by predicting the humor of a joke, but we attempt to take it a step further by generating jokes and analyzing how humor is detected4

## Pipeline Overview


## What Can Bert Tell Us About Humor?
Overall, there is no universally agreed upon theory of humor. 

Two leading theories:
*Benign Violation Theory*: a situation threatens the way that you believe the world “ought” to be but is benign.

*Incongruity Theory*: humour arises when things that do not normally go together replace logic and familiarity.
These theories seem to match how jokes are told (especially puns), but are likely too vague to build a quantitative description of humor

### Other Findings
-We filtered the r/jokes data set through BERT-MNLI (trained on Multi NLI) 
--We found that for 98% of jokes the second half of the joke was neutral or contradictory and only 2% entailment
-Highest rated Reddit jokes - similar overall pattern but still very different:
--Breaking news: Bill Gates has agreed to pay for Trump’s wall …On the condition he gets to install windows
--My girlfriend told me to take the spider out instead of killing it. We went and had some drinks. Cool guy. Wants to be a web developer.	
-Puns seem to have a much more distinctive pattern of word play
--they met in cooking class it was boil meets grill
the violinist spent the night in a vile inn
 Puns
0.934
0.931
N/A
Full Reddit Joke Dataset
0.693
0.724
0.663


## Joke Classification Model Results 

Category | Our Model | Previous Paper | Human
--- | --- | --- | ---
Puns | 0.934 |0.931 | N/A
Full Reddit Joke Dataset | 0.693 |0.724 | 0.663

