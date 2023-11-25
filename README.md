# T5-summarization
## Introduction
Abstractive summarization is a type of text summarization where the summary is not simply a selection of existing sentences from the original text but is generated in a more creative way. 
In abstractive summarization, the system interprets and understands the content of the source text and then formulates a summary using its own words, potentially introducing new phrases and sentence structures that were not present in the original text.
This approach contrasts with extractive summarization, where the summary is created by selecting and arranging existing sentences or passages from the source text. 
Abstractive summarization aims to produce more human-like and coherent summaries, often requiring natural language generation techniques.
!DEMO (summarization.png)
This repo show how to fine-tune the model for abstractive summarization task with T5 
## Dataset
VietNews : https://github.com/ThanhChinhBK/vietnews
!DEMO (data.png)
## Metrics
ROUGE (Recall-Oriented Understudy for Gisting Evaluation) is a set of metrics commonly used for the automatic evaluation of machine-generated text, particularly in the context of text summarization. 
These metrics assess the quality of a summary by comparing it to one or more reference (human-generated) summaries.
!DEMO (rouge.png)
The main ROUGE metrics include:

- ROUGE-N (N-gram Overlap): Measures the overlap of n-grams (contiguous sequences of n items, usually words) between the system-generated summary and the reference summaries. ROUGE-N includes various variations like ROUGE-1 (unigrams), ROUGE-2 (bigrams), and ROUGE-3 (trigrams).

- ROUGE-L (Longest Common Subsequence): Measures the longest common subsequence of words between the system summary and reference summaries. It considers word sequences rather than just n-grams, providing a more global measure of content overlap.
In this task we just use **Rouge-1**, **Rouge-2** and **Rouge-L**

## Result
Result after training evalue by ROUGE Metrics

!DEMO (benchmark.png)
