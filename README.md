# People Tracking with Age and Gender Detection

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [License](#license)
- [Contributing](#contributing)
- [Contact](#contact)

## Introduction

Welcome to the People Tracking with Age and Gender Detection project! This system leverages state-of-the-art computer vision techniques to track multiple individuals in real-time, providing accurate age and gender predictions. Built using Python and a suite of powerful libraries, this project showcases the potential of AI in enhancing video analytics.

## Features

- **Real-time People Tracking**: Efficiently track multiple individuals in live video streams or recorded footage.
- **Age Detection**: Predict the age of each tracked individual with high accuracy.
- **Gender Detection**: Classify the gender of each tracked individual using pre-trained models.
- **User-Friendly Interface**: Simple command-line interface for ease of use and integration.

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/people-tracking-age-gender.git
    cd people-tracking-age-gender
    ```

2. **Create and activate a virtual environment (optional but recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Prepare the models and input video:**
   - Ensure you have the pre-trained models for age and gender detection placed in a `models` directory within the project.
   - Provide the path to your input video or set up your webcam for real-time detection.

2. **Run the script:**
    ```bash
    python people_tracking.py --input path/to/video --prototxt models/deploy.prototxt --model models/res10_300x300_ssd_iter_140000.caffemodel --age_model models/age_net.caffemodel --gender_model models/gender_net.caffemodel
    ```

    **Command line arguments:**
    - `--input`: Path to the input video file. Use `0` for webcam.
    - `--prototxt`: Path to the Caffe 'deploy' prototxt file.
    - `--model`: Path to the pre-trained Caffe model.
    - `--age_model`: Path to the pre-trained age detection model.
    - `--gender_model`: Path to the pre-trained gender detection model.

## Technologies Used

- **Python**: Main programming language.
- **OpenCV (cv2)**: For image processing and computer vision operations.
- **dlib**: For facial landmark detection.
- **NumPy**: For numerical operations.
- **PyImageSearch**: For various computer vision utilities.
- **argparse**: For parsing command line arguments.
- **imutils**: For simplifying OpenCV operations.

## Project Structure

```plaintext
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
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contributing

We welcome contributions from the community! If you'd like to contribute, please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request.

## Contact

For any inquiries or suggestions, feel free to reach out:

**Author**: Amrish kumar Tiwary
**Email**: tiwariambrish81@gmail.com
**GitHub**: https://github.com/Coderamrish

---

We hope this project helps you in your endeavors with computer vision. Happy coding! 🚀
