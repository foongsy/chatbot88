# Chatbot88 - Japanese AI Chatbot

A Japanese language chatbot built with Chainlit and powered by Google's Gemini 2.5 Flash Lite model through OpenRouter.

## Features

- **Japanese Language Support**: Configured to respond entirely in Japanese
- **Web-based Interface**: Built with Chainlit for an intuitive chat experience
- **Modern AI Model**: Uses Google's Gemini 2.5 Flash Lite for high-quality responses
- **Docker Support**: Containerized for easy deployment
- **Environment-based Configuration**: Secure API key management

## Tech Stack

- **Framework**: Chainlit 2.6.7
- **AI Model**: Google Gemini 2.5 Flash Lite
- **Model Provider**: OpenRouter
- **Language**: Python 3.13.3
- **Container**: Docker

## Prerequisites

- Python 3.13+
- Docker (optional)
- OpenRouter API key

## Setup

### 1. Clone the repository
```bash
git clone <repository-url>
cd chatbot88
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Environment Configuration
Create a `.env` file in the root directory:
```bash
OPENROUTER_API_KEY=your_openrouter_api_key_here
```

### 4. Run the application
```bash
chainlit run main.py
```

The chatbot will be available at `http://localhost:8000`

## Docker Deployment

### Build the image
```bash
docker build -t chatbot88 .
```

### Run the container
```bash
docker run -p 8080:8080 -e OPENROUTER_API_KEY=your_api_key chatbot88
```

The application will be accessible at `http://localhost:8080`

## Usage

1. Open the web interface in your browser
2. Start chatting in any language
3. The bot will respond in Japanese as configured

## Project Structure

```
chatbot88/
├── main.py              # Main application logic
├── requirements.txt     # Python dependencies
├── Dockerfile          # Docker configuration
├── chainlit.md         # Welcome screen content
├── README.md           # This file
└── .env               # Environment variables (create this)
```

## Configuration

The chatbot is configured with:
- **System Prompt**: "Please answer everything in japanese"
- **Model**: google/gemini-2.5-flash-lite
- **Provider**: OpenRouter with custom base URL

## Development

This project was created for a class on August 8th, 2025. It demonstrates:
- Integration of modern AI models with web interfaces
- Multi-language chatbot development
- Containerized deployment practices
- Environment-based configuration management

## License

This project is for educational purposes.
