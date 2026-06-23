\# 🫁 Respiratory Disease Detection Using CNN on Cough Audio Signals



A deep learning system that analyzes respiratory audio recordings to automatically detect and classify lung diseases using a Convolutional Neural Network (CNN). Trained on real patient audio data from the Respiratory Sound Database.



> 📄 \*\*Published Research:\*\* Co-authored paper published in \*\*DogoRangsang Research Journal (UGC Care Group I)\*\*, December 2023.



\---



\## 📌 Problem Statement



Respiratory diseases like Asthma, Pneumonia, and Bronchiectasis are difficult to diagnose early without expensive clinical equipment. This project builds an AI-powered system that can analyze cough audio signals and predict the underlying lung disease — enabling faster, low-cost, non-invasive diagnosis.



\---



\## 🎯 Project Highlights



\- \*\*CNN model trained on real respiratory audio data\*\* from 126 patients

\- Detects \*\*8 different respiratory diseases\*\* from `.wav` audio files

\- Achieved \*\*100% training accuracy\*\* over 50 epochs

\- Loss reduced to \*\*0\*\* with increasing epochs

\- End-to-end pipeline: audio upload → feature extraction → CNN prediction → disease label



\---



\## 🦠 Diseases Detected



| Disease         |

|----------------|

| Asthma         |

| Pneumonia      |

| Bronchiectasis |

| COPD           |

| And 4 more...  |



\---



\## 📈 CNN Training Results



| Metric        | Value         |

|---------------|---------------|

| Epochs        | 50            |

| Final Accuracy| \*\*100%\*\*      |

| Final Loss    | \*\*0\*\*         |

| Patients      | 126           |

| Disease Classes | 8           |



> With each increasing epoch, accuracy increased and loss decreased to 0.



\---



\## 🏗️ System Architecture



```

Respiratory Audio Dataset (.wav files)

&#x20;           ↓

&#x20; Feature Extraction from Audio

&#x20; (audio features per patient)

&#x20;           ↓

&#x20; Associate Disease Label

&#x20; (from diagnosis dataset)

&#x20;           ↓

&#x20; Train CNN Model (50 epochs)

&#x20;           ↓

&#x20; Upload Test Audio → Predict Disease

```



\---



\## 🔧 Tech Stack



| Component         | Technology              |

|-------------------|-------------------------|

| Language          | Python                  |

| Deep Learning     | TensorFlow / Keras      |

| Model             | Convolutional Neural Network (CNN) |

| Audio Processing  | Librosa                 |

| Data Handling     | NumPy, Pandas           |

| Visualization     | Matplotlib              |

| UI                | Tkinter (Desktop GUI)   |



\---



\## 📁 Project Structure



```

mini-project/

├── model/

│   ├── model\_weights.h5     # Trained CNN model weights

│   ├── history.pckl         # Training history

│   ├── x.txt.npy            # Feature vectors

│   └── y.txt.npy            # Labels

├── testAudio/               # Sample test .wav files

│   ├── 1.wav ... 7.wav

│   ├── aa.wav               # Predicted: ASTHMA

│   ├── aa1.wav

│   └── aa2.wav              # Predicted: Pneumonia

├── Main.py                  # Core CNN pipeline and GUI

├── req.txt                  # Python dependencies

└── run.bat                  # Launch script (Windows)

```



\---



\## 🚀 How to Run



\### Prerequisites

```bash

pip install -r req.txt

```



\### Launch

```bash

\# Windows

run.bat



\# Or directly

python Main.py

```



\### Steps in the Application

1\. \*\*Upload Respiratory Audio Dataset\*\* → select the `Respiratory\_Sound\_Database` folder

2\. \*\*Extract Features from Audio Dataset\*\* → extracts audio features, assigns disease labels

3\. \*\*Train CNN Algorithm\*\* → trains CNN on 126 patient audio files across 8 disease classes

4\. \*\*CNN Accuracy \& Loss Graph\*\* → view training performance over 50 epochs

5\. \*\*Upload Test Audio \& Predict Disease\*\* → upload any `.wav` file to get disease prediction



\---



\## 🧪 Sample Predictions



| Test File | Predicted Disease |

|-----------|-------------------|

| aa.wav    | ASTHMA            |

| aa2.wav   | Pneumonia         |

| others    | COPD, Bronchiectasis, etc. |



\---



\## 📚 Dataset



\- \*\*Respiratory Sound Database\*\* — real patient `.wav` audio recordings

\- \*\*Disease Diagnosis Dataset\*\* — patient-level disease labels

\- 126 patients, 8 disease categories



\---



\## 📰 Publication



> \*\*"Respiratory Analysis Detection of Various Lung Infections Using Cough Signal"\*\*

> Published in \*\*DogoRangsang Research Journal\*\*, UGC Care Group I — December 2023



\---



\## 🎓 Academic Context



\*\*Project Type:\*\* B.Tech Mini Project (Published Research)

\*\*Domain:\*\* Deep Learning / Medical Audio Analysis

\*\*Institution:\*\* Malla Reddy Institute of Technology \& Science, Hyderabad

\*\*Year:\*\* 2023



\---



\## 👤 Author



\*\*Akshay Etukuri\*\*

B.Tech CSE (Networks) | MRITS Hyderabad

\[GitHub](https://github.com/AkshayEtukuri) | \[LinkedIn](#)

