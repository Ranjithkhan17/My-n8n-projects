# AI Chat Agent Using n8n + Ollama + Memory

This workflow creates an AI-powered chat agent that uses local language models via Ollama with conversation memory.

## What This Workflow Does

- 🤖 **AI Chat Interface**: Provides a chat trigger for user interactions
- 🧠 **Memory Management**: Maintains conversation history using BufferWindow memory
- 🦙 **Ollama Integration**: Uses local Ollama models for language processing
- 💬 **Conversations**: Enables multi-turn conversations with AI

## Prerequisites

1. **Ollama** installed and running locally
2. **Model downloaded**: `llama3.2:1b` (or another model of your choice)
3. **n8n** running with Ollama integration

## Setup Instructions

### 1. Install Ollama
- Download from [ollama.ai](https://ollama.ai)
- Start the Ollama service: `ollama serve`

### 2. Pull a Model
```bash
ollama pull llama3.2:1b
```

### 3. Configure Ollama in n8n
- Go to n8n → Credentials
- Create new **Ollama** credential
- Set the base URL (usually `http://localhost:11434`)
- Note the credential ID

### 4. Setup Workflow
- Copy `AI Chat Agent using n8n + Ollama + Memory.json.template` to `AI Chat Agent using n8n + Ollama + Memory.json`
- Replace placeholders:
  - `YOUR_CHAT_WEBHOOK_ID_HERE`: Your chat webhook ID
  - `YOUR_OLLAMA_CREDENTIAL_ID`: Your Ollama credential ID from step 3
  - `YOUR_VERSION_ID_HERE`: Your version ID
  - `YOUR_INSTANCE_ID_HERE`: Your instance ID
  - `YOUR_WORKFLOW_ID_HERE`: Your workflow ID

## Testing

1. Deploy the workflow
2. Click on the chat widget to interact with the AI
3. Have a conversation with the bot!

## Customization

- **Change Model**: Modify the model name in "Ollama Chat Model" node
- **Adjust Memory**: Edit "Simple Memory" node to change memory window size
- **Customize Welcome**: Update "initialMessages" in the chat trigger

## Troubleshooting

- **Ollama Connection Error**: Ensure Ollama is running on `http://localhost:11434`
- **Model Not Found**: Run `ollama pull <model-name>` in terminal
- **Memory Issues**: Reduce model size if experiencing performance problems
