🖐️ Action Detection for Sign Language
-------------------------------------------------------------------------
This project implements real-time action detection for sign language using deep learning and Mediapipe.
It can recognize hand movements and classify them into different sign language actions (e.g., Hello, Thanks, Yes, No).

-------------------------------------------------------------------------
📂 Project Structure
ActionDetectionforSignLanguage/
│── MP_Data/                  # Dataset (keypoints for training)
│── action.h5                 # Trained deep learning model
│── Action Detection.ipynb    # Jupyter Notebook with implementation
│── README.md                 # Project documentation

-------------------------------------------------------------------------
✨ Features
-------------------------------------------------------------------------
Collects keypoints from hand, body, and face landmarks using Mediapipe.

Trains an LSTM-based deep learning model to detect actions.

Supports real-time sign language action recognition.

Easy to extend for custom datasets and new signs.

-------------------------------------------------------------------------
⚙️ Installation
-------------------------------------------------------------------------
Clone the repo:

      git clone https://github.com/your-username/ActionDetectionforSignLanguage.git
      cd ActionDetectionforSignLanguage

-------------------------------------------------------------------------
Create and activate a virtual environment:
-------------------------------------------------------------------------
    python -m venv venv
    source venv/bin/activate   # On Linux/Mac
    venv\Scripts\activate      # On Windows

-------------------------------------------------------------------------
Install dependencies:
-------------------------------------------------------------------------
    pip install -r requirements.txt

-------------------------------------------------------------------------
⚠️ If requirements.txt is missing, install manually:
-------------------------------------------------------------------------
    pip install mediapipe opencv-python tensorflow numpy matplotlib
-------------------------------------------------------------------------
📊 Dataset
-------------------------------------------------------------------------
The dataset is stored in the folder MP_Data/.

It contains landmark data (collected using Mediapipe) for each action.

You can add new actions by collecting more data with the notebook.

-------------------------------------------------------------------------
🚀 Usage
1️⃣ Train the Model
-------------------------------------------------------------------------
Open the Jupyter notebook:

jupyter notebook "Action Detection.ipynb"


Follow the steps to:

Collect data (keypoints for actions).

Train the LSTM model.

Save the trained model as action.h5.

-------------------------------------------------------------------------
2️⃣ Run Real-Time Detection
-------------------------------------------------------------------------
Once trained, you can use your webcam to test:

python run_realtime.py   # (Create script to load model + run detection)

📈 Results
-------------------------------------------------------------------------
The trained model achieves good accuracy on common actions like:

Hello 👋

Thanks 🙏

i love you <img width="1924" height="1084" alt="Screenshot 2025-08-26 005819" src="https://github.com/user-attachments/assets/d56832e6-3826-4a19-bb51-8c98cc6c19b4" />


(You can include screenshots or demo GIFs here)

🔮 Future Work

Add support for more sign language gestures.

Improve accuracy with larger datasets.

Deploy model as a web app or mobile app.
