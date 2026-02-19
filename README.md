# ollama-claude-code-free
Run Anthropic's Claude Code CLI for free using Ollama + local models (qwen2.5-coder, glm-4.7, devstral, etc.). Full offline coding agent write, edit, test, debug code directly in your terminal. No API keys, no subscription.
# Ollama + Claude Code: Free & Local Coding Agent

Run a **Claude Code**-style terminal coding agent **100% free and offline** using Ollama + powerful open models.

No Anthropic API, no monthly fees, no internet required after model download.

## What is this?

This guide shows how to use **Claude Code** (Anthropic's official CLI coding agent) but powered by free local LLMs via Ollama instead of paid Claude.

You get:
- Writes/edits files directly in your folder (with approval)
- Runs/tests/debugs code (with approval)
- Plans multi-step tasks
- Fixes bugs in loops
- Works offline on your GPU/CPU

All with models like qwen2.5-coder, glm-4.7-flash, devstral-small — often close to Claude 3.5/4 quality for coding.

## Requirements

- Ollama installed → https://ollama.com/download
- Decent GPU recommended (RTX 3060+ for fast responses; CPU works but slow)
- Python (only needed if you want to extend it later)

## Quick Setup (5 minutes)

1. Install Ollama (if not already)  
   https://ollama.com/download

2. Pull a strong coding model (choose one):

   ```bash
   ollama pull qwen2.5-coder:7b          # Very strong, best balance
   # or
   ollama pull glm-4.7-flash             # Fast & smart
   # or
   ollama pull devstral-small            # Optimized for coding agents
