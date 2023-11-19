# PoliticalSlant_NewsHeadlinesClassification

News coverage in recent times has become increasingly polarized, and a larger fraction of mentions of political figures in the news are associated with polarized language. This can hamper discussions on contentious social and political issues and further the existing ideological gap among readers. 

We use a previously created dataset of news headlines from major US news publishers. The headlines relate to the 2020 US Presidential elections and mention one of the two major parties' presidential candidates. The dataset contains political news headlines from left-leaning and right-leaning news publishers in the US.

We formalize the task for understanding bias in news headlines as a source prediction problem. Given a news headline, the task is to predict if the headline is published by a left-leaning news publisher or a right-leaning news publisher. Our dataset differs from previous datasets in that each news headline contains an entity mention (the presidential candidate), towards which the bias is to be determined. 

We fine-tune a pre-trained language model (DistilBERT) to identify if a given news headline is from Left or Right. We further conduct an ablation study of the fine-tuned model to better understand the differences in news coverage between Left and Right. We also use Integrated Gradient (IG) to compute attributions for each text feature contributing to the predictions, thus improving model interpretability. 

This is an ongoing project. It consists of the following files:

1. Classification of Left and Right Leaning News Headlines by Fine-Tuning a BERT model. [Fine-Tuning BERT](https://github.com/saxenamansi/PoliticalSlant_NewsHeadlinesClassification/blob/main/FineTuningDistilBERT.ipynb)
2. Obtaining Word Attributions (Unigram, Bigram, Trigram) for each word using Integrated Gradients to improve model interpretability. [WordAttributions]()
3. Analysing Unigram Attributions [UnigramAnalysis]()
4. Analysing Bigram Attributions [BigramAnalysis]()
5. Analysing Trigram Attributions [TrigramAnalysis]()
