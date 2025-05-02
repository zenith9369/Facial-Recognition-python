
# Face Detection and Recognition Project

This repository contains a face detection and recognition system using OpenCV and Haar cascade classifiers.

## 📁 Project Structure

```
.
├── dataset/                             # Folder to store captured face images
├── trainer/                             # Folder for storing trained model files
├── 1.py                                 # Script to capture face data and store in dataset/
├── final.py                             # Final script for real-time face recognition
├── haarcascade_frontalface_default.xml # Pre-trained Haar Cascade for face detection
├── trainerr.py                          # Script to train the face recognition model
```

---

## 🚀 How to Use

### 1. Install Dependencies

```bash
pip install opencv-python numpy
```

---

### 2. Capture Face Data

Run the following command to start capturing face images. Ensure your webcam is connected.

```bash
python 1.py
```

- This will open your webcam.
- Follow the prompts to enter your ID/name and collect multiple face images.
- Images will be saved to the `dataset/` folder.

---

### 3. Train the Model

After capturing images, train the recognizer:

```bash
python trainerr.py
```

- This script reads images from `dataset/`, trains a model, and saves it in the `trainer/` folder.

---

### 4. Run Face Recognition

Finally, run real-time face recognition using:

```bash
python final.py
```

- The webcam will detect and recognize known faces based on the trained model.
- Unknown faces will not be labeled or will be marked as "Unknown".

---

## 🧠 Notes

- `haarcascade_frontalface_default.xml` is used to detect faces and must be in the same directory as the scripts or correctly referenced.
- Ensure good lighting and frontal face angles while capturing data for better accuracy.

---

## 📌 Requirements

- Python 3.x
- OpenCV
- NumPy

---

## 🔒 License

This project is licensed under the MIT License.
