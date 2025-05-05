# React Application for Emotion Detection Using Audio-Visual Modalities for Accident Prevention

## 📌 Overview

This project presents a **React-based front-end** integrated with an **AI back-end** for detecting human emotions using both **audio and video data**. The primary goal is to enhance safety—particularly in automotive environments—by monitoring emotional states to prevent accidents.

---

## 🧠 AI Model Title

**Audio-Visual Emotion Detection with eNTERFACE and CREMA-D Datasets**

---

## 📂 Datasets Used

- **[CREMA-D Dataset](https://github.com/CheyneyComputerScience/CREMA-D)**  
- **[eNTERFACE Dataset](http://mirlab.org/dataset/public/eNTERFACE/)**

These datasets provide high-quality labeled **audio** and **video** samples for training and evaluating emotion recognition models.

---

## 🔧 Data Preprocessing and Fusion

### 🎙️ Audio Processing

- **MFCC (Mel-Frequency Cepstral Coefficients)**  
- **Mel Spectrograms**

Both are converted into image representations to allow fusion with visual data.

### 🎞️ Visual Processing

- Video frames are extracted at a fixed rate and resized to 224x224.
- Stored as sequences of images for time alignment with audio.

### 🔗 Fusion Techniques

#### 1. **Early Fusion**
- Combines audio and video at the input stage.
- Enables joint learning from both modalities from the start.

#### 2. **Late Fusion**
- Processes audio and video separately.
- Combines their features at the classification layer.

---

## 🚀 Model Details

- **Model:** VideoMAE (Masked AutoEncoder for Video)
- **Pre-trained on:** Kinetics-400 dataset
- **Fine-tuned Version Used:** `TFVideoMAE_L_K400_16x224_FT`
- **Repository:** [VideoMAE GitHub](https://github.com/MCG-NJU/VideoMAE)

The VideoMAE model is well-suited for capturing **temporal and spatial features** from both video and aligned audio representations.

---

## 🌐 React Front-End Features

- Upload video or audio input
- Preview input video
- Sends request to AI model back-end
- Displays predicted emotion in real-time
- Responsive and easy-to-use UI

---

## 💡 Application Use Cases

- **Driver Emotion Monitoring** (for in-vehicle safety systems)
- **Real-Time Surveillance Emotion Analysis**
- **Multimodal Interaction Interfaces**

---

## 📬 Contact

For questions, collaboration, or contributions:

- 📧 mohammed.ghanemi@tum.de  
- 📧 mohammed.ghanemi@iav.de

---

## 🏁 Getting Started

```bash
# Clone the repository
git clone https://github.com/yourusername/React-aaplication-for-Emotion-detection-using-audio-visual-modalities-for-accident-prevention

# Navigate to project folder
cd React-aaplication-for-Emotion-detection-using-audio-visual-modalities-for-accident-prevention

# Install dependencies
npm install

# Start the development server
npm start
