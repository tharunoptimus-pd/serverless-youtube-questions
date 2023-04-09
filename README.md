# Questions Generator for YouTube Videos - Serverless

It uses `youtube-transcript-api` to get the captions from YouTube. Then it separates the captions into 5 chunks and generates questions for each chunk. It uses a deployed [Hugging Face model](https://currentlyexhausted-question-generator.hf.space) to generate the questions.

It uses Vercel Serverless Function to run the flask server. Hopefully in under 10 seconds.

## Installation

```bash
pip install -r requirements.txt
```

## Usage

```bash
python app.py
```

## Endpoints
- `/` **POST** 
    - body: {"youtubeVideoId": "g0amdIcZt5I"}
- `any` **GET**
