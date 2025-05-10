# Speech Emotion Recognition – Hi_Kia

This repository presents **Speech Emotion Recognition** on the **hi_kia** wake-up-word dataset. It extracts rich audio features and trains an **XGBoost** model tuned via **GridSearchCV**. You can run the notebook or load the pre-trained model from `models/`.

## Table of Contents

- [Built With](#built-with)  
- [Getting Started](#getting-started)  
  - [Prerequisites](#prerequisites)  
  - [Installation](#installation)  
- [Usage](#usage)  
- [Models](#models)  
- [Contributing](#contributing)  
- [License](#license)  
- [Acknowledgements](#acknowledgements)  

## Built With

- Python 3.8+  
- librosa  
- scikit-learn & XGBoost  
- pandas, NumPy  
- gradio (for demo)  
- matplotlib  

## Getting Started

### Prerequisites

- Python 3.8 or higher  
- pip  

### Installation

~~~bash
git clone https://github.com/rohanambati/Speech_Emotion_Recognition-Hi_Kia-.git
cd Speech_Emotion_Recognition-Hi_Kia-
pip install -r requirements.txt
~~~

## Usage

1. **Run the Notebook**

   ~~~bash
   jupyter notebook SER_Hi_Kia_RohanAmbati.ipynb
   ~~~

2. **(Optional) Launch the Web Demo**

   ~~~bash
   cd app
   python app.py
   ~~~

## Models

The pre-trained scaler and XGBoost model are in the `models/` directory:

~~~python
import pickle

with open('models/scaler.pkl', 'rb') as f:
    scaler = pickle.load(f)
with open('models/model.pkl', 'rb') as f:
    model = pickle.load(f)
~~~

## Contributing

Contributions are welcome! Fork the repo and submit a pull request.

## License

Distributed under the **MIT License**. See `LICENSE` for details.

## Acknowledgements

- **hi_kia 1.0** dataset on Zenodo: https://zenodo.org/records/7091465  
- **Best-README-Template** by othneildrew  
