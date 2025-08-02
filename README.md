# 🚦 Traffic Sign Classification Using LeNet Architecture

This project implements a Convolutional Neural Network (CNN) using the **LeNet-5 architecture** to classify traffic signs from the German Traffic Sign Recognition Benchmark (GTSRB) dataset.

## 🧠 Model Overview

- **Architecture**: LeNet-5  
- **Framework**: TensorFlow / Keras  
- **Input**: 32x32 grayscale traffic sign images  
- **Output**: 43 classes representing different traffic signs

## 📁 Project Structure

```

Traffic\_Sign\_Classification\_Using\_LeNet\_Architecture/
│
├── traffic-signs-data/
│   ├── train.p
│   ├── test.p
│   └── valid.p
│
├── model.py                 # CNN model definition
├── train.py                 # Training script
├── evaluate.py              # Evaluation and predictions
├── README.md                # Project description
└── requirements.txt         # Dependencies

````

## 📦 Requirements

Install the dependencies:

```bash
pip install -r requirements.txt
````

Or manually install:

```bash
pip install tensorflow keras numpy matplotlib scikit-learn
```

## 🏗️ Model Architecture

```
Input: 32x32x1 grayscale images

1. Conv2D (6 filters, 5x5) + ReLU  
2. AvgPooling2D  
3. Conv2D (16 filters, 5x5) + ReLU  
4. AvgPooling2D  
5. Flatten  
6. Dense (120) + ReLU  
7. Dense (84) + ReLU  
8. Dense (43) + Softmax
```

## 🚀 How to Run

Train the model:

```bash
python train.py
```

Evaluate the model:

```bash
python evaluate.py
```

## 🧪 Dataset

* [German Traffic Sign Recognition Benchmark (GTSRB)](https://benchmark.ini.rub.de/?section=gtsrb&subsection=news)
* Pickled files used: `train.p`, `valid.p`, `test.p` (each contains features and labels)

## 📊 Results

* **Accuracy**: \~98% on validation set (with grayscale normalization)
* **Loss Function**: `sparse_categorical_crossentropy`
* **Optimizer**: Adam

## 📝 License

This project is licensed under the [MIT License](LICENSE).

## 👨‍💻 Author

[Sai Vamshi Burugu](https://github.com/SaiVamshiBurugu)
