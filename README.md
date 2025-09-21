# VidSnap AI

VidSnap AI is a web application that allows users to create engaging Instagram Reels using AI-powered text-to-speech and video processing. Upload images, add your own text, and generate a vertical video reel with voiceover and music.

## Features

- Upload multiple images to create a video reel
- Add custom text to be converted into AI-generated voiceover
- Automatic video formatting for Instagram Reels (1080x1920)
- Gallery to view generated reels
- Clean, modern UI with responsive design

## How It Works

1. **Upload Images:** Go to the "Create Reel" page and upload your images.
2. **Add Text:** Enter the text you want to be spoken in the reel.
3. **Generate Reel:** Submit the form. The backend will:
   - Save your images and text
   - Convert your text to speech using ElevenLabs API
   - Generate a video using ffmpeg, combining your images and audio
4. **View Gallery:** Visit the Gallery to see all generated reels.

## Setup

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/vidsnap-ai.git
   cd vidsnap-ai
   
2. **Install dependencies:**
   ```sh
   pip install flask python-dotenv elevenlabs
   
3. **Configure API Keys:**
    - Set your ElevenLabs API key in config.py:
    ```sh
    ELEVENLABS_API = "YOUR_API_KEY"

4. **Start the background process:**
    ```sh
    python generate_process.py

5. **Run the Flask server:**
    ```sh
    python main.py

6. **Visit the app:**
- Open http://localhost:5000 in your browser.
