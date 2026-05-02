# <div align="center">VeriCode 🛡️</div>

<div align="center">

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_AI-8E75B2?style=for-the-badge&logo=googlebard&logoColor=white)

**The Advanced AI-Powered Code Analysis Assistant**

🚀 **Analyze, Debug, and Optimize your code with the power of Hybrid AI.**

[Features](#-key-features) • [Installation](#-installation) • [Configuration](#-%EF%B8%8F-configuration) • [Usage](#-usage)

</div>

---

## 📖 Overview

**Vericode** is a modern web application designed to help developers write better code. By combining the speed of local LLMs (Phi-3 via GPT4All) with the depth of cloud-based AI (Google Gemini), Vericode offers a seamless, secure, and intelligent pair-programming experience.

Whether you need a quick syntax check or a deep architectural review, Vericode adapts to your needs.

---

## ✨ Key Features

- **🧠 Hybrid AI Engine**: Switch seamlessly between **Cloud (Gemini)** for complex tasks and **Local (Phi-3)** for privacy and offline capability.
- **💬 Intelligent Chat Interface**: Full markdown support, syntax highlighting, and conversation history.
- **🔐 Secure Authentication**: Robust JWT-based authentication with persistent sessions.
- **📂 Chat History Management**: automatic titling, search, rename, and delete functionalities for your conversations.
- **🎨 Modern UI/UX**: A stunning, dark-themed interface built with React, TailwindCSS, and Framer Motion.
- **👤 User Profiles**: customizable profiles with avatar support (Local/Cloudinary).

---

## 🛠️ Installation

Get Vericode up and running in minutes with our automated setup scripts.

### Prerequisites

- **Node.js** (v16+)
- **Python** (v3.10+) 
- **MongoDB** (Local or Atlas URI)

### 1. Clone the Repository

```bash
git clone https://github.com/OmPimple26/VeriCode---AI-Powered-Code-Quality-Analyzer-and-Refactoring-Suggestion-Tool.git
cd vericode
```

### 2. Environment Setup

Create a `.env` file in the `backend/` directory:

```env
# backend/.env

PORT=3000
MONGO_URI=mongodb://localhost:27017/vericode
DB_NAME=vericode
JWT_SECRET=your_super_secret_key_here

# AI Configuration
GEMINI_API_KEY=your_gemini_api_key
LLM_OP_MODE=cloud              # Options: 'cloud' or 'local'
GEMINI_MODEL=gemini-1.5-flash

# Optional: Cloudinary for Image Uploads
CLOUDINARY_CLOUD_NAME=...
CLOUDINARY_API_KEY=...
CLOUDINARY_API_SECRET=...
IMG_UPLOAD=local               # Options: 'local' or 'cloud'
```

### 3. Automatic Installation ⚡

We have provided a single command to install **Frontend dependencies**, **Backend dependencies**, **Python requirements**, and download the **Local LLM model**.

```bash
npm run install:all
```

> **Note**: This may take a few minutes as it downloads the ~2GB LLM model for local use.

---

## 🚀 Usage

Start the development servers for both Frontend and Backend with one command:

```bash
npm run dev
```

- **Frontend**: http://localhost:5173
- **Backend**: http://localhost:3000

---

## 📂 Project Structure

```bash
vericode/
├── frontend/          # React (Vite) Application
│   ├── src/
│   │   ├── pages/     # Chat, Auth, Settings, Home
│   │   ├── context/   # Auth Context
│   │   └── ...
├── backend/           # Node.js/Express API
│   ├── models/        # Mongoose Models (User, Chat)
│   ├── scripts/       # Python Scripts (Local LLM)
│   ├── llmModel/      # Downloaded GGUF Models
│   └── ...
└── package.json       # Root scripts
```

---

<div align="center">

Made with ❤️ by [Om](https://github.com/OmPimple26)

</div>
