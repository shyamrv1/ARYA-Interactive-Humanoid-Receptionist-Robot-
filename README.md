# Arya - Humanoid Receptionist Robot - ChatGpt integrated 

Arya is a humanoid receptionist robot, designed to provide a welcoming experience, interact with visitors, and handle various reception tasks at Amity University Bengaluru. This project leverages speech recognition, text-to-speech, object detection, and OpenAI's language model to perform interactive tasks.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Setup](#setup)
- [Usage](#usage)
- [Configuration](#configuration)
- [Requirements](#requirements)
- [Authors](#authors)

## Features

- **Speech Recognition**: Listens and responds to visitors' queries using Google's Speech Recognition API.
- **Text-to-Speech**: Communicates through voice using Pyttsx3, enhancing interaction.
- **Object Detection**: Detects objects (like people) using OpenCV and alerts Aarryaa to engage with visitors.
- **Conversational AI**: Uses OpenAI's GPT-3.5-turbo to process and respond to visitor questions.
- **Information Storage**: Records visitor information, including name, address, and purpose, in a local directory.
- **Room Guidance**: Provides directions for various rooms in the university.
  
## Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/your-repository-name.git
    cd your-repository-name
    ```

2. **Install the Required Libraries**:
    Install the required dependencies using `pip`:
    ```bash
    pip install opencv-python-headless speechrecognition pyttsx3 openai numpy
    ```

3. **Download the Model Files**:
   - Download the `ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt` and `frozen_inference_graph.pb` files for object detection and save them in the `Object_Detection_Files` directory.
   - Download the `coco.names` file containing class names and save it in the same directory.

## Setup

1. **API Key for OpenAI**:
   - Obtain an API key from [OpenAI](https://openai.com/).
   - Replace `apikey` in the code with your actual API key.

2. **Adjust Paths**:
   Ensure paths for `coco.names`, `ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt`, and `frozen_inference_graph.pb` files are correct in the code.

3. **Configure Text-to-Speech Voice**:
   Optionally, you can adjust the voice used by Pyttsx3.

## Usage

To start Aarryaa:

1. **Run the Script**:
   ```bash
   python main.py
