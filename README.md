Detection of Abnormal and Suspicious Human Activities Using Deep Learning
This project aims to detect abnormal and suspicious human activities from video footage using deep learning
techniques. 
It uses a combination of Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (RNNs) with
LSTM layers 
to analyze video sequences and identify events such as fighting, robbery, or other unusual behaviors.
 What This Project Does
- Takes in video input (like CCTV footage)
- Processes the frames using deep learning models
- Detects if the activity is normal or abnormal
- Sends an alert (e.g., email) when abnormal behavior is detected
 Technologies Used
- Python
- TensorFlow / Keras
- OpenCV
- CNN + RNN (LSTM)
- Email automation with SMTP
 Dataset
We used a dataset consisting of labeled videos for both normal and abnormal activities. The dataset includes
actions like:
- Normal: Walking, talking, standing
- Abnormal: Fighting, theft, aggression
The videos were processed into frames for model training and testing.
 How It Works
1. Video to Frame Conversion: Video files are split into frames.
2. Model Training: A CNN extracts features from each frame, and an LSTM learns the sequence pattern to
classify the action.
3. Real-Time Detection: The trained model can process incoming video streams.
4. Alert System: When an abnormal activity is detected, an email alert is triggered to notify the concerned
authorities.
 Alert Feature
This project includes a simple mail system. When suspicious activity is detected, an email is automatically
sent with a message like:
Suspicious activity detected at camera location at [timestamp]. Please check immediately.
 How to Run
1. Clone this repo 
 git clone https://github.com/yourusername/abnormal-activity-detection.git
 cd abnormal-activity-detection
2. Install the requirements 
 pip install -r requirements.txt
3. Run the main notebook or script 
 python detect_activity.py
4. Set up your email credentials in the script before using the alert feature.
 Applications
- Surveillance systems in public places
- Security for smart cities
- Automatic alert systems for crimes in real-time
 Note
This is a research-based project and not meant for production as-is. Accuracy may vary based on dataset
quality and model training. 
You can improve it by experimenting with different models, larger datasets, or advanced preprocessing
techniques.
