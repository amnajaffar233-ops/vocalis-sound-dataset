# Vocalis Data Preprocessing Methodology

## 1. Dataset Overview
The Vocalis project uses an audio dataset containing
approximately 2,000 audio files from 50 original sound
categories.

## 2. Binary Classification
To simplify the initial classification task, the original
sound categories are grouped into two classes:

- Target Sound
- Background Sound

The purpose is to distinguish the selected target sounds
from background sounds.

## 3. Feature Extraction
Forty numerical features are extracted from each audio
file to represent its acoustic characteristics.

## 4. Input and Output Variables

### X - Input Features
X contains the extracted numerical features used as input
for model training. The expected shape is (2000, 40),
provided all audio files are processed successfully.

### y - Target Labels
y contains the corresponding class labels for each audio
file: Target Sound or Background Sound.

## 5. Models Evaluated
Three models were evaluated in Jupyter Notebook:

- Support Vector Machine (SVM)
- Random Forest
- Convolutional Neural Network (CNN)

## 6. Initial Results

| Model | Accuracy |
|---|---:|
| SVM | 27% |
| Random Forest | 94.58% |
| CNN | 51% |

Random Forest achieved the highest observed accuracy
in the current experiments.

## 7. Further Validation
The evaluation process should verify the train-test split,
class balance, possible data leakage, and performance
metrics such as precision, recall, and F1-score.

## 8. Current Status
Initial preprocessing and model comparison have been
performed using Jupyter Notebook.
