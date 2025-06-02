## Meeting Notes AI Summarizer (Gemini API)

## Description
A simple Node.js backend that processes meeting notes (text or file) and returns summaries, decisions, and action items using Google Gemini AI.

## Setup

1. Clone repo and enter folder:
 - git clone https://github.com/vengadesh-max/AI-Powered-Meeting-info-Extractor.git

2. set directory
 - cd meeting-notes-ai

3. Install dependencies:
 - npm install

4. Create `.env` file with:
 - GEMINI_API_KEY=your_gemini_api_key_here
 - PORT=3001

## Run the app 
##### Terminal
1. set directory
 - cd meeting-notes-ai
2. Start the server:
 - node app.js

 - Output : ✅ Server running on port 3001


## Test

Send meeting notes as raw text:
 - curl -X POST http://localhost:3001/process-meeting -H "Content-Type: text/plain" -d "Your meeting notes here"

Or upload a `.txt` file:
 - curl -X POST http://localhost:3001/process-meeting -F "file=@test-notes/sample1.txt"

---

## Output

Returns JSON with summary, decisions, and action items.

![Screenshot (1757)](https://github.com/user-attachments/assets/985b889a-2b67-4219-abbc-aeec051795e8)


---

## Notes

- Ensure your Gemini API key is valid.
- Run curl commands from project root for file paths to work.
