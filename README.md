# Arabic Image Captioning and Question Answering App 

This project implements an **automated pipeline** for processing images, generating captions, translating captions to Arabic, and answering questions related to the images. It employs state-of-the-art machine learning models for image captioning, translation, and visual question answering (VQA). Additionally, the system converts Arabic captions to audio for playback. The interactive interface is powered by Gradio.

## Table of Contents  
- [Overview](#overview)  
- [Features](#features)  
- [Workflow](#workflow)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Technologies Used](#technologies-used)  
- [License](#license)  

## Overview  

The pipeline allows users to upload an image and interactively receive captions, translations, and answers to questions about the image. Designed for accessibility, it provides text and audio outputs in Arabic.  

### Key Components:  
1. **Image Captioning**: Generates descriptive captions for input images.  
2. **Arabic Translation**: Translates captions from English to Arabic.  
3. **Audio Playback**: Converts Arabic captions to speech for playback.  
4. **Visual Question Answering (VQA)**: Answers questions about the image in Arabic.  

---

## Features  

- **Caption Generation**  
   - Automatically generates captions for uploaded images using advanced AI models.  

- **Arabic Translation**  
   - Translates captions into Arabic for accessibility.  

- **Question Answering**  
   - Enables users to ask questions about the image and receive context-aware answers in Arabic.  

- **Audio Output**  
   - Converts Arabic captions into speech for audio playback or download.  

- **Interactive Interface**  
   - Provides a user-friendly Gradio-based UI for seamless interaction.  

---

## Workflow  

Here’s a step-by-step breakdown of the system pipeline:  

1. **Input Image**: User uploads an image via the Gradio interface.  
2. **Caption Generation**: The image is processed to generate an English caption using a BLIP-based model.  
3. **Arabic Translation**: The caption is translated to Arabic using a pre-trained translation model.  
4. **Audio Output**: Arabic captions are converted to speech using Google Text-to-Speech (gTTS).  
5. **Question Suggestions**: The model generates suggested questions related to the image. Users can select or input custom questions.  
6. **Visual Question Answering (VQA)**: The selected question is answered, and the answer is translated into Arabic.  
7. **Result Display**: Both the Arabic caption and the VQA answer are displayed.  

---

## Installation  

To set up this project locally, follow these steps:  

1. **Clone the repository**  
    ```bash  
    git clone https://github.com/Abdelmanemm/Image_arabic_description.git  
    cd Image_arabic_description  
    ```  

2. **Install required libraries**  
    ```bash  
    pip install -r requirements.txt  
    ```  

3. **Run the application**  
    ```bash  
    python app.py  
    ```  

4. **Access the interface**  
   Open your browser at `http://127.0.0.1:7860` to interact with the app.  

---

## Usage  

1. Upload an image via the Gradio interface.  
2. The pipeline generates an English caption, translates it to Arabic, and provides an audio playback option.  
3. Select a suggested question or input a custom question about the image.  
4. Receive the answer in Arabic, both as text and audio.  

---

## Technologies Used  

- **[BLIP Image Captioning Models](https://huggingface.co/Salesforce/blip-image-captioning-large)**: For generating image captions.  
- **[MBART Translation Models](https://huggingface.co/facebook/mbart-large-50-many-to-many-mmt)**: For Arabic translation.  
- **gTTS**: For converting Arabic text to speech.  
- **Gradio**: For building an interactive user interface.  

---

## License  

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.  
