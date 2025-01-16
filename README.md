# RagaXonic: AI-Powered Music Generation  

RagaXonic is a custom AI-based music generator that fuses Hindustani and Western musical traditions to produce unique polyphonic MIDI compositions. It leverages a 3-layered LSTM neural network to analyze, learn, and create music based on input MIDI datasets.  

## Key Features  
- **Fusion of Hindustani and Western Music**: A unique approach to blending two musical traditions.  
- **Deep Learning Architecture**: A 3-layered LSTM network for polyphonic music generation.  
- **Interactive UI**: Gradio-powered interface for temperature control, number of notes, and music generation.  
- **Customizable Outputs**: Adjust the length and style of generated music.  
- **MIDI File Support**: Outputs music as MIDI files for further editing or playback.  

---

## Table of Contents  
- [Setup and Installation](#setup-and-installation)  
- [How It Works](#how-it-works)  
- [Usage](#usage)  
- [Sample Output](#sample-output)  
- [Future Work](#future-work)  
- [Acknowledgments](#acknowledgments)  

---

## Setup and Installation  

### Prerequisites  
- Python 3.8+  
- TensorFlow  
- Music21  
- Gradio  

Install dependencies using:  
```bash  
pip install tensorflow music21 gradio numpy
```  

### Project Files  
- **`notes/`**: Processed note data extracted from MIDI files.  
- **`weights/`**: Model checkpoint files.  
- **`outputf.mid`**: Generated MIDI files.  
- **`scripts/`**: Python files for training and generation.  

---

## How It Works  

### 1. Data Preprocessing  
- Extracts notes and chords from input MIDI files.  
- Converts musical elements into sequences of integers for LSTM processing.  

### 2. Model Training  
- A 3-layered LSTM network is trained on the processed sequences.  
- Incorporates dropout and batch normalization to enhance performance.  

### 3. Music Generation  
- Generates notes using a probabilistic approach based on temperature scaling.  
- Converts sequences back into MIDI format for playback.  

### 4. Interactive UI  
- Gradio-powered interface to adjust generation parameters.  
- Outputs MIDI files for download and playback.  

---

## Usage  

### Training the Model  
To train the model from scratch:  
```bash  
python train_network.py  
```  

### Generating Music  
Run the interactive UI using Gradio:  
```bash  
python app.py  
```  

### Output  
- Specify the number of notes and temperature (creativity) for generation.  
- Download the generated MIDI file for playback.  

---

## Sample Output  
Here’s a preview of the generated music:  
- **[Output MIDI File 1](./samples/output1.mid)**  
- **[Output MIDI File 2](./samples/output2.mid)**  

---

## Future Work  
- Integration with additional musical styles and datasets.  
- Real-time music playback within the web UI.  
- Exporting to audio formats (e.g., WAV, MP3).  

---

## Acknowledgments  
- Built with [TensorFlow](https://www.tensorflow.org/) and [Music21](http://web.mit.edu/music21/).  
- Inspired by classical Hindustani Ragas and Western music theory.  
- Developed by **Manas K.**  

---

Enjoy generating music with **RagaXonic**! 🎶  

---  

Let me know if you'd like to add anything specific!
