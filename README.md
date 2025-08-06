# Snake Game LLM Tests 🐍

A collection of Snake games created by different Large Language Models to explore their code generation capabilities.

## The Experiment

This repository showcases how different LLMs interpret and execute the same simple request: creating a Snake game using HTML/CSS/JavaScript. It demonstrates the varying approaches, code quality, and visual polish that different models produce.

## The Models & Results

### 🤖 GPT-OSS (120B) - `snake_gptoss.html`
**Model:** GPT-OSS 120B running on server  
**Approach:** 3-shot prompting (initial request + 2 refinements)  
**Result:** Required iterative refinement to achieve a polished neon-styled game with smooth animations and overlays.

### 🎯 Qwen3 Coder (30B) - `snake_qwen3.html`
**Model:** Qwen3 Coder 30B (8-bit quantized) running locally  
**Approach:** Single-shot generation  
**Result:** Impressively complete and polished game on the first try, featuring gradient backgrounds, animated buttons, high score tracking with localStorage, and a professional UI.

### 🔥 Windsurf Pokemon Models - Enhanced Versions
The Windsurf test models (Bulbasaur, Charmander, Squirtle) were given the GPT-OSS output as a starting point with the prompt:  
*"This is a simple Snake Game in HTML/CSS/JS, can you spice this up significantly so it feels like a much prettier and more polished game."*

Each model took its own creative approach:
- **Bulbasaur:** Enhanced with glassmorphism effects and sophisticated visual polish
- **Charmander:** Added cyber-neon aesthetic with animated backgrounds
- **Squirtle:** Created an "Enhanced Edition" with advanced visual effects

## Key Findings

1. **Qwen3 Coder** demonstrated exceptional single-shot performance, producing production-ready code without refinement
2. **GPT-OSS** needed guidance but eventually delivered solid results
3. **Windsurf models** showed strong enhancement capabilities, each with unique stylistic choices

## How to Play

Simply open any HTML file in a web browser. Each game is self-contained with no external dependencies.

### Controls
- **Arrow Keys** or **WASD**: Move the snake
- **Space**: Start/Pause game (varies by implementation)

## Technical Notes

All games are:
- Zero-dependency (pure HTML/CSS/JavaScript)
- Self-contained in single files
- Responsive and playable in modern browsers
- Safe to run locally