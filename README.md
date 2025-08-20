✋ Hand Gesture Recognition System
---

A real-time hand gesture recognition system powered by OpenCV, cvzone, and TensorFlow.

This project captures hand gestures through your webcam and classifies them into predefined categories (like A, B, C).

🌟 Features
---

🖐️ Real-time hand detection using cvzone.HandTrackingModule

✂️ Automatic preprocessing (cropping, resizing, white background adjustment)

🔍 CNN-based classification with DepthwiseConv2D

📸 Built-in data collection for training your own custom gestures

🧠 Customizable labels (A, B, C, etc.) – retrain easily with your own data

🛠 Tech Stack
---
Component	Library / Tool

Hand Detection	cvzone.HandTrackingModule

Model Framework	TensorFlow, Keras


Image Processing	OpenCV, NumPy
Classifier	cvzone.ClassificationModule
IDE (Optional)	VS Code, Jupyter

📂 Folder Structure
---
```bash

Hand-Gesture-Recognition/
├── Data/
├── Model/
│   ├── keras_model.h5
│   └── labels.txt
├── dataCollection.py
├── test.py
├── requirements.txt
└── README.md
```
🔧 Setup Instructions (Local)
--
Clone the repository
```bash
git clone https://github.com/your-username/Hand-Gesture-Recognition.git
cd Hand-Gesture-Recognition
```
Create a virtual environment
---
```bash
python -m venv venv
```
Activate the environment
---
Windows:
```bash
venv\Scripts\activate
```
Linux/Mac:
```bash
source venv/bin/activate
```
Install dependencies
---
```bash
pip install -r requirements.txt
```
📸 Collect Your Own Gesture Data
---
Run the data collection script:
```bash
python dataCollection.py
```
Your webcam will open.

Show a gesture to the camera.

Press s to save a cropped + resized image into the Data/ folder.

🖥️ Run the Gesture Recognition App
---
Once you’ve collected data and trained the model:
```bash
python test.py
```
This will:
✅ Open webcam

✅ Detect your hand

✅ Predict gestures in real-time

🧠 Model Details
---

Model File: Model/keras_model.h5

Labels File: Model/labels.txt

Example Labels
labels = ["A", "B", "C"]


Add your own gestures, retrain the model, and update labels.txt.

✅ Best Practices
---

Keep large datasets & trained models in external storage (not in GitHub repo).

Use a .gitignore to exclude unnecessary files (.venv/, __pycache__/, *.h5, etc.).

Separate training scripts if you plan to experiment with different architectures.

🚀 Future Improvements
---

Extend to full ASL Alphabet recognition.

Deploy as a mobile app with TensorFlow Lite.

Add support for gesture-controlled applications (games, IoT, smart devices).

👩‍💻 Author
---

📧allupragathi@gmail.com
