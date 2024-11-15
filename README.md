## Accessibility App

## Overview
The Accessibility App is a Chrome extension designed to make websites more accessible. It includes the following features:

- **Text Summarization**: Summarizes the content of a selected paragraph.
- **Text-to-Speech**: Converts the summarized text into speech for visually impaired users.
- **AI Chatbot**: Allows users to ask further questions related to the summarized text.

## Features

- **Text Summarization**: Select any paragraph of text on a webpage, and the app will summarize it.
- **Text-to-Speech**: Listen to the summary by clicking the "Play" button.
- **AI Chatbot**: Ask further questions to clarify the summary or explore more details.

## Requirements

To run this project, you’ll need the following:

- **Google Chrome** browser
- **OpenAI API Key**: You need to obtain an API key from OpenAI to enable the text summarization and chatbot functionality.

## Installation

1. Clone this repository to your local machine:

2. Install dependencies:

    - If you're using a Node.js environment, install any necessary dependencies (like `axios` if you use it for making requests) by running:

3. Add your OpenAI API key:
    - Open the `background.js` file.
    - Replace the placeholder text `YOUR_OPENAI_API_KEY` with your actual OpenAI API key.

    Example:

    ```javascript
    const apiKey = 'YOUR_OPENAI_API_KEY';
    ```

    You can obtain an API key by signing up at [OpenAI](https://platform.openai.com/signup).

## Usage

1. Load the extension in Chrome:
    - Open Chrome and go to `chrome://extensions/`.
    - Enable **Developer mode**.
    - Click on **Load unpacked** and select the extension’s directory.

2. Once the extension is loaded:
    - Highlight any paragraph on a webpage.
    - Right-click to access the **Summarize** option in the context menu.
    - The summary will be displayed in a popup with the option to listen to it using the text-to-speech feature.

3. Click the **Play** button to listen to the summary.

## Troubleshooting

- If the text-to-speech functionality isn't working, ensure that the `SpeechSynthesis` API is supported by your browser.
- If the summarization isn't working, check your OpenAI API key and ensure you have the correct permissions.
