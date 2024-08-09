# HoloBar Project

## Overview

HoloBar is an love project that I created for google's Hackathon that combines an Android application with a backend API to create an "immersive" AI-powered bar experience. Users can interact with AI agents representing various bar characters through text and voice, receiving responses in both audio and text formats. All the resources where created with AI, the only active thinking I did was for writing the python code and problem solving the code that LLMs provided. 

## Components

This repository consists of two main components:

1. **HoloBar Android App**: An Android application that provides the user interface and client-side processing for interacting with AI bar characters.

2. **AI Bar Agents API**: A FastAPI backend that handles the core logic for AI agent interactions and response generation.

## HoloBar Android App

The Android app is the front-end interface for users to interact with AI bar characters. 

Key features:
- Text and voice input support
- Text-to-speech synthesis using a custom VITS model
- Multiple AI agent personalities
- Background music playback
- Conversation history management

For more details, see the [HoloBar Android App README](./HoloAndroid/README.md).

## AI Bar Agents API

The FastAPI backend handles the processing of user inputs and generates appropriate responses from AI agents.

Key features:
- Voice and text-based interactions
- Real-time audio transcription
- Response monitoring and safety checks
- Google AI (Gemini) integration for natural language processing

For more details, see the [AI Bar Agents API README](./HoloFastApi/README.md).

## System Architecture

1. User interacts with the Android app through voice or text.
2. The app processes the input (speech-to-text if necessary) and sends it to the backend API.
3. The API processes the input, generates a response using the appropriate AI agent, and sends it back to the app.
4. The app converts the text response to speech using the VITS model and plays it back to the user.

## Setup

1. Clone this repository including submodules:
git clone --recurse-submodules https://github.com/your-repo-url.git

2. Set up the Android app:
- The code for the Android app was written 100% from LLMs. Same for configuring things and getting plugins
and dependencies. So I cannot give you instructions of how to deal with the code. The only thing that I want to mention is that if you want to use your own fastapi server, you need to change the calls. Although 

3. Set up the FastAPI backend:
- Follow the instructions in the [API README](./HoloFastApi/README.md).

4. Configure the Android app to communicate with your deployed API instance.

## Usage

1. Launch the HoloBar Android app on your device.
2. Choose an AI agent to interact with.
3. Speak or type your message to the AI agent.
4. Receive audio and text responses from the AI agent.

For detailed usage instructions, refer to the individual component READMEs.

## Development

- The Android app is primarily written in Kotlin.
- The backend API is implemented using FastAPI and Python.
- Both components use various AI and machine learning technologies, including custom VITS models and the Gemini API.


## License

This project is licensed under [Your chosen license]. See the [LICENSE](LICENSE) file for details.

## Support

If you encounter any issues or have questions, please file an issue on the GitHub repository.
