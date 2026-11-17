# PyLearn IDE

## Windows 11 Quick Start (PowerShell)

This project is a **static website**, not a Python package. There is no `pip install`, `requirements.txt`, `venv`, or Node build step. Install [Git](https://git-scm.com/downloads/win) and Python 3 if missing, then open PowerShell. Run **each command individually** in the folder where you want the project downloaded:

```powershell
git --version
```

```powershell
python --version
```

```powershell
git clone https://github.com/Tyler-Keesee/PyLearn-IDE.git
```

```powershell
Set-Location .\PyLearn-IDE
```

```powershell
python -m http.server 8000
```

With the server running, open **http://localhost:8000/** in Edge or Chrome. Press **Ctrl+C** in PowerShell to stop it.

**What to expect / caveats:** This is a browser-based educational Python IDE, not an installed Python desktop app. It uses browser-delivered libraries; internet access may be required for initial loads.

**Verification:** The HTTP server starting proves only that files are served; it does not prove every browser feature or third-party API is functioning. Open browser Developer Tools (F12) and check Console and Network for failures.

---


![PyLearn IDE logo](assets/logo.png)

[![Version](https://img.shields.io/badge/version-3.5.0-blue.svg)](https://github.com/Tyler-Keesee/PyLearn-IDE)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Stars](https://img.shields.io/github/stars/Tyler-Keesee/PyLearn-IDE?style=social)](https://github.com/Tyler-Keesee/PyLearn-IDE)

## 🚀 Next-Generation Python Learning Environment

PyLearn IDE is a cutting-edge, browser-based Python development environment specifically designed for educational purposes. It combines the power of modern web technologies with advanced visualization tools to create an immersive learning experience for Python programmers of all skill levels.

## ✨ Key Features

### 🔧 Core Functionality

- **Real-time Python Execution** - Run Python code directly in your browser using Brython
- **Intelligent Code Editor** - Syntax highlighting, auto-completion, and error detection
- **Interactive Console** - View output, errors with smart suggestions, and input support
- **Persistent Storage** - Automatically saves your code as you type

### 📊 Advanced Visualizations

- **Flow Diagram Generator** - Automatically visualizes your code execution flow
- **Data Structure Visualizer** - Graphically represents lists, dictionaries, and other data structures
- **Plot Generation** - Preview matplotlib-style plots directly in the browser
- **Memory Usage Analyzer** - Track memory consumption of your code

### 🎓 Learning Resources

- **Interactive Tutorials** - Step-by-step guides for Python concepts
- **Code Examples** - Pre-built examples for common programming tasks
- **Documentation Access** - Quick links to official Python documentation
- **Exercise Challenges** - Practice problems with automated verification

### 🛠️ Developer Tools

- **Dark/Light Theme** - Customizable UI themes for comfortable coding
- **File Operations** - Save, export, and share your code
- **Keyboard Shortcuts** - Productivity-enhancing shortcuts
- **Responsive Design** - Works on desktop and mobile devices

## 🖥️ Installation

### Local Setup

```bash
# Clone the repository
git clone https://github.com/Tyler-Keesee/PyLearn-IDE.git

# Navigate to the project directory
cd PyLearn-IDE

# If you have Python installed, you can use a simple HTTP server
python -m http.server

# Or use a Node.js server with live reload
npx serve
```

### Container setup

This repository does not currently include a Dockerfile. Use the local static-server setup above; do not run a `docker build` command until container packaging has been implemented and tested.

## 🎮 Usage

1. **Write Code** - Use the editor to write your Python code
2. **Run Code** - Click the "Run" button or press Ctrl+Enter
3. **View Output** - See the results in the console
4. **Explore Visualizations** - Toggle visualization panels to see your code in action
5. **Learn & Practice** - Access resources and examples to enhance your skills

## 📋 Code Examples

PyLearn IDE comes with pre-built examples for various programming concepts:

```python
# Basic Hello World
print("Hello, World!")

# Working with variables
name = input("Enter your name: ")
age = int(input("Enter your age: "))
print(f"Hello {name}, you are {age} years old!")

# Control flow example
numbers = [1, 2, 3, 4, 5]
for num in numbers:
    if num % 2 == 0:
        print(f"{num} is even")
    else:
        print(f"{num} is odd")
```

## 🔌 Integration Options (experimental / planned)

PyLearn IDE supports several integration options:

- **Embed in LMS** - Easily embed in Canvas, Moodle, or other learning platforms
- **API Access** - Programmatically interact with the IDE
- **Custom Plugins** - Extend functionality with your own plugins
- **Cloud Storage** - Connect to GitHub, Google Drive, or Dropbox

## 🧩 Advanced Features (proposals; availability not verified)

### AI-Powered Code Assistance

A potential AI assistant could:

- Suggest code improvements
- Explain code snippets
- Help debug errors
- Generate code from natural language descriptions

### Custom Visualization API

Create your own visualizations using our JavaScript API:

```javascript
// Example: Creating a custom visualization
pylearn.visualize({
  type: "network",
  data: myPythonVariable,
  options: {
    layout: "hierarchical",
    physics: true,
  },
});
```

### Collaboration Tools

- Real-time code sharing
- Collaborative editing
- Classroom management for educators
- Code review capabilities

## 🛣️ Roadmap (ideas, not shipped functionality)

- WebAssembly-based execution experiments
- Expanded code and data visualizations
- Optional code-assistance features
- Classroom and collaboration experiments

## 🤝 Contributing

We welcome contributions! Please check our [Contributing Guidelines](CONTRIBUTING.md) for details on how to submit pull requests, report issues, or request features.

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- [Brython](https://brython.info/) - Python in the browser
- [CodeMirror](https://codemirror.net/) - Versatile text editor
- [Vis.js](https://visjs.org/) - Network visualization
- [Chart.js](https://www.chartjs.org/) - Beautiful charts
- [Grid.js](https://gridjs.io/) - Data tables

---

<p align="center">Made with ❤️ by the PyLearn IDE Team</p>
<p align="center">© 2025 PyLearn IDE. All rights reserved.</p>
