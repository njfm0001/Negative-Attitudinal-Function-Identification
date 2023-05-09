# Communicative function identification (WIP)
## Introduction
Communicative function identification is presented as a new NLP task for the classification of communicative functions from text messages (Fernández-Martínez, 2023). Thus, this is a sequence classification task. Unlike emotion detection and dialog act classification, which focus on the identification of emotions and generic speech acts, respectively, this task encompasses the identification of expressions of different types of socio-cognitive phenomena: the expression of emotion, feeling, intent, judgement, mood, argument, etc.

The notion of communicative function comes from the foreign language learning and teaching literature; specifically, it comes from the communicative approach in English as a Foreign Language (EFL) (Finocchiaro & Brumfit, 1983). A communicative function is defined as a communicative act or the use of linguistic utterances for a given purpose or intention, typically to express the speaker's emotion or attitude (Milanovic & Saville, 2012).

## Datasets
Due to the different taxonomies found in the literature, we decided to focus on the one presented by Blundel et al. (1982), a practical EFL coursebook that contains a wide range of attitudinal, informative, and active communicative functions. From this, we obtained a basic taxonomy of 18 negative communicative functions related to the attitudinal category.

On the basis of this, we built two synthetic datasets: a basic dataset of constructions and an extended one of social media microtexts synthethically generated with ChatGPT using prompt engineering. The datasets will be made publicly available in this repository.

## Evaluation
We evaluated the usefulness and validity of these datasets with state-of-the-art emotion-detection datasets of tweets (i.e. EmoEvent, GoEmotions, CARER, AIT) that were automatically mapped to the communicative function categories of our taxonomy. The corresponding mapping was not perfect, but useful enough for our purposes. For details about the emotion-detection datasets used, including the files themselves, we refer the readers to the original papers. 

The experiments that were carried out for each dataset, including each of the supervised approaches (Naïve Bayes, fine-tuning, semantic similarity through contextualized sentence embeddings, zero-shot classification through Natural Language Inference) will be made publicly available in this repository.

## Additional information
Further details about this task, dataset creation, mapping, experimental setup, evaluation, results, discussion, error analysis, and limitations can be found in the original paper in Fernández-Martínez (2023).

## Funding
Financial support for this research has been provided under grant PID2020-112827GB-I00, funded by the Spanish Ministry of Science and Innovation MCIN/AEI/10.13039/501100011033, and grant number 101017861[project SMARTLAGOON] funded by the European Union's Horizon 2020 research and innovation program

## References

- Blundell, Jon, Higgens, Jonathan, & Middlemiss, Nigel. (1982). *Function in English*. Oxford University Press.
- Fernández-Martínez, N.J. (2023). Introducing Communicative Function Identification as a new NLP task. Unpublished manuscript.
- Finocchiaro, M., & Brumfit, C. (1983). *The functional-notional approach: from theory to practice*. Oxford University Press.
- Milanovic, Michael, & Saville, Nick. (2012). The Theoretical Foundations for functions in the Council of Europe modern languages projects and the Common European Framework of Reference for languages. In *Language Functions Revisited*. Cambridge University Press. Retrieved from www.cambridge.org
