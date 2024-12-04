# BERT-Plot-Analysis
## Description
This research **compares the performance** of different versions of BERT-based (Bidirectional Encoder Representations from Transformers) language models on question-answering tasks related to stories written by Sir Arthur Conan Doyle. 

We perform one-shot testing on **BERT, RoBERTa, and SpanBERT models** to understand how all three models work and why they differ. We ask questions of varying difficulty levels to find the extent to which these models can comprehend and answer them. 

We observed that the **RoBERTa** models were the best compared to BERT and SpanBERT. To gauge performance, we eyeballed the answers and determined them correct/incorrect via a test bank of answers. These graphs are generated via another script in this project's zip file.

## Workflow
![BERT plot analysis workflow](https://github.com/user-attachments/assets/3377ddce-7606-4930-a7bd-68868cafbc1d)

### Models
- BERT:
    - bert-base-uncased
    - bert-base-cased
- SpanBERT:
    - spanbert-base-cased
    - spanbert-large-uncased
- RoBERTa:
    - oberta-base-squad2
    - roberta-large-squad2
    - tinyroberta-squad2
    - roberta-base-squad2-distilled

## Observation
* **BERT** is severely under-trained but was meant to be a generalizable model that can easily be fine-tuned to certain tasks - given parts of words, single words & sentences, etc.
* **SpanBERT** was not even close to the correct answer - gave long sentences with punctuation.
* Overall, **RoBERTa** worked the best with the lower-level questions - comprehension achieved
* All models incorrectly answered complicated questions.

## Related Works
* **BERT**: https://arxiv.org/pdf/1810.04805
* **SpanBERT**: https://arxiv.org/pdf/1907.10529
* **RoBERTa**: https://arxiv.org/pdf/1907.11692
