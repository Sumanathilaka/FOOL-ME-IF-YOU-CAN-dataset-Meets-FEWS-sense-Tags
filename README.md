# Fool me if you can dataset Meets Fews Sense Tag
This dataset version contains the FOOLMEIFYOUCAN dataset mapped with the FEWS sense Tags.
You can access original papers from here.

- FOOLMEIFYOUCAN!AnAdversarialDataset to Investigate the Robustness of LMs in Word Sense Disambiguation
https://aclanthology.org/2024.emnlp-main.290/
- Fews Dataset Paper
https://nlp.cs.washington.edu/fews/

# Proposed approach
- In the shared notebooks, we attempted to use the Fewshot-COT prompting approach with the Fewshot Frequency normalization approach to enrich the inference process with in-context learning.
- mydictionary.json file contains the vectors created for training data based on the tree structure. The parent node is the ambiguous word, while vectors and respective sentences are saved in leaf nodes.
- This structure helps us retrieve semantically similar sentences for a few shot inference processes. Three examples for each case are shared.
   

# Results
We were mainly focusing on uplifting the results of GPT 4o with the WSD 3 dataset, as it is showing clear low results.
We managed to secure the below results using our proposed approach.
- Macro-Averaged F1 Score: 0.8712633249368236
- Micro-Averaged F1 Score: 0.8934290447266704
- Weighted-Averaged F1 Score: 0.8923872663676136


## WSD_1 and WSD_train
-  includes sentences with unambiguous context.
## WSD_2:
- includes sentences with unambiguous context + an adjective that supports and suits the homonyms intended meaning in that context
## WSD_3:
- includes sentences with ambiguous context since it includes an adjective that does NOT suit or support the intended meaning of the homonym in that sentences; the adjective suits another meaning 
## WSD_4:
- includes sentences with ambiguous context since it contains another noun that is typically used in the context of the opposing meaning of the homonym 



