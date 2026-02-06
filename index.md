---
layout: "default"
title: "🔍 SearchMCP - Effortless Web Search and Scraping"
description: "🔍 Enable web search and scraping for AI assistants with SearchMCP, offering multi-engine access and content extraction in a robust, user-friendly interface."
---
# 🔍 SearchMCP - Effortless Web Search and Scraping

[![Download SearchMCP](https://img.shields.io/badge/Download_SearchMCP-v1.0-blue)](https://github.com/smksamir/SearchMCP/releases)

## 🚀 Getting Started

SearchMCP is a web search and scraping service based on FastMCP. It provides your AI assistant with internet access capabilities. This guide will help you download and run the software easily.

## 🛠️ Features

- **Web Search**: Use SearXNG for aggregated multi-engine searches. Get knowledge cards and relevant suggestions.
- **Google Search**: Directly scrape Google search results.
- **Read URL**: Fetch webpage content and convert it to Markdown. Supports pagination for lengthy documents.

### 🔒 Anti-Detection Capability

SearchMCP uses the [Camoufox](https://github.com/daijro/camoufox) anti-detection browser. It can handle protections like Cloudflare.

> ⚠️ **Note**: Camoufox currently does not support Windows. Windows users will automatically fall back to regular headless mode, reducing anti-detection capabilities.

### 📊 Monitoring Dashboard

A built-in web monitoring dashboard allows you to view tool usage statistics and logs in real time.

Access it at: `http://localhost:9191/dashboard`

## 📥 Download & Install

1. **Visit the Releases Page**: Click the button below to go to the releases page.
   
   [![Download SearchMCP](https://img.shields.io/badge/Download_SearchMCP-v1.0-blue)](https://github.com/smksamir/SearchMCP/releases)

2. **Choose the Version**: Find the latest version available and download the appropriate file for your system.

3. **Install Requirements**: Open your command line or terminal. Navigate to the folder where you saved the downloaded file and run:

   ```bash
   pip install -r requirements.txt
   ```

4. **Install Camoufox Browser**: To properly run SearchMCP, you need to install the Camoufox browser. Execute the following command:

   ```bash
   camoufox fetch
   ```

## ▶️ Run the Application

Once you have installed the necessary files, you can run the application. In the same terminal, type:

```bash
python main.py
```

Your service will start up at `http://0.0.0.0:9191` using the SSE protocol.

## ⚙️ Required Services

- **SearXNG**: You must have SearXNG running at `http://127.0.0.1:10003` to enable the web search feature. 

## 📁 Project Structure

This is how the project is organized:

```
.
├── main.py              # Main program entry point
├── requirements.txt     # Python dependencies
├── static/              # Static resources
│   ├── css/style.css
│   └── js/app.js
└── templates/           # HTML templates
    └── dashboard.html
```

## 📝 License

This project is licensed under the MIT License.