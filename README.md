# Negative Attitudinal Function Identification
This repository contains the data and code for the identification of **Negative Attitudinal Functions** in text, a task designed for Smart City applications. This research has evolved in two main phases.

## 1. Initial Research: Basic Synthetic Dataset (2024)
This phase introduced the task and a **Basic Corpus** consisting of 902 synthetic constructions derived from English as a Foreign Language (EFL) resources (Fernández-Martínez, 2024a). 

*   **Dataset:** `Data/comfunct_basic.txt`.
*   **Experiments:** Models (NB, DistilBERT, Meta-embeddings) were trained on the basic corpus and evaluated against external emotion detection datasets (EmoEvent, GoEmotions, CARER, AIT) mapped to my taxonomy (Fernández-Martínez, 2024b).
*   **Location:** `Experiments/2024_Basic_Research/`.

## 2. Advanced Research: LLM-Assisted Extended Corpus (2026)
This phase leverages Large Language Models (ChatGPT, Copilot, Gemini, Mixtral, and OpenChat) and **few-shot prompting** to generate a balanced dataset of 4,500 informal tweets (250 per category) (Fernández-Martínez, 2026).

*   **Dataset:** `Data/extended_synthetic_corpus/`.
*   **Experiments:**
    *   **Experiment I:** Training and testing on the extended corpus (Achieved **0.83 accuracy** with DistilBERT).
    *   **Experiment II:** Cross-corpus evaluation (Basic vs. Extended).
    *   **Experiment III:** Zero-shot NLI classification.
*   **Location:** `Experiments/2026_LLM_Research/`.

## Taxonomy
I identify **18 negative attitudinal functions** relevant to detecting citizen dissatisfaction (e.g., complaints, distrust, pessimism):
*PESSIMISTIC, WORRIED, ANGRY, DISAPPOINTED, BORED, DISLIKE, NOT_APPROVE, NOT_IMPORTANT, NOT_INTERESTED, DISAGREE, NOT_CORRECT, WARN, COMPLAIN, THREATEN, UNWILLING, REFUSE, DISTRUST, and OTHER* [14].

## Funding
*   **Project SMARTLAGOON** (Horizon 2020, grant 101017861)
*   **Project PID2023-147137NB-I00**, funded by MICIU/AEI/10.13039/501100011033 and by ERDF, EU [15].

## References
*   Fernández-Martínez, N.J. (2024a) Taxonomía de funciones comunicativas negativas para su identificación automática en el contexto de las ciudades inteligentes. En F. Olmo-Cazevieille (Ed.) *Investigación lingüística en entornos digitales*. Valencia: Tirant Lo Blanch.
*   Fernández-Martínez, N.J. (2024b). Introducing the NLP task of negative attitudinal function identification. *Procesamiento del Lenguaje Natural*, 52: 57-71.
*   Fernández-Martínez, N.J. (2026). *LLM-assisted Corpus Building and Annotation: Building a Synthetically Generated Corpus of Tweets with Negative Attitudinal Functions for Smart City Applications* (Forthcoming).
