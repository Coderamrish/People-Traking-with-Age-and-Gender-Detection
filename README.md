# People-Traking-with-Age-and-Gender-Detection
People Tracking with Age and Gender Detection
Table of Contents
Introduction
Features
Installation
Usage
Technologies Used
Project Structure
License
Introduction
This project implements a people tracking system with age and gender detection using Python. By leveraging computer vision libraries and pre-trained models, the system can track multiple people in real-time and predict their age and gender.

Features
Real-time people tracking
Age detection
Gender detection
Utilizes pre-trained models for accurate predictions
Installation
Clone the repository:


git clone https://github.com/your-username/people-tracking-age-gender.git
cd people-tracking-age-gender
Create and activate a virtual environment (optional but recommended):


python -m venv venv
source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
Install the required packages:


pip install -r requirements.txt
Usage
Prepare the models and input video:

Ensure you have the pre-trained models for age and gender detection placed in a models directory within the project.
Provide the path to your input video or set up your webcam for real-time detection.
Run the script:


python people_tracking.py --input path/to/video --prototxt models/deploy.prototxt --model models/res10_300x300_ssd_iter_140000.caffemodel --age_model models/age_net.caffemodel --gender_model models/gender_net.caffemodel
Command line arguments:

--input: Path to the input video file. Use 0 for webcam.
--prototxt: Path to the Caffe 'deploy' prototxt file.
--model: Path to the pre-trained Caffe model.
--age_model: Path to the pre-trained age detection model.
--gender_model: Path to the pre-trained gender detection model.
Technologies Used
Python: Main programming language.
OpenCV (cv2): For image processing and computer vision operations.
dlib: For facial landmark detection.
NumPy: For numerical operations.
PyImageSearch: For various computer vision utilities.
argparse: For parsing command line arguments.
imutils: For simplifying OpenCV operations.
Project Structure
plaintext

people-tracking-age-gender/
├── models/
│   ├── deploy.prototxt
│   ├── res10_300x300_ssd_iter_140000.caffemodel
│   ├── age_net.caffemodel
│   ├── gender_net.caffemodel
├── examples/
│   ├── example_video.mp4
├── people_tracking.py
├── requirements.txt
├── README.md
License
This project is licensed under the MIT License. See the LICENSE file for more details.

Feel free to contribute to this project by submitting issues or pull requests. Your feedback and contributions are highly appreciated!

Author: Amrish kumar Tiwary

Contact: Tiwariambrish81@gmail.com

GitHub: https://github.com/Coderamrish
