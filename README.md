# Face-Recognition

## Overview

- This project demonstrates a basic face recognition system using **[Python](https://www.python.org/)**, **[OpenCV](https://opencv.org/)**, and the **[face_recognition](https://pypi.org/project/face-recognition/)** library.
- The system can encode known faces from images in a directory, recognize faces in an input image, and label the recognized faces.
- This repository contains all the codes and resources of this project.

## Steps

- Encoding faces from images stored in a directory.
- Recognizing and label faces in an input image.
- Displaying the input image with labeled faces.

## Code

You can find the code for this project here.
* [face_rec.py](https://github.com/LasithaAmarasinghe/Face-Recognition/blob/main/face_rec.py).

## Technologies/Tools

* Python 3.10.12
* OpenCV `pip install opencv-python`
* Python packages
    * numpy `pip install numpy`
    * cmake `pip install cmake`
    * dlib `pip install dlib`
    * face_recognition `pip install face_recognition`
 
![Python](https://img.shields.io/badge/python-3670A0?logo=python&logoColor=FFFF00)
![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?logo=opencv&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?logo=numpy&logoColor=white)
![cmake](https://img.shields.io/badge/cmake_-red)
![dlib](https://img.shields.io/badge/dlib_-purple)
![face_recognition](https://img.shields.io/badge/face_recognition_-brown)
   
* C++ compiler - install [Visual Studio](https://visualstudio.microsoft.com/downloads/)

## Installation
 
  1. **Clone the repository:**
 
     ```bash
     git clone https://github.com/LasithaAmarasinghe/Face-Recognition.git
     cd Face-Recognition
     ```
 
  2. **Create and activate a virtual environment (optional but recommended):**

     ```bash
     python -m venv venv
     source venv/bin/activate   # On Windows use `venv\Scripts\activate`
     ```
 
  3. **Install the required packages:**
 
     ```bash
     pip install -r requirements.txt
     ```
 
## Usage
 
  1. **Prepare the Faces Directory:**
 
     - Create a directory named `faces` in the root of your project.
     - Add images of known faces to the `faces` directory. Ensure the images are named with the format `name.jpg` or `name.png` 
       where `name` is the label you want to assign to the face.
 
  2. **Run the Face Recognition Script:**

     - Place the image you want to test in the root of your project directory and name it `test.jpg`.
     - Run the script:
 
       ```bash
       python face_rec.py
       ```
 
  3. **Interact with the Display:**
 
     - The script will display the `test.jpg` image with labeled faces.
     - Press 'q' to close the display window.
 
## Code Explanation

  - **`get_encoded_faces()`:** This function scans the `faces` directory, encodes each face, and stores the encodings in a dictionary.
  - **`unknown_image_encoded(img)`:** This function encodes an unknown face from a given image file.
  - **`classify_face(im)`:** This function reads an image, detects faces in it, compares them to the known face encodings, labels the faces, 
    and displays the image with labeled faces.

## Results

![image](https://github.com/LasithaAmarasinghe/Face-Recognition/assets/106037441/5c986ce6-ca57-4888-b27a-1d0b3568e116)


## License
 
 * This project is licensed under the MIT License. See the [LICENSE](MIT-LICENSE.txt) file for details.
 

