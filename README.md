# Reddit Depression Detection Final Project CSCI 1460

This project analyzes mental health discourse on Reddit to identify and predict 10 distinct symptoms of depression using advanced Natural Language Processing (NLP) techniques. It serves as a simplified reimplementation of the study [Detecting Symptoms of Depression on Reddit](https://dl.acm.org/doi/abs/10.1145/3578503.3583621). The project compares the performance of topic modeling (LDA) and transformer-based embeddings (DistilRoBERTa) in symptom prediction. It features a complete pipeline for data preprocessing, feature extraction, and classification.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install packages (keep in mind this was produced in a google notebook.

```bash
!pip install happiestfuntokenizing
!pip install transformers torch
```

## Usage


1. Download the notebook.
2. Download *student.pkl*. 
2. OPTIONAL- Download *lda_feature_embeddings.pkl* and *roberta_batch_embeddings.pkl*
2. Download the [data here](https://drive.google.com/drive/folders/1Ln1gkniXNicOSv_n9h4I8XDDXAgaJjq6?usp=sharing)

### With all optional pkl files downloaded (Run's faster):
1. Run all the previous cells before main() 
#### (EXCLUDING THOSE THAT HAVE 'TEST' or 'DOWNLOAD' as the first comment)
2. Adjust all the file paths shown below.

```python
# ADJUST FILE PATHS
FILEPATH = '/content/student.pkl'
ROBERTA_FILEPATH = '/content/roberta_batch_embeddings.pkl'
LDA_FILEPATH = '/content/lda_feature_embeddings.pkl'
```
3. Call main with load_data as True:

```python
main(load_data=True)
```

### Without all pkl files downloaded:
1. Run all the previous cells before main() 
#### (EXCLUDING THOSE THAT HAVE 'TEST' or 'DOWNLOAD' as the first comment)
2. Adjust all the file paths shown below.

```python
# ADJUST FILE PATHS
FILEPATH = '/content/student.pkl'
```
3. Call main with load_data as False:

```python
main(load_data=False)
```
## Final Project Video
[Julien Ward CSCI 1470 Final Project Video](https://drive.google.com/file/d/1zoUl6Qt3wDBZpXtKtoSml7tlCbOD4etM/view?usp=sharing)

(Sorry, I really tried to make the video as short as possible!)