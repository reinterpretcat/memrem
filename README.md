# Memory Remains - Language Learning App

A static, serverless web application for learning foreign languages through flashcards, grammar lessons, and spaced repetition.

![Version](https://img.shields.io/badge/version-0.1.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## Overview

Memory Remains is a purely client-side web application designed for language learning. It features a comprehensive flashcard system with spaced repetition, grammar lessons, and progress tracking - all without any backend dependencies.

I've built it for myself using LLMs (I'm not a front-end SE) with the goal to prepare to B1 exam.

<img src="https://github.com/user-attachments/assets/71249f56-f491-4e3d-9b5a-8ba3affd45a1" width="400">
<img src="https://github.com/user-attachments/assets/ffc9a0b4-f9bd-4bc6-a264-afa04be5f048" width="400">
<img src="https://github.com/user-attachments/assets/e5db9da3-1416-4f45-8ed5-5896ee212da7" width="400">
<img src="https://github.com/user-attachments/assets/0ede464a-df06-4b21-b0cc-6dd23ecb76af" width="400">


## Features

### Core Functionality
- **File Explorer**: Browse language content organized the way you
- **Flashcard System**: Learn vocabulary and phrases through interactive flashcards
- **Spaced Repetition** (Experimental): Advanced SRS algorithm to optimize review intervals
- **Chat with LLM**: allows you to chat with LLM (via openrouter) and even generate a new cards based on your content which you can start learning in one click
<img src="https://github.com/user-attachments/assets/a0461ca0-003c-421e-ae9e-a32171363a90" width="400">
<img src="https://github.com/user-attachments/assets/0227280d-0314-40a3-8e39-49d9aabe743a" width="400">



### Technical Highlights
- Vanilla Javascript, HTML, CSS only with no external dependencies
- 100% client-side implementation (no server required)
- Markdown-driven content management
- Local storage for saving progress
- Full offline support
- Responsive design for desktop and mobile
- Dark/light theme support
- Build with LLM (vibe coding)

## Getting Started

### Installation

1. Clone the repository:
```bash
git clone https://github.com/reinterpretcat/memrem.git
cd memrem
```

2. Open the application:
   - Option 1: Open `index.html` directly in your browser (you will need to use workaround for CORS)
   - Option 2: Serve with a local HTTP server:
     ```bash
     # Using Python's built-in server
     python -m http.server
     ```

### Usage

1. **Exploring Content**:
   - Navigate through the file explorer to browse available lessons
   - Use keyboard (arrow keys) or touch/mouse to navigate
   - Select files or folders with Space or by clicking
   - Search for specific content with the search bar (Ctrl+F)

2. **Learning Cards**:
   - Select content files and click "Learn Cards"
   - Review flashcards one by one
   - Reveal answers and rate your recall difficulty
   - Track your progress with the built-in SRS system

3. **Settings**:
   - Configure app behavior through the settings panel (gear icon)
   - Adjust card behavior (shuffle, reversed mode)
   - Enable/disable spaced repetition
   - Filter content by tags
   - Change interface language

4. **Chat Features**:
   - Select content and use "Chat with LLM" to get AI assistance
   - Generate similar practice cards
   - Get grammar explanations
   - Create additional exercises

## Content Structure

Given content is only example, create and build your own content depending on what you're learning.

```
content/
├── index.md             # Main content index
└── b1_kurs/             # B1 level German course
    ├── 01-06/           # Lessons 1-6
    │   ├── 01_grammatik.md  # Grammar for lesson 1
    │   ├── 01_uebung.md     # Exercises for lesson 1
    │   └── ...
    └── 07-12/           # Lessons 7-12
        ├── 07_grammatik.md
        └── ...
```

## Content Format

Learning materials are stored in Markdown files with a standardized format:

```markdown
# Lesson Title

## Card Title
- Front side content (question)
* Back side content (answer)
> tag1, tag2, tag3
```

## Keyboard Shortcuts

- **Navigation**:
  - Arrow keys: Move between items
  - Enter: Navigate into folder/select file
  - Backspace: Navigate up a folder
  - Space: Toggle item selection
  - Ctrl+F: Search files

- **Card Learning**:
  - Space: Show answer
  - 1/E: Mark as Easy
  - 2/M: Mark as Medium
  - 3/H: Mark as Hard
  - Esc: Return to file explorer


## License

This project is licensed under the MIT License - see the LICENSE file for details.
