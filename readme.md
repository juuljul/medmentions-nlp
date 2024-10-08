# medmentions-nlp

## Description
Ce projet utilise le dataset **MedMentions** pour extraire et classer des **entités biomédicales** à partir de documents médicaux annotés. Le projet repose sur des modèles de machine learning classiques, tels que **Naive Bayes** et **Random Forest**, pour effectuer la **classification** d'entités biomédicales (maladies, syndromes, etc.) en fonction de leurs types sémantiques **UMLS**.

## Fonctionnalités principales
- Extraction des textes (titres et résumés) à partir du dataset **MedMentions** (format PubTator).
- Prétraitement des textes : tokenisation et préparation des caractéristiques pour les modèles de machine learning.
- Classification des entités biomédicales avec les modèles **Naive Bayes** et **Random Forest**.
- Évaluation des performances des modèles à l'aide de métriques classiques (accuracy, précision, rappel, F1-score).

## Technologies utilisées
- **Python 3.11.6**
- **Scikit-learn** pour l'implémentation des algorithmes de classification (Naive Bayes, Random Forest).
- **Pandas** pour la manipulation des données.
- **UMLS** pour l'identification des types sémantiques (T047 pour les maladies, etc.).

## Dataset
Le projet utilise le dataset **MedMentions**, qui contient plus de 4 000 articles de **PubMed** annotés avec des concepts biomédicaux provenant de l'**UMLS** (Unified Medical Language System). Le dataset peut être téléchargé depuis le dépôt GitHub suivant : [MedMentions GitHub](https://github.com/chanzuckerberg/MedMentions).

## Installation

1. **Cloner le repository** :
   ```bash
   git clone https://github.com/juuljul/medmentions-nlp.git
   cd medmentions-nlp

   python3 -m venv env
   source env/bin/activate  # Sur Windows: env\Scripts\activate
   pip install -r requirements.txt
