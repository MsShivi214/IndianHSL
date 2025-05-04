# IndianHSL
# Indian Hand Sign Language Recognition System

This project implements a real-time Indian Hand Sign Language recognition system using computer vision and machine learning. The system can detect and classify hand gestures from a live video feed.

## Features

- Real-time hand gesture detection using webcam
- Support for multiple hand sign classes (A, B, C)
- Live visualization of detected gestures
- Data collection utility for training new gestures

## Project Structure

```
.
├── Data/              # Directory for storing training data
├── Model/             # Contains trained model files
├── dataCollection.py  # Script for collecting training data
├── test.py           # Main application for real-time recognition
└── venv/             # Python virtual environment
```

## Prerequisites

- Python 3.x
- OpenCV (cv2)
- cvzone library
- NumPy
- Webcam

## Installation

1. Clone this repository
2. Create a virtual environment:
   ```bash
   python -m venv venv
   ```
3. Activate the virtual environment:
   - Windows:
     ```bash
     .\venv\Scripts\activate
     ```
   - Linux/Mac:
     ```bash
     source venv/bin/activate
     ```
4. Install required packages:
   ```bash
   pip install opencv-python cvzone numpy
   ```

## Usage

### Data Collection
To collect training data for new gestures:
```bash
python dataCollection.py
```
- Press 's' to save the current hand gesture
- Images will be saved in the Data directory

### Real-time Recognition
To run the hand sign recognition system:
```bash
python test.py
```
- The system will open your webcam
- Show hand gestures to the camera
- The recognized gesture will be displayed on screen

## Model Training
The project uses a pre-trained model stored in the Model directory:
- `keras_model.h5`: The trained model file
- `labels.txt`: Contains the class labels

## Contributing
Feel free to contribute to this project by:
- Adding support for more hand signs
- Improving the recognition accuracy
- Enhancing the user interface

## License
This project is open source and available under the MIT License.
