# EoinClaw.ai

Does data augmentation improve generalization when data is scarce?

## Prerequisites

- Python 3.10 or newer
- Git

## Setup

1. Clone the repository and move into it:

```bash
git clone <repo-url>
cd EoinClaw.ai
```

2. Create and activate venv:

```bash
python -m venv .venv
source .venv/bin/activate        # macOS / Linux
.venv\Scripts\activate           # Windows
```

3. Install the dependencies:

```bash
pip install -r requirements.txt
```

4. Download the dataset from
   https://www.kaggle.com/datasets/balabaskar/tom-and-jerry-image-classification
   and unzip it into a `TomJerry` folder at the repository root, so the images end up at:

```
TomJerry/tom_and_jerry/tom_and_jerry/
```

5. Open `preprocessing.ipynb`, select the `.venv` kernel, and choose **Run All**.
6. Open `training.ipynb`, select the `.venv` kernel, and choose **Run All**.
7. Open `analysis.ipynb`, select the `.venv` kernel, and choose **Run All**.

## Notes

- The dataset is not committed to the repository. Each person downloads it locally.
- Seeds are set in the Settings cell of the notebook, for reproducibility.
