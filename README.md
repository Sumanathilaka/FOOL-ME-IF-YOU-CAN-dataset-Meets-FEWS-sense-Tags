# The Final Dataset 
This version of the dataset contains the FOOLMEIFYOUCAN dataset mapped with the FEWS sense Tags.
You can access original papers from here.

https://aclanthology.org/2024.emnlp-main.290/
https://nlp.cs.washington.edu/fews/


## WSD_1 and WSD_train
-  includes sentences with unambiguous context.
-  Example: "Apple revolutionized the technology industry with its innovative products like the iPhone and MacBook ." 
- the homonym "Apple" should be easily disambiguated

## WSD_2:
- includes sentences with unambiguous context + an adjective that supports and suits the homonyms intended meaning in that context
- Example: "trendsetting Apple revolutionized the technology industry with its innovative products like the iPhone and MacBook ."
- the homonym "Apple" should be easily disambiguated

## WSD_3:
- includes sentences with ambiguous context since it includes an adjective that does NOT suit or support the intended meaning of the homonym in that sentences; the adjective suits another meaning 
- Example: "fresh Apple revolutionized the technology industry with its innovative products like the iPhone and MacBook ."
- the homonym "Apple" should be harder to disambiguate

## WSD_4:
- includes sentences with ambiguous context since it contains another noun that is typically used in the context of the opposing meaning of the homonym 
- Example: "Apple offers juice to all employees ."
- the homonym "Apple" should be harder to disambiguate 


