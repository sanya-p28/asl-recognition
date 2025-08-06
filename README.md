# 🖐️ ASL Hand Detection System

A computer vision system that detects **left and right hands** to assist in recognizing American Sign Language (ASL) gestures. This project uses OpenCV and Mediapipe to identify and crop hand regions from webcam video in real time, saving them for dataset creation and further training.

---

## 📸 Features

✅ Real-time detection of left and right hands  
✅ Automatic cropping and saving of detected hands  
✅ Adjustable offset and image size for better framing  
✅ Label assignment to different ASL gestures  
✅ Built with Python, OpenCV, and Mediapipe

---

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/HandSignDetectionn.git
   cd HandSignDetectionn
(Optional but recommended) Create a virtual environment

bash
Copy
Edit
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
.venv\Scripts\activate      # Windows
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
⚙️ Usage
Run the data collection script to start capturing images:

bash
Copy
Edit
python dataCollection.py
By default, images will be saved under the Data/ folder with subfolders based on your assigned labels.

Edit dataCollection.py to change:

offset → Margin around the cropped hand

imgSize → Output image size (default: 300×300)

folder → Data save location

labels → List of labels for your ASL signs

Press q in the OpenCV window to exit the program.

🛠️ Project Structure
bash
Copy
Edit
HandSignDetectionn/
├── dataCollection.py       # Main hand detection & data collection script
├── test.py                 # Script for testing detection (optional)
├── Data/                   # Folder for collected hand images
├── README.md               # Project documentation
└── requirements.txt        # Python dependencies
❗ Troubleshooting
cv2.error: ... !ssize.empty()
This error occurs if no hand is detected in the frame. Make sure your webcam is active and your hand is visible.

Cannot open camera
Check your webcam permissions or try restarting your computer.

🏗️ Contributing
Contributions are welcome! You can:

Add new ASL gestures or improve label handling.

Optimize detection accuracy.

Create a GUI for easier usage.

Train a full ASL recognition model using collected data.

To contribute:

Fork the repo

Create a new branch (git checkout -b feature/YourFeature)

Commit your changes

Push to your branch and open a pull request

📜 License
This project is licensed under the MIT License.

🙌 Acknowledgements
OpenCV – Computer vision library

Mediapipe – Real-time hand tracking

Python – The language powering it all

⭐ If you find this project helpful, consider giving it a star on GitHub!

yaml
Copy
Edit

---

## ✅ Next Steps

1. Save this text as a `README.md` file at your project root.
2. Commit and push it to GitHub:
   ```bash
   git add README.md
   git commit -m "Add complete project README"
   git push origin main
