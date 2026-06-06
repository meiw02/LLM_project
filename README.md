## Course
IMT 526 Final Project
# LLM Project

A machine learning project using QLoRA fine-tuning to classify/analyze text data.

# Project Structure
```
LLM_project/
├── data/              # Raw and processed datasets
├── outputs/           # Model predictions and evaluation results and labeled test data
├── checkpoints/       # Saved model checkpoints
├── notebooks/         # Jupyter notebooks
└── README.md
```

## Setup
Clone the repository:
git clone https://github.com/meiw02/LLM_project.git
cd LLM_project

Install dependencies:
pip install -r requirements.txt

## Usage
Open and run the notebook:
notebooks/project.ipynb

## Data
- `train_data.csv` — training dataset
- `val_data.csv` — validation dataset
- `test.csv` — test dataset
- `test_labels.csv` - labels for the test data; value of -1 indicates it was not used for scoring

## Models Compared
- TF-IDF + Logistic Regression (baseline)
- Zero-shot Llama 3.1 8B
- QLoRA Fine-tuned Llama 3.1 8B

## Results
| Model | Macro F1 | Toxic F1 | Toxic Precision | Toxic Recall |
|---|---|---|---|---|
| TF-IDF + Logistic Regression | 0.778 | 0.618 | 0.478 | 0.874 |
| Zero-shot Llama 3.1 8B | 0.696 | 0.490 | 0.352 | 0.809 |
| QLoRA Fine-tuned Llama 3.1 8B | 0.707 | 0.514 | 0.361 | 0.880 |

## Key Findings
- QLoRA achieved the highest Toxic Recall (0.880)
- TF-IDF baseline had the strongest overall Macro F1 (0.778)

## Authors
- Mei Wu 
- Vivien Wang
- Terresa Tran

## Acknowledgments
Built with QLoRA and LLama and George Harker and Tunir Mitra 
