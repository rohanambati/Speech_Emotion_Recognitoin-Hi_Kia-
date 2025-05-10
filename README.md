````markdown
# Speech Emotion Recognition – Hi_Kia

This repo presents **Speech Emotion Recognition** on the **hi_kia** wake-up-word dataset. It extracts rich audio features and trains an **XGBoost** model tuned via **GridSearchCV**. A Gradio demo lets you predict emotions from speech in real time.

## Table of Contents

* [Built With](#built-with)  
* [Getting Started](#getting-started)  
  * [Prerequisites](#prerequisites)  
  * [Installation](#installation)  
* [Usage](#usage)  
* [Demo](#demo)  
* [Features](#features)  
* [Contributing](#contributing)  
* [License](#license)  
* [Acknowledgements](#acknowledgements)  

## Built With

* **Python 3.8+**  
* **librosa** for audio feature extraction  
* **scikit-learn** & **XGBoost** for modeling  
* **pandas**, **NumPy** for data handling  
* **Gradio** for the web demo  
* **matplotlib**, **plotly** for visualizations  

## Getting Started

### Prerequisites

* Python 3.8 or higher  
* `pip` package manager  

### Installation

1. **Clone** the repo:  
   ```bash
   git clone https://github.com/rohanambati/Speech_Emotion_Recognition-Hi_Kia-.git
````

2. **Enter** the directory:

   ```bash
   cd Speech_Emotion_Recognition-Hi_Kia-
   ```
3. **Install** dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Explore the Notebook**

   * Open `nlpprojectfinal_cleaned_f.ipynb` in Jupyter or Colab.
   * Follow the steps: data prep → feature extraction → model tuning → evaluation.

2. **Run the Demo**

   ```bash
   cd app
   python app.py
   ```

   * Visit the local Gradio link.
   * Upload a `.wav` clip.
   * Instantly see the predicted emotion.

## Demo

![Gradio Demo Screenshot](assets/demo_screenshot.png)
*An interactive interface for real-time emotion prediction* ([View on GitHub](https://github.com/rohanambati/Speech_Emotion_Recognition-Hi_Kia-))

## Features

* **Rich Audio Features**: MFCCs, deltas, chroma, spectral contrast, zero-crossing rate, RMS.
* **Robust Classification**: XGBoost tuned with stratified cross-validation.
* **Comprehensive Metrics**: Accuracy, precision, recall, F1, ROC & PR curves.
* **Embedding Visualizations**: t-SNE & PCA projections.
* **Live Web Demo**: Simple Gradio interface for instant feedback.

## Contributing

Contributions welcome!

1. Fork the repo
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m "Add feature"`)
4. Push to your branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

Distributed under the **MIT License**. See `LICENSE` for details.

## Acknowledgements

* **Best-README-Template** by othneildrew for the structure
* **Awesome README** curated list for inspiration
* Tom Preston-Werner’s “Write Your README First” best practice

```
```
