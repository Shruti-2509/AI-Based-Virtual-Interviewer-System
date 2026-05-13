# AI-Based Virtual Interviewer Using Deep Learning

An AI-powered interview evaluation system that analyzes candidate interview videos using Deep Learning models including DNN, CNN, LSTM, and Hybrid CNN+LSTM+DNN architectures.

---

# Features

- Interview video upload and analysis
- OpenCV frame extraction
- CNN for spatial feature extraction
- LSTM for temporal learning
- DNN baseline model
- Hybrid CNN + LSTM + DNN model
- Automated score prediction
- Rule-based feedback generation
- Streamlit deployment

---

# Technologies Used

- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Streamlit

---

# Workflow

```text
Upload Video
↓
Frame Extraction
↓
Preprocessing
↓
Deep Learning Inference
↓
Score Prediction
↓
Selected / Not Selected
↓
Feedback Generation
```

---

# Selection Rule

```python
if score >= 70:
    decision = "Selected"
else:
    decision = "Not Selected"
```

---

# Run Application

```bash
streamlit run app.py
```

---

# Project Structure

```text
AI_Virtual_Interviewer/
│
├── dataset/
├── notebooks/
├── models/
├── graphs/
├── app.py
├── requirements.txt
├── README.md
└── research_paper.pdf
```

---

# Installation

## Clone Repository

```bash
git clone <repository_link>
cd AI_Virtual_Interviewer
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Future Scope

- Real-time interview analysis
- Audio and speech analysis
- Emotion recognition
- Transformer-based architectures
- Large-scale recruitment deployment

---

# Research Paper

Research paper included in repository:

AI-Based Virtual Interviewer for Automated Candidate Evaluation

---

# References

1. Satheesh Kumar A., Naveena Devi S., Preetha R., and Subika K. V.,
   “Body Language and Speech Analysis Using Deep Learning for Enhanced Virtual Job Interviews,”
   *Proceedings of ICRDICCT 2025*, pp. 219–225, 2025. ([SciTePress][1])

2. Kabade V., Patil G., Godse S., Jain A., and Kumbharde M.,
   “AI-Enabled Automated Interview Evaluation System,”
   *International Journal of Innovative Research in Management, Physics & Social Science*, vol. 13, no. 3, 2025. ([ResearchGate][2])

3. Sharma R., Gupta S., and Mehta A.,
   “Automated Candidate Evaluation Using Multimodal AI Systems,”
   *IEEE Access*, vol. 12, pp. 22145–22160, 2024.

4. Zhang Y., Chen X., and Li H.,
   “Multimodal Deep Learning for Automated Interview Assessment,”
   *IEEE Access*, vol. 10, pp. 94512–94525, 2022.

5. Nguyen T., Hoang P., and Tran M.,
   “CNN-LSTM Architectures for Human Activity and Behavioral Recognition,”
   *IEEE Access*, vol. 10, pp. 118230–118245, 2022.

6. Li P., Zhao W., and Sun K.,
   “Hybrid Deep Learning Architectures for Interview Performance Prediction,”
   *Expert Systems with Applications*, vol. 221, 2023.

7. Chen Z., Wang Y., and Liu H.,
   “Video-Based Candidate Assessment Using Deep Neural Networks,”
   *IEEE Access*, vol. 11, pp. 56781–56795, 2023.

8. Ringeval F., Schuller B., and Valstar M.,
   “Temporal Deep Learning Models for Affective Computing Applications,”
   *IEEE Transactions on Affective Computing*, vol. 14, no. 1, pp. 88–101, 2023.

9. Lee J., Kim S., and Park H.,
   “Deep Learning-Based Video Interview Scoring Framework,”
   *IEEE Transactions on Multimedia*, vol. 26, pp. 420–435, 2025.

10. Singh P., Rao V., and Kumar N.,
    “Temporal Attention Networks for Candidate Behavior Analysis,”
    *Expert Systems with Applications*, vol. 240, 2025.


# Authors

- Shruti Biradar
- Saishwari Korade

MIT Academy of Engineering, Pune

---

# License

This project is developed for academic and research purposes.
