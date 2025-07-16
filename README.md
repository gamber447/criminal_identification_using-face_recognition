# 🧠 Face Recognition System using dlib & OpenCV

This project is a **real-time face recognition system** built using Python, OpenCV, and `face_recognition` (which wraps around `dlib`). It captures video from your webcam and detects known faces by comparing them with a preloaded dataset of images.

## 🔍 Features

- Real-time face detection and recognition
- Alerts when a known face is identified
- SMS alert via Twilio (optional)
- Location lookup via IP (optional)

## 🖼 Dataset

The project uses a folder named `Datasets` which contains images of known individuals. Each image should be a clear frontal face image and saved with a recognizable name (e.g., `criminal_test_images.jpg`).

---

## 🛠 Installation

### 📦 Dependencies

Install the following packages using `pip`:

```bash
pip install face_recognition opencv-python numpy twilio
✅ Note: face_recognition depends on dlib. On Windows, installing dlib may require Visual C++ Build Tools. If you face issues, try:

bash
Copy code
pip install cmake
pip install dlib
🔧 Additional Requirements
Python 3.7 - 3.11 recommended

A webcam connected to your computer

🚀 How to Run
Clone the repo or download the project folder.

Make sure your known face images are placed in the Datasets/ directory.

Open the notebook Untitled1.ipynb or run the script file if available.

Run all cells (if using Jupyter Notebook) or execute the Python script:

bash
Copy code
python your_script_name.py
Press q to quit the webcam window.

📂 Folder Structure
Copy code
project-folder/
│
├── Datasets/
│   ├── ganesh_c1.jpg
│   ├── ntr.jpeg
│
├── ganesh_c1.txt
├── veena.txt
├── Untitled1.ipynb
├── README.md
📱 Optional SMS Alert Setup (Twilio)
If you want to enable SMS alerts when a known face is detected:

Create a Twilio account.

Get your ACCOUNT_SID and AUTH_TOKEN.

Replace the placeholder values in the code:

python
Copy code
account_sid = 'YOUR_ACCOUNT_SID'
auth_token = 'YOUR_AUTH_TOKEN'
from_='+1xxxxxxxxxx'
to='+91xxxxxxxxxx'
🔐 Note
This project is for educational/demo purposes only.

Always ensure you have consent when using facial recognition on individuals.
