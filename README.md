# AI Typing Assistant 🚀

A smart Python script that uses local AI to fix typos and formatting as you type!

## ✨ What It Does
- Press **F9** → Fixes the current line
- Press **F10** → Fixes selected text
- Uses your local AI (Ollama) to correct typos, casing, and punctuation

## 🛠 Setup

### 1. Install Ollama
```bash
# On Mac/Linux
curl -fsSL https://ollama.ai/install.sh | sh

# On Windows - download from https://ollama.ai/
```
### 2. Get AI Model
```bash
ollama pull mistral:7b-instruct-v0.2-q4_K_S
```

### 3. Install Python Packages
```bash
pip install httpx pynput pyperclip
```

## How to Run
1. art Ollama (in one terminal):
```bash
ollama serve
```

2. Run the script (in another terminal):
```bash
python your_script_name.py
```

3. Use it anywhere!
- Select text → Press F10
- Click on a line → Press F9

## Configuration
Edit these in the code if needed:
- Ollama URL: `http://localhost:11434`
- AI Model: `mistral:7b-instruct-v0.2-q4_K_S`
- Hotkeys: F9 and F10


## Troubleshooting
Hotkeys not working?

- Run VSCode as administrator
- Close other apps that might use F9/F10


Connection errors?
- Make sure `ollama serve` is running
- Check if port 11434 is available

Model errors?

```bash
ollama list  # See available models
ollama pull mistral:7b-instruct-v0.2-q4_K_S  # Download model
```

## Notes
- Works with any text editor/application
- Your data stays local - no internet needed!
- Currently configured for Mac keybindings
