# Legal AI Assistant for Law Enforcement

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![Rasa](https://img.shields.io/badge/Rasa-3.6.2-purple)

---

## 🎬 Demo Video

> **Watch the project demo:**  
> [▶️ Download & Play Demo --Version 01.mkv](../Demo%20--Version%2001.mkv)
>
> _Note: GitHub does not support direct playback of .mkv files. Download and play locally for best experience._

---

## 🖼️ Screenshots

| Login Page | Chat Page |
|:----------:|:---------:|
| ![Login](../Test%20Output's/Frontend/loginpage.png) | ![Chat](../Test%20Output's/Frontend/Chatpage.png) |

---

## 🗂️ Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [Tech Stack](#tech-stack)
- [Directory Structure](#directory-structure)
- [Setup & Installation](#setup--installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## 📝 Overview
**Legal AI Assistant for Law Enforcement** is an advanced AI-powered platform designed to streamline legal research, FIR management, and intelligent query handling for law enforcement agencies and legal professionals. Leveraging Rasa, FastAPI, and modern NLP, it provides:
- Natural language legal query resolution
- Automated FIR and IPC section management
- A user-friendly web chat interface
- Robust backend for data scraping, database population, and analytics

---

## 🚀 Features
- **AI Chatbot:** Natural language interface for legal queries (IPC, crimes, punishments)
- **FIR Management:** Create, view, and administer First Information Reports
- **IPC Section Search:** Fast lookup and analysis of Indian Penal Code sections
- **Admin Panels:** Manage IPC and FIR data via web UI
- **Automated Scraping:** Scripts to fetch and update legal data
- **Extensible:** Modular codebase for easy feature addition
- **Secure:** Credentials and config management
- **Tested:** Includes unit and integration tests

---

## 🏗️ Architecture

![Use Case Diagram](../Documentation/Diagrams/Use%20Case%20Diagram.png)
![Data Flow Diagram](../Documentation/Diagrams/Data%20Flow%20Diagram.png)

---

## 🛠️ Tech Stack
- **Backend:** Python 3.8+, FastAPI, Rasa 3.6.2
- **Database:** MySQL
- **NLP:** Rasa NLU, custom actions
- **Frontend:** HTML, CSS, JS (static)
- **Scraping:** Selenium
- **Other:** Jinja2, Websockets, Socket.IO

---

## 📁 Directory Structure
```
chat/
├── actions/                # Custom Rasa actions
├── data/                   # Rasa NLU, stories, rules
├── models/                 # Trained Rasa models
├── rasa/                   # Rasa project files
├── rasa_data/              # Additional Rasa data
├── static/                 # Frontend static files (HTML, SVG, etc.)
├── tests/                  # Test cases and test data
├── results/                # Output and result files
├── *.py                    # Core backend scripts (API, DB, scraping, etc.)
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation
├── LICENSE                 # MIT License
```

---

## ⚡ Setup & Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Babureddy009/Legal-AI-Assistant-For-Law-Enforcement.git
   cd Legal-AI-Assistant-For-Law-Enforcement/chat
   ```
2. **Create and activate a virtual environment:**
   ```bash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On Unix/Mac:
   source venv/bin/activate
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Configure environment variables:**
   - Copy `.env.example` to `.env` and update as needed (if applicable).
5. **Set up the database:**
   - Run the provided SQL scripts in your MySQL instance.
   - Update connection details in config files if needed.
6. **Train the Rasa model:**
   ```bash
   rasa train
   ```
7. **Run the backend services:**
   - Start Rasa server:
     ```bash
     rasa run --enable-api
     ```
   - Start FastAPI server:
     ```bash
     uvicorn chat:app --reload
     ```

---

## 💡 Usage
- Access the web chat interface via your browser (see `static/about.html` or main app entrypoint).
- Use the API endpoints for programmatic access (see `api_client.py` and FastAPI docs).
- Refer to the `data/` and `rasa_data/` folders for NLU and story customization.

---

## 🤝 Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

---

## 📄 License
MIT License. See [LICENSE](LICENSE) for details.

---

## 📬 Contact
For questions, feedback, or collaboration:
**Babureddy B N**  
📧 babureddy2603@gmail.com

---
*Developed by Babureddy B N, 2025* 