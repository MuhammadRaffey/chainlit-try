# Chainlit Chat with Claude 3.5 Sonnet

A real-time chat application built with Chainlit and Anthropic's Claude 3.5 Sonnet model. This application provides an interactive chat interface where users can communicate with Claude, leveraging its advanced language capabilities.

## Features

- Real-time streaming responses from Claude 3.5 Sonnet
- Persistent chat session management
- Clean and intuitive web interface powered by Chainlit
- Asynchronous message handling

## Prerequisites

- Python 3.8 or higher
- An Anthropic API key
- UV package manager (recommended)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/MuhammadRaffey/chainlit-try
cd chainlit-try
```

2. Install dependencies using UV:

```bash
uv venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
uv sync
```

3. Set up your environment variables:

```bash
# On Windows
set ANTHROPIC_API_KEY=your_api_key_here

# On Unix/MacOS
export ANTHROPIC_API_KEY=your_api_key_here
```

## Usage

To start the application:

```bash
chainlit run src/chainlit_try/main.py
```

The application will be available at `http://localhost:8000` by default.

## Project Structure

```
chainlit-try/
├── src/
│   └── chainlit_try/
│       └── main.py      # Main application logic
├── requirements.txt     # Project dependencies
└── README.md           # Project documentation
```

## How It Works

1. When a chat session starts, a new message history is initialized.
2. User messages are sent to Claude 3.5 Sonnet via the Anthropic API.
3. Responses are streamed in real-time to the user interface.
4. The chat history is maintained throughout the session.

## Dependencies

- chainlit
- anthropic
- python-dotenv (recommended for environment variable management)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

[Add your license here]

## Acknowledgments

- [Chainlit](https://github.com/Chainlit/chainlit) for the chat interface framework
- [Anthropic](https://www.anthropic.com/) for Claude 3.5 Sonnet API



