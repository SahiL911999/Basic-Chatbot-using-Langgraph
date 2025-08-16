# Basic Chatbot using LangGraph

A simple yet powerful chatbot implementation built with LangGraph, featuring conversation memory, state management, and integration with Groq's LLM models.

## 🚀 Features

- **Conversation Memory**: Maintains chat history across interactions
- **State Management**: Uses LangGraph's StateGraph for workflow management
- **LLM Integration**: Powered by Groq's llama-3.1-8b-instant model
- **Interactive Interface**: Console-based chat interface for easy testing
- **Checkpointing**: Persistent conversation state with memory saver

## 🛠️ Technologies Used

- **LangGraph**: For building stateful, multi-step applications
- **LangChain**: Core framework for LLM applications
- **Groq**: High-performance LLM inference platform
- **Python**: Core programming language
- **Jupyter Notebook**: Development and testing environment

## 📋 Prerequisites

- Python 3.8+
- pip package manager
- Groq API key

## 🔧 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/SahiL911999/Basic-Chatbot-using-Langgraph.git
   cd Basic-Chatbot-using-Langgraph
   ```

2. **Install required packages:**
   ```bash
   pip install langgraph langchain-groq langchain-core python-dotenv
   ```

3. **Set up environment variables:**
   Create a `.env` file in the project root and add your Groq API key:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   ```

## 🚀 Usage

1. **Open the Jupyter notebook:**
   ```bash
   jupyter notebook chatbot_using_Langgraph.ipynb
   ```

2. **Run all cells** to initialize the chatbot

3. **Start chatting** by typing messages in the console

4. **Exit the chat** by typing `exit`, `quit`, or `bye`

## 🏗️ Architecture

### Core Components

- **ChatState**: Typed dictionary managing conversation messages
- **chat_node**: Function that processes user input and generates AI responses
- **StateGraph**: LangGraph workflow defining the chat flow
- **MemorySaver**: Checkpoint system for conversation persistence

### Workflow

```
START → chat_node → END
         ↓
   Process messages
   Generate response
   Update state
```

## 💬 Example Conversation

```
User: my name is sahil
AI: Nice to meet you, Sahil. Is there something I can help you with or would you like to chat for a bit?

User: whats my name?
AI: Your name is Sahil.

User: add 10 to 15
AI: 15.

User: now add the result to 5
AI: Now I'll add the result (25) to 5: 25 + 5 = 30
```

## 🔑 Configuration

### Model Settings
- **LLM Model**: `llama-3.1-8b-instant` (Groq)
- **Thread ID**: Configurable for multiple conversation sessions
- **Checkpointing**: Enabled for conversation persistence

### Environment Variables
- `GROQ_API_KEY`: Your Groq API key for LLM access

## 📁 Project Structure

```
Basic-Chatbot/
├── chatbot_using_Langgraph.ipynb  # Main chatbot implementation
├── README.md                       # Project documentation
└── .env                           # Environment variables (create this)
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- [LangGraph](https://github.com/langchain-ai/langgraph) for the workflow framework
- [Groq](https://groq.com/) for high-performance LLM inference
- [LangChain](https://github.com/langchain-ai/langchain) for the LLM application framework

## 📞 Support

If you have any questions or need help with this project, please:

1. Check the [Issues](https://github.com/SahiL911999/Basic-Chatbot-using-Langgraph/issues) page
2. Create a new issue with a detailed description
3. Contact the maintainer

---

**Happy Chatting! 🤖💬**
