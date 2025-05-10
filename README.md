# 🤖 Gemini LLM + LangChain Playbook  
**A structured and hands-on guide to mastering Google Generative AI models using LangChain**

[![LangChain](https://img.shields.io/badge/LangChain-Framework-blue)](https://www.langchain.com/)
[![Google Gemini](https://img.shields.io/badge/Google%20Gemini-LLM-red)](https://ai.google.dev/)
[![Colab Ready](https://img.shields.io/badge/Google%20Colab-Compatible-yellow)](https://colab.research.google.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📚 Overview

This repository serves as a modular and practical **playbook** for using [Google Generative AI (Gemini)](https://ai.google.dev/) models via [LangChain](https://python.langchain.com) — tailored for learners, builders, and portfolio builders.

> ✅ **Focus**: Functional demos — not production apps  
> ✅ **Style**: Clean, structured, and Colab-friendly  
> ✅ **Audience**: AI developers, LangChain explorers, ML hobbyists

---

## 🗂️ Repository Structure

```bash
gemini-llm-langchain-playbook/
├── modules/                            # 📚 Core modules and demos
│   ├── README.md                       # 📑 General explanation of the 'modules' folder structure and purpose
│   ├── google_generative_ai/           # 📌 Basic usage of the GoogleGenerativeAI class
│   │   ├── README.md                   # 📑 Explanation of the basic usage of GoogleGenerativeAI
│   │   ├── demo_invoke.ipynb           # 🔹 Demo of the Invoke usage
│   │   ├── demo_batch.ipynb            # 🔹 Demo of the Batch usage
│   │   ├── demo_async.ipynb            # 🔹 Demo of the Async usage
│   │   ├── demo_stream.ipynb           # 🔹 Demo of the Stream usage
│   │   └── utils.py                    # 🔧 Utility functions supporting basic usage
│   ├── chat_google_genai/              # 💬 Chat model integration (Coming Soon)
│   │   ├── README.md                   # 📑 Explanation of ChatGoogleGenerativeAI and chat workflows
│   │   ├── demo_chat_workflow.ipynb    # 💬 Example of implementing chat with Gemini
│   │   └── utils.py                    # 🔧 Supporting functions and classes for chat workflows
│   ├── tools/                          # 🛠️ Gemini + LangChain Tools demo
│   │   ├── README.md                   # 📑 Explanation of using Gemini with LangChain tools
│   │   ├── demo_tools_integration.ipynb # 🛠️ Example of integrating Gemini tools with LangChain
│   │   └── utils.py                    # 🔧 Supporting functions for tools integration
│   └── memory/                         # 🧠 Demo of memory usage with Gemini
│       ├── README.md                   # 📑 Explanation of using memory in LangChain with Gemini
│       ├── demo_memory_chain.ipynb     # 🧠 Example of using memory in a Gemini workflow
│       └── utils.py                    # 🔧 Supporting functions for memory usage
├── assets/                             # 📸 Diagrams & screenshots
├── requirements.txt                    # 🔧 Dependencies list
├── LICENSE                             # 📜 License information
└── README.md                           # 📘 You're here! Main documentation file
```

## 🧪 Core Modules & Demos

| 📁 Module               | 📋 Description                                                  | 📓 Notebooks                        |
|------------------------|------------------------------------------------------------------|-------------------------------------|
| `google_generative_ai` | Demonstration of `GoogleGenerativeAI` class in LangChain        | 🔹 Invoke, Stream, Batch, Async     |
| `chat_google_genai`    | *(Coming Soon)* Conversational AI using `ChatGoogleGenerativeAI` | 🔸 Chat workflows                   |
| `tools`                | Example of Gemini integrated with LangChain tools and agents     | 🔸 Tool usage + parsing             |
| `memory`               | Shows how Gemini can retain and use memory via LangChain         | 🔸 Memory chains                    |

---

## 🚀 Getting Started

### 🔧 1. Install Dependencies
```bash
pip install -r requirements.txt
```
### 📥 2. Enable Google Generative AI (Gemini)

Get your Gemini API key from:  
👉 [https://makersuite.google.com/app/apikey](https://makersuite.google.com/app/apikey)

#### 🔐 Set API Key

Set it as an environment variable (Linux/macOS):

```bash
export GOOGLE_API_KEY=your_api_key_here
```
Or set it directly in your notebook or Python script:
```bash
import os
os.environ["GOOGLE_API_KEY"] = "your_api_key_here"
```
---
## 🧠 Features Demonstrated

- 🎯 **Simple Usage** → `.invoke()`
- 🚀 **Batch Processing** → `.batch()`
- 🔁 **Async Execution** → `.ainvoke()` / `.abatch()`
- 🛰️ **Streaming Output** → `.stream()` / `.astream()`
- 🧩 **Prompt Integration** → `PromptTemplate`
- 📊 **Token & Metadata Inspection** → `response.generation_info`
- 🧠 **(Soon)** Memory Chains for conversational state
- 🛠️ **(Soon)** Tool + Agent integration for advanced flows
---
## 🌐 Run on Google Colab

Each notebook is designed to be **Colab-friendly**.  
Just click the badge below to open in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/your-username/gemini-llm-langchain-playbook)

> ⚠️ **Note:** Update the `your-username` part with your GitHub username once the repo is public.
---
## 📸 Screenshots & Visuals

Explore visual outputs, diagrams, and real-time streaming previews of the models. These resources will be placed in the `assets/` folder for easy access.

Below are some visual representations of the demo processes:

![Example Visual 1](assets/example_image1.png)
*Example of streaming output in real-time.*

![Example Visual 2](assets/example_image2.png)
*Diagram showing integration of GoogleGenerativeAI with LangChain tools.*

> 📌 **Note:** Preview images will be uploaded soon, and we are working on adding more visual content to enhance understanding.
---
## 📜 License

This project is licensed under the **MIT License**.

MIT © 2025 — Built with ❤️ for **educational** and **portfolio** purposes.

> Feel free to use, modify, and distribute this project for personal or educational purposes. Contributions and improvements are welcome via issues and pull requests.
---
## 🙋‍♂️ Contribute / Follow-up

This repository serves as a personal learning log and portfolio showcase. If you would like to suggest improvements, submit corrections, or ask any questions, feel free to:

- 🐛 **Open an Issue**  
  If you encounter bugs, have suggestions, or want to discuss improvements, please open an issue in the repository.

- ⭐ **Star the Repository**  
  If you find this project helpful or inspiring, consider starring it on GitHub. It helps me track the project’s popularity and motivates me to continue improving it.

- 💬 **Reach Out via Discussions**  
  Join the conversation by participating in the discussions section. Feel free to share your thoughts, ask questions, or provide feedback on this project.
