# 🚀 Ryuu Studio Pro v1.8.9

> A powerful browser-based code editor with AI assistant, multi-language support, and full terminal input handling. Built by an 11-year-old coder! 🔥

![Version](https://img.shields.io/badge/version-1.8.9-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Made by](https://img.shields.io/badge/made%20by-Ryuu-orange)

![Screenshot](screenshot.png)

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 📝 **Monaco Editor** | The same editor that powers VS Code! |
| 🤖 **Xzetron Ultra AI** | Real AI coding assistant (Zhipu API) |
| 🖥️ **Full Input Support** | `input()`, `scanf()`, `cin`, `Scanner` all work! |
| 🌍 **Multi-Language** | JavaScript, Python, C, C++, Java |
| 🎨 **Dark/Light Themes** | Easy on the eyes, day or night |
| 📁 **File Explorer** | Organize your code like a pro |
| 🖱️ **Integrated Terminal** | Run commands and see output |
| 📋 **Copy Code Button** | One-click copy from AI responses |
| ⌨️ **Keyboard Shortcuts** | Full VS Code-style shortcuts |
| 💾 **Auto-Save** | Never lose your work |

---

## 🎮 Demo / Example

Open `example_game.js` in the `src` folder – it's a fully working number guessing game:

```javascript
// Number Guessing Game
async function playGame() {
    console.log("🎮 Welcome to the Number Guessing Game!");
    let secretNumber = Math.floor(Math.random() * 100) + 1;
    let attempts = 0;
    let guessed = false;
    
    while (!guessed) {
        let guess = await input("Enter your guess (1-100): ");
        guess = parseInt(guess);
        attempts++;
        
        if (guess < secretNumber) console.log("Too low!");
        else if (guess > secretNumber) console.log("Too high!");
        else {
            console.log(`🎉 Correct! ${attempts} attempts!`);
            guessed = true;
        }
    }
}
