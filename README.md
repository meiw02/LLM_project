IMT 526
# LLM Project

A machine learning project using QLoRA fine-tuning to classify/analyze text data.

# Project Structure
```
LLM_project/
├── data/              # Raw and processed datasets
├── outputs/           # Model predictions and evaluation results
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

## Results
- Best checkpoint saved in `checkpoints/best_qlora_checkpoint`
- Predictions saved in `outputs/qlora_predictions.csv`

## Authors
- Mei Wu 
- Vivien Wang
- Terresa Tran

## Acknowledgments
Built with QLoRA and LLaMA and George Harker and Tunir Mitra 
