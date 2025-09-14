# Intruder Detection with Face Recognition

This project uses OpenCV and the `face_recognition` library to detect faces through a webcam. 
If the detected face does not match the owner, the system captures an image and sends an email alert.

## Features
- Detect faces in real-time using webcam
- Identify owner vs intruder
- Save intruder image locally
- Send intruder image to email

## Requirements
- Python 3.7+
- OpenCV
- face_recognition
- smtplib (for email alerts)

## Setup Instructions
1. Install required libraries:
   ```bash
   pip install opencv-python face_recognition
   ```

2. Save an image of the owner (e.g., `owner.jpg`) in the same folder.

3. Update your Gmail credentials in the code:
   - Replace `youremail@gmail.com` with your Gmail
   - Replace `your_app_password` with your Gmail App Password
   - Replace `receiveremail@gmail.com` with the email that should receive alerts

4. Run the notebook `Intruder_Detection.ipynb` step by step.

5. Press **Q** in the camera window to stop detection.

## Notes
- You must enable "App Passwords" in Gmail for sending emails.
- Accuracy depends on lighting and camera quality.
