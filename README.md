
# Live Event Detection for People's Safety Using NLP and Deep Learning

![IEEE Published](https://img.shields.io/badge/Published-IEEE%20Access%202024-blue)
![Python](https://img.shields.io/badge/Python-3.8+-green)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![Accuracy](https://img.shields.io/badge/Accuracy-96.6%25-brightgreen)

## 📌 About
A real-time software-based threat detection system that analyzes 
ambient audio from a smartphone microphone to detect dangerous 
situations and automatically alert emergency contacts — with 
zero hardware dependency.

**Published in IEEE Access, Volume 12, January 2024**
DOI: 10.1109/ACCESS.2023.3349097

---

## 🚨 Problem Statement
People — especially women working alone at night — face threats 
like robbery, assault, and homicide. Existing solutions require 
bulky hardware. This system uses only a smartphone microphone 
to detect threats and alert emergency contacts instantly.

---

## ⚙️ How It Works
1. Live audio is recorded from smartphone microphone
2. Audio is preprocessed using Fast Fourier Transform and 
   Mel-Spectrogram analysis
3. Deep learning models classify the audio into 13 sound classes
4. If dangerous sound is detected — automatic alert is sent via 
   SMS, Email and WhatsApp

---

## 🔊 Sound Classes (13 Total)
| Safe Sounds | Dangerous Sounds |
|-------------|-----------------|
| Air Conditioner | 🔴 Fire Crackling |
| Car Horn | 🔴 Glass Breaking |
| Children Playing | 🔴 Gunshot |
| Dog Bark | 🔴 Scream |
| Drilling | |
| Engine Idling | |
| Jackhammer | |
| Siren | |
| Street Music | |

---

## 🧠 Deep Learning Models & Results

| Model | Training Accuracy | Validation Accuracy |
|-------|------------------|-------------------|
| 1D-CNN | 95.2% | 90.2% |
| 2D-CNN | 96.3% | 92.7% |
| LSTM | **96.6%** | **90.3%** |

- **35 epochs** trained per model
- **9,000+ audio clips** used for training
- **90-10 train-test split**
- Best model saved using validation loss checkpoint

---

## 🛠️ Technologies Used
- **Language:** Python
- **Deep Learning:** TensorFlow, Keras
- **Models:** 1D-CNN, 2D-CNN, LSTM (Bidirectional)
- **Audio Processing:** Kapre, LibROSA, FFT, Mel-Spectrogram
- **Alert System:** SMTP (Email), Twilio (SMS), PyWhatKit (WhatsApp)
- **Dataset:** UrbanSound8K, ESC-50, Custom Scream Dataset (Kaggle)

---

## 📊 Dataset
- **Total Audio Clips:** 9,000+
- **Classes:** 13
- **Sampling Rate:** 16,000 Hz (downsampled from 44,100 Hz)
- **Format:** .wav (mono channel)
- **Sources:** UrbanSound8K + ESC-50 + Custom Scream Dataset

---

## 🚀 How To Run

### 1. Clone the repository
```bash
git clone https://github.com/gopigalam/live-event-detection-nlp
cd live-event-detection-nlp
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Train the models
```bash
python train.py
```

### 4. Run live prediction
```bash
python predict.py
```

---

## 📧 Alert System
On detection of dangerous audio:
- 📧 **Email** sent with recorded audio attached
- 📱 **SMS** sent to registered contact
- 💬 **WhatsApp** message sent automatically

---

## 📄 Research Paper
**Title:** Live Event Detection for People's Safety Using 
NLP and Deep Learning

**Journal:** IEEE Access, Volume 12, 2024

**Authors:** Amrit Sen, Gayathri Rajakumaran, Miroslav Mahdal, 
Shola Usharani, Vezhavendhan Rajasekharan, Rajiv Vincent, 
Karthikeyan Sugavanan

**DOI:** [10.1109/ACCESS.2023.3349097](https://doi.org/10.1109/ACCESS.2023.3349097)

---

## 👨‍💻 Developer
**Gopi Galam**
- 📧 gopigalam8@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/gopigalam/)
- 🎓 B.Tech Computer Science & Engineering, 2025

---

## ⭐ Star this repository if you found it useful!
