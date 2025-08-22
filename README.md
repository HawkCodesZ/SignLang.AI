# SignLang.AI: Sign Language Translation into Text and Audio

SignLang.AI is a project that translates American Sign Language (ASL) gestures into text and audio using computer vision and machine learning techniques.

## Overview

The project utilizes computer vision techniques to detect hand gestures captured through a webcam, processes these gestures using machine learning models, and translates them into corresponding text and audio outputs. It employs the Mediapipe library for hand landmark detection and OpenCV for video capture and display.

## Installation

Ensure you have the necessary libraries installed. You can install them using pip:

```bash
pip install mediapipe opencv-python numpy matplotlib scikit-learn
```

## How it Works

1. **Data Collection**: The system collects images of ASL gestures to build a dataset for training. Users move their hands across the screen to record each letter of the alphabet.

2. **Data Processing**: Hand landmarks from the collected images are extracted using the Mediapipe library. These landmarks serve as features for training a machine learning model.

3. **Model Training**: A Random Forest classifier is trained on the extracted hand landmark data to classify gestures into corresponding letters (A-Z).

4. **Real-time Translation**: During inference, the trained model predicts the gesture from live video feed, converts it into text using predefined mappings, and generates corresponding audio output.

## Usage

1. **Data Collection**:
   - Run the data collection script to capture hand gesture images.
   - Move your hand to record each letter from A to Z.

2. **Training**:
   - Use the collected dataset to train the machine learning model using the provided training script.
   - Ensure the dataset is properly labeled and split into training and testing sets.

3. **Inference**:
   - Run the inference script to translate real-time hand gestures into text and audio.
   - Ensure your webcam is connected and positioned to capture hand movements.

## Dependencies

- **Mediapipe**: Provides hand landmark detection capabilities.
- **OpenCV**: Used for video capture, image processing, and display.
- **NumPy**: Essential for numerical operations and data handling.
- **Matplotlib**: Optional for data visualization during development.
- **scikit-learn**: Provides machine learning utilities for training and inference.

## Collabrators
- Harsh Choubey: Harshchoubey55 (git username), harshcy55@gmail.com (mail ID)
- Neha Singh: Miuchan24 (git username), noctis24x@gmail.com (mail ID)

## Credits

This project template is inspired by advancements in computer vision and machine learning techniques, leveraging Mediapipe and OpenCV for real-time hand gesture translation.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
