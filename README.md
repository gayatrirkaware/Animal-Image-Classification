# 🐾 15-Class Animal Image Classifier Web App

This is a Flask-based web application that uses a trained **MobileNet** deep learning model to classify images of animals into one of 15 predefined categories. Users can upload an image and receive a prediction along with confidence scores for all classes. Predictions are stored in **MongoDB** for record-keeping.

---

## 🧠 Model Details

- Model: `MobileNet_best_tuned_model.h5`
- Classes:  
  `"Bear", "Bird", "Cat", "Cow", "Deer", "Dog", "Dolphin", "Elephant", "Giraffe", "Horse", "Kangaroo", "Lion", "Panda", "Tiger", "Zebra"`
- Input Shape: 224x224 RGB images
- Output: Single-label classification with confidence

---

## 🗂️ Project Structure

.
├── app.py # Main Flask app
├── model/
│ └── MobileNet_best_tuned_model.h5 # Trained model
├── templates/
│ └── index.html # Upload form (optional UI)
├── static/ # Optional for CSS/JS
├── requirements.txt # Project dependencies
└── README.md # This file


---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/animal-classifier-app.git
cd animal-classifier-app
```

### 2. Create a Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash 
pip install -r requirements.txt
```
Sample requirements.txt:
Flask
numpy
opencv-python
tensorflow
pymongo


### Run the App
Make sure MongoDB is running:
```bash
mongod --dbpath "C:/data/db"  # Adjust path as needed
```

Then run the Flask app:
```bash
python app.py
```
Access it at: http://127.0.0.1:5000