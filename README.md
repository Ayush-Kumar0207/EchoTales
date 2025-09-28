
# 🤖 EchoTales - AI Story & Narration Generator 📖

Transform a series of images into a captivating, AI-generated story with accompanying audio narration. This application uses the power of Google's Gemini model to analyze your images and weave them into a coherent narrative based on your chosen genre.

## ✨ Features

* **Visual Storytelling**: Generates a single, coherent story from a sequence of 1 to 10 images.
* **Genre Selection**: Tailor the story's tone by choosing from styles like Comedy, Thriller, Fairy Tale, Sci-Fi, Mystery, Adventure, and Morale.
* **Dynamic Prompting**: The AI prompt is intelligently customized based on the selected genre to include unique elements, like a `[SOLUTION]:` for a mystery, a `[MORAL]:` for a morale-based story, or a `[TWIST]:` for a thriller.
* [cite_start]**AI-Powered Narration**: Converts the generated story into speech using Google Text-to-Speech (gTTS). The final audio is displayed in the app.
* **Indian Context**: The AI is specifically prompted to use only Indian names, characters, and places in the narrative.
* [cite_start]**Simple Web Interface**: An intuitive and user-friendly interface built with Streamlit.

---

## ⚙️ How It Works

The application follows a simple workflow:

1.  **Image Upload & Style Selection**: The user uploads multiple images and selects a story genre through the Streamlit web interface's sidebar.
2.  **AI Story Generation**:
    * The images and a dynamically generated prompt from `story_generator.py` are sent to the Google Gemini API's `gemini-2.5-flash-lite` model.
    * The prompt instructs the AI to act as a storyteller, connect all images in order, and adhere to the chosen genre's conventions.
3.  **Text-to-Speech Conversion**:
    * The story text returned by the API is passed to the `narrate_story` function.
    * This function uses the `gTTS` library to convert the text into an MP3 audio file in memory using `BytesIO`.
4.  **Display Results**: The generated story and an embedded audio player are displayed on the Streamlit frontend for the user to read and listen to.

---

## 🛠️ Tech Stack

* **Backend / AI Logic**: Python
* [cite_start]**Generative AI Model**: Google Gemini (`google-genai`, `google-generativeai`) 
* [cite_start]**Web Framework**: Streamlit 
* [cite_start]**Text-to-Speech**: gTTS 
* [cite_start]**Image Processing**: Pillow 
* [cite_start]**Environment Variables**: `python-dotenv` 

---

## 🚀 Getting Started

Follow these instructions to set up and run the project locally.

### Prerequisites

* Python 3.8+
* A Google API Key. You can get one from [Google AI Studio](https://makersuite.google.com/app/apikey).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/ai-story-generator.git](https://github.com/your-username/ai-story-generator.git)
    cd ai-story-generator
    ```

2.  **Create and activate a virtual environment (recommended):**
    * **On macOS/Linux:**
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```
    * **On Windows:**
        ```bash
        python -m venv venv
        .\venv\Scripts\activate
        ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    [cite_start][cite: 1]

4.  **Set up your environment variables:**
    * Create a new file named `.env` in the root of your project directory.
    * Add your Google API key to this file. `load_dotenv()` is called to load it.
        ```
        GOOGLE_API_KEY="YOUR_API_KEY_HERE"
        ```

### Usage

1.  **Run the Streamlit application:**
    ```bash
    streamlit run app.py
    ```
   

2.  **Open the application in your browser:**
    * Navigate to the local URL provided in the terminal (usually `http://localhost:8501`).

3.  **Create your story:**
    * Use the sidebar to upload your images (`png`, `jpg`, `jpeg`).
    * Select a story style from the dropdown menu.
    * Click the "Generate Story and Narration" button and wait for the process to complete.

---

## 📂 Project Structure
Markdown

# 🤖 AI Story & Narration Generator 📖

Transform a series of images into a captivating, AI-generated story with accompanying audio narration. This application uses the power of Google's Gemini model to analyze your images and weave them into a coherent narrative based on your chosen genre.

## ✨ Features

* **Visual Storytelling**: Generates a single, coherent story from a sequence of 1 to 10 images.
* **Genre Selection**: Tailor the story's tone by choosing from styles like Comedy, Thriller, Fairy Tale, Sci-Fi, Mystery, Adventure, and Morale.
* **Dynamic Prompting**: The AI prompt is intelligently customized based on the selected genre to include unique elements, like a `[SOLUTION]:` for a mystery, a `[MORAL]:` for a morale-based story, or a `[TWIST]:` for a thriller.
* [cite_start]**AI-Powered Narration**: Converts the generated story into speech using Google Text-to-Speech (gTTS). The final audio is displayed in the app.
* **Indian Context**: The AI is specifically prompted to use only Indian names, characters, and places in the narrative.
* [cite_start]**Simple Web Interface**: An intuitive and user-friendly interface built with Streamlit.

---

## ⚙️ How It Works

The application follows a simple workflow:

1.  **Image Upload & Style Selection**: The user uploads multiple images and selects a story genre through the Streamlit web interface's sidebar.
2.  **AI Story Generation**:
    * The images and a dynamically generated prompt from `story_generator.py` are sent to the Google Gemini API's `gemini-2.5-flash-lite` model.
    * The prompt instructs the AI to act as a storyteller, connect all images in order, and adhere to the chosen genre's conventions.
3.  **Text-to-Speech Conversion**:
    * The story text returned by the API is passed to the `narrate_story` function.
    * This function uses the `gTTS` library to convert the text into an MP3 audio file in memory using `BytesIO`.
4.  **Display Results**: The generated story and an embedded audio player are displayed on the Streamlit frontend for the user to read and listen to.

---

## 🛠️ Tech Stack

* **Backend / AI Logic**: Python
* [cite_start]**Generative AI Model**: Google Gemini (`google-genai`, `google-generativeai`) 
* [cite_start]**Web Framework**: Streamlit 
* [cite_start]**Text-to-Speech**: gTTS 
* [cite_start]**Image Processing**: Pillow 
* [cite_start]**Environment Variables**: `python-dotenv` 

---

## 🚀 Getting Started

Follow these instructions to set up and run the project locally.

### Prerequisites

* Python 3.8+
* A Google API Key. You can get one from [Google AI Studio](https://makersuite.google.com/app/apikey).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/ai-story-generator.git](https://github.com/your-username/ai-story-generator.git)
    cd ai-story-generator
    ```

2.  **Create and activate a virtual environment (recommended):**
    * **On macOS/Linux:**
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```
    * **On Windows:**
        ```bash
        python -m venv venv
        .\venv\Scripts\activate
        ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    [cite_start][cite: 1]

4.  **Set up your environment variables:**
    * Create a new file named `.env` in the root of your project directory.
    * Add your Google API key to this file. `load_dotenv()` is called to load it.
        ```
        GOOGLE_API_KEY="YOUR_API_KEY_HERE"
        ```

### Usage

1.  **Run the Streamlit application:**
    ```bash
    streamlit run app.py
    ```
   

2.  **Open the application in your browser:**
    * Navigate to the local URL provided in the terminal (usually `http://localhost:8501`).

3.  **Create your story:**
    * Use the sidebar to upload your images (`png`, `jpg`, `jpeg`).
    * Select a story style from the dropdown menu.
    * Click the "Generate Story and Narration" button and wait for the process to complete.

---

## 📂 Project Structure
```
.
├── app.py              # Main Streamlit application file
├── story_generator.py  # Core logic for interacting with Gemini API and gTTS
├── requirements.txt    # Project dependencies
└── .env                # For storing API keys (needs to be created by you)
```
