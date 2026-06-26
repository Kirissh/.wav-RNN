# RNN Speech Command Classifier

Bidirectional GRU that classifies short audio clips (`go`, `yes`, `no`) using MFCC features from the [Google Speech Commands](https://www.tensorflow.org/datasets/catalog/speech_commands) dataset.

## Setup

```bash
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## Run

```bash
python app.py
```

On first run, the dataset is downloaded into `data/`. Training saves `model.pt` and writes `predictions.csv` if `student_test_features.pt` is in the project folder.
