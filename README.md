AI-Based Virtual Interviewer for Automated Candidate Evaluation

An AI-powered interview evaluation system that analyzes candidate interview videos using Deep Learning models including DNN, CNN, LSTM, and Hybrid CNN+LSTM+DNN architectures. The system extracts video frames using OpenCV, performs behavioral analysis, predicts candidate selection status, and generates automated feedback through a Streamlit web application.

Project Overview

This project automates the initial screening process in recruitment by evaluating recorded interview videos. The system analyzes:

Confidence
Communication
Facial Expression
Eye Contact
Overall Interview Performance

The final prediction classifies candidates as:

Selected → Score ≥ 70
Not Selected → Score < 70

The project includes:

Deep Learning model training
Comparative analysis of multiple architectures
Mathematical modeling
Automated feedback generation
Streamlit deployment

Based on our research paper:


Technologies Used
Python
TensorFlow / Keras
OpenCV
NumPy
Pandas
Matplotlib
Scikit-learn
Streamlit
Deep Learning Models Used
1. DNN Baseline

Uses structured CSV features:

confidence
communication
expression
eye_contact
score
2. CNN Frame-Based Model

Extracts spatial features from video frames.

3. LSTM Temporal Model

Captures behavioral changes across video frames over time.

4. Hybrid CNN + LSTM + DNN Model

Combines:

CNN spatial learning
LSTM temporal learning
DNN structured feature learning
Workflow
Upload Video
      ↓
Frame Extraction using OpenCV
      ↓
Preprocessing
(Resize + RGB Conversion + Normalization)
      ↓
Deep Learning Inference
(DNN / CNN / LSTM / Hybrid)
      ↓
Score Prediction
      ↓
Selection Decision
      ↓
Automated Feedback Generation

Workflow figure used in the research paper:


Dataset Information

Dataset contains:

Interview videos
Behavioral scores
Binary decision labels

CSV Columns:

video_name
confidence
communication
expression
eye_contact
Score
decision
Preprocessing Steps
Video Processing
20 frames extracted per video
Uniform frame sampling using np.linspace
Frames resized to 64 × 64
Converted from BGR → RGB
Pixel normalization using /255
Tensor Shape
(20, 64, 64, 3)
Selection Rule
if score >= 70:
    decision = "Selected"
else:
    decision = "Not Selected"
Performance Metrics

Models evaluated using:

Accuracy
Precision
Recall
F1-Score
Validation Loss
Experimental Results
Model	Accuracy	F1-Score
DNN	95%	95.7%
CNN	90%	90.9%
LSTM	90%	91.7%
Hybrid	95%	95.7%

Performance table from research paper:


Streamlit Deployment

The project includes a Streamlit web application where users can:

Upload interview videos
Run AI evaluation
View prediction score
Get candidate selection status
Receive automated feedback

Run application:

streamlit run app.py
Project Structure
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
Installation
Clone Repository
git clone <repository_link>
cd AI_Virtual_Interviewer
Install Dependencies
pip install -r requirements.txt
Future Scope
Real-time interview analysis
Audio and speech analysis
Emotion recognition
Transformer-based architectures
Large-scale recruitment deployment
Research Paper

Research paper included in repository:

AI-Based Virtual Interviewer for Automated Candidate Evaluation

Paper reference:
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

Authors
Shruti Biradar   (202402040027)
Saishwari Korade (202402040028)

MIT Academy of Engineering, Pune

License
This project is developed for academic and research purposes.
