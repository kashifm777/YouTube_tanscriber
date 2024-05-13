# YouTube Transcript Summarizer with Streamlit

This Streamlit web app leverages Google's GenerativeAI service (Gemini Pro) to automatically summarize YouTube videos based on their transcripts.

## Streamlit  

You can try the app on Streamlit Server:  
[YouTube Transcriber](https://youtube-transcriber-mk.streamlit.app)

## 1. Features

- **YouTube Link Input:** Enter the URL of a YouTube video.
- **Video Preview:** See a thumbnail image of the selected video.
- **AI-powered Summarization:** Gemini Pro analyzes the video transcript and generates a concise summary with key points.
- **Detailed Notes:** The summary is presented in a clear and easy-to-read format.

## 2. Requirements

- Python 3.x
- Streamlit (`pip install streamlit`)
- `dotenv` library (`pip install python-dotenv`)
- `youtube-transcript-api` library (`pip install youtube-transcript-api`)
- Google Cloud Project with GenerativeAI API enabled ([https://cloud.google.com/ai/generative-ai](https://cloud.google.com/ai/generative-ai))

## 3. Setup

1. Create a virtual environment (recommended): `python -m venv venv`
2. Activate the environment: `source venv/bin/activate` (Windows: `venv\Scripts\activate`)
3. Install dependencies: Refer to the requirements section and install the necessary libraries.
4. Create a `.env` file in the project directory:
   - Add `GOOGLE_API_KEY=<YOUR_API_KEY>` (replace with your API key)

## 4. Running the App

1. Open a terminal in the project directory.
2. Run the app: `streamlit run app.py`
3. Access the app in your web browser at http://localhost:8501.

## 5. Usage

1. Paste the URL of a YouTube video in the input field.
2. Click the "Get Detailed Notes" button.
3. The app will display a thumbnail image of the video and, if successful, a detailed summary of the video content extracted from the transcript.

## 6. Disclaimer

- This is a basic example using a free-tier API. The accuracy and detail of summaries may vary.
- Consider the limitations of natural language processing and the quality of YouTube transcripts for the best results.

## 7. Note

- This README assumes you have completed initial setup and configured your Google Cloud Project with the GenerativeAI API.