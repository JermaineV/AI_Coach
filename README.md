# AI Communication Coach

[![AI Communication Coach Image](https://github.com/JermaineV/JermaineV.github.io/blob/9485850cfc3d0007e00998eb6b26f9225f5d1721/images/botpic.jpeg?raw=true)](https://github.com/JermaineV/AI_Coach)

This project aims to develop a platform that utilizes Artificial Intelligence (AI) to assist users in improving their communication skills for public speaking and interviews. The coach can leverage various techniques, including:

- **Speech Recognition:** Capture user input through speech.
- **Text Analysis:** Analyze the text content to understand sentiment, keywords, and named entities.
- **Pre-trained LLM Integration:** Utilize a pre-trained Large Language Model (LLM) like GPT-j to generate informative responses.

## Index
1. [Features (In Progress)](#features-in-progress)
2. [Tech Stack](#tech-stack)
3. [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
    - [Usage](#usage)
4. [Current Functionality](#current-functionality)
5. [Future Development](#future-development)
6. [Transformers and LLMs](#transformers-and-llms)
7. [License](https://github.com/JermaineV/AI_Coach/blob/230c61b8769721db73a9b1c617dfdd47eb4db38f/LICENSE.md)

## Features (In Progress)

- **Speech Recognition**: Capture and analyze user speech for content and delivery.
- **Text Analysis**: Process user-provided text (e.g., job descriptions, presentation outlines) to understand context and generate relevant questions.
- **Mock Interview Simulation**: Simulate interview scenarios with AI-powered questions based on user input.
- **Performance Analysis**: Provide feedback on speech patterns, body language (future implementation), and content organization.

## Tech Stack

- **Python**: Programming Language
- **Jupyter Notebook**: Development environment
- **SpeechRecognition**: Speech Recognition
- **NLP Libraries**: NLTK, spaCy, TextBlob
- **Transformers**: Hugging Face Transformers for text generation
- **(Optional) OpenCV**: Computer Vision for future features

## Getting Started

### Prerequisites

- Python 3.x (Ensure you have the latest version)
- Jupyter Notebook (Consider using Anaconda for a bundled environment)
- Additional libraries (install using `pip` in your terminal or the Jupyter Notebook environment):
    - `transformers`
    - `speech_recognition`
    - `nltk`
    - `textblob`
    - `spacy`
    - `torch` (for PyTorch backend)

### Installation

1. **Clone this repository** :
    ```sh
    git clone https://github.com/JermaineV/AI_Coach
    cd AI_Coach
    ```

2. **Install the required libraries**:
    ```sh
    pip install -r requirements.txt # To install the dependencies, you can simply run this line
    # OR individual installations
    pip install transformers speech_recognition nltk textblob spacy torch
    ```

3. **Download the necessary NLTK resources**:
    ```python
    import nltk
    nltk.download('punkt')
    ```

4. **(Optional) Install PyAudio for speech recognition**:
    - Download The necessary PyAudio file:
      ```sh
      pip install PyAudio
      ```

### Usage

1. **Open the Jupyter Notebook**:
    ```sh
    jupyter notebook AI_coach.ipynb
    ```

2. **Ensure you have a working internet connection for initial model downloads (if applicable)**.

3. **Run the notebook cells** (usually by pressing `Shift + Enter`) to execute the code.

## Current Functionality

- **Speech Recognition**: Capture and analyze user speech.
- **Text Analysis**: Perform sentiment analysis, keyword extraction, and named entity recognition.
- **LLM Integration**: Use pre-trained LLMs to generate responses based on user input.
- **Video Showcasing Current progress** [Video link](https://photos.onedrive.com/share/916B414DAF7F6FE4!5226?cid=916B414DAF7F6FE4&resId=916B414DAF7F6FE4!5226&authkey=!AOuQb0RbxwT6jjM&ithint=video&e=Amhrcv)
  
## Future Development

- Enhance response generation using the LLM with context awareness and conversation history.
- Integrate feedback mechanisms to improve the coach's responses over time.
- Explore additional features like voice synthesis for coach responses or sentiment visualization.

## Transformers and LLMs

The project utilizes the `transformers` library to interact with pre-trained LLMs.

### Transformers Library
- **Transformers Library:** [https://huggingface.co/transformers](https://huggingface.co/transformers)
- Install using `pip install transformers`

### Pre-trained LLM
The code snippet utilizes the `EleutherAI/gpt-j-6B` model. Explore the Hugging Face Model Hub for various LLMs: [https://huggingface.co/models](https://huggingface.co/models)

### Downloading the LLM

There are two main approaches to using pre-trained LLMs with the transformers library:

#### A. Using Transformers Pipeline
- **Pros:**
  - Simpler setup, no need to manage model files.
- **Cons:**
  - Requires an internet connection during script execution.
  - Might have limitations on model customization or fine-tuning.

#### B. Downloading Model Weights
- **Pros:**
  - Offline functionality after initial download.
  - More flexibility for fine-tuning or advanced usage.
- **Cons:**
  - Requires additional storage space for the model files.
  - Downloading large models can take time.

### Downloading Instructions
For option A (using pipeline), no additional downloads are necessary.

For option B (downloading weights), refer to the specific LLM's documentation on the Hugging Face Model Hub. Some models might provide pre-built transformers compatible weights files, while others may require specific download steps.

**Important Note:**
Downloading large LLMs can require significant storage space and processing power. Consider your computational resources and the specific needs of your project before choosing a model.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
