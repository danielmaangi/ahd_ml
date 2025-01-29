Advanced HIV Disease (AHD) Prediction using Machine Learning
===============
Overview
--------------
This project applies machine learning techniques to predict Advanced HIV Disease (AHD) in patients based on clinical and demographic data. 
The goal is to develop a predictive model that can assist healthcare professionals in identifying high-risk individuals and optimizing interventions.

Please send a pull request if you find things that belongs to here.

Project Structure
--------
```markdown
|-- ahd_prediction/
    |-- data/              # Directory for raw and processed data (ignored in Git)
    |-- config/            # Configuration files (ignored in Git)
    |-- models/            # Trained models and checkpoints
    |-- notebooks/         # Jupyter notebooks for exploratory data analysis and modeling
    |-- scripts/           # Python scripts for data preprocessing, training, and evaluation
    |-- .gitignore         # Files and directories to ignore in Git
    |-- requirements.txt   # Dependencies for the project
    |-- README.md          # Project documentation
```

Installation
-------------
### 1. Clone the repository
```markdown
git clone https://github.com/danielmaangi/ahd_ml.git
cd ahd_ml
```
### 2. Create a virtual environment
```markdown
python -m venv .venv
source .venv/bin/activate  # On macOS/Linux
.venv\Scripts\activate    # On Windows
```
### 3. Install dependencies
```markdown
pip install -r requirements.txt
```
### Data

- The dataset contains clinical, laboratory, and demographic features used for training the model.
- Due to privacy concerns, raw data is not included in this repository.
- You can preprocess the data using scripts in the scripts/ directory.

## Model Development
### 1. Data Preprocessing
Run the preprocessing script:
```markdown
python scripts/preprocess.py
```

### 2. Train the model
Execute the training script:
```markdown
python scripts/train.py
```

### 3. Evaluate the Model
Execute the training script:
```markdown
python scripts/evaluate.py
```

## Usage
To make predictions using the trained model:
```markdown
python scripts/predict.py --input data/sample_input.csv
```

## Technologies Used

- [Python](https://www.python.org/) (pandas, NumPy, scikit-learn, xgboost)
- [upyter Notebook ](https://github.com/microsoft/FLAML) - for exploratory data analysis
- [Flask/FastAPI](https://flask.palletsprojects.com/en/stable/) - for deploying the model as an API

## Contributors
- [Daniel Maangi](https://github.com/danielmaangi) 
- [Jacques Muthusi](https://github.com/kmuthusi) 

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Healthcare professionals and researchers contributing to HIV/AIDS data and insights.
- Open-source contributors to machine learning frameworks.