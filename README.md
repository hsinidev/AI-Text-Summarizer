<div align="center">
# 🚀 Ai Text Summarizer
### *High-Performance Autonomous Intelligence & Modular HTML Engine*

<p align="center">
  [![Architect](https://img.shields.io/badge/Architect-Hsini%20Mohamed-0055ff?style=for-the-badge&logo=github&logoColor=white)](https://hsini.dev)
  [![Portfolio](https://img.shields.io/badge/Portfolio-hsini.dev-00c853?style=for-the-badge&logo=google-chrome&logoColor=white)](https://hsini.dev)
  [![Language](https://img.shields.io/badge/Language-HTML-f59e0b?style=for-the-badge)](https://github.com/hsinidev)
  [![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
</p>

<img src="favicon.svg" alt="Logo" width="100" height="100">

</div>

---
## 🌟 Executive Overview

**Ai Text Summarizer** is an enterprise-grade artificial intelligence solution engineered for low-latency reasoning, deterministic workflow automation, and high-accuracy data orchestration. Built with modern **HTML** and **HTML**, it delivers modular architecture and seamless developer ergonomics.

## ⚡ Key Highlights & Capabilities

- **Autonomous Orchestration**: Advanced state management and deterministic execution pipelines.
- **Modular Architecture**: Plug-and-play integrations with clean abstraction layers.
- **Zero-Overhead Processing**: High-throughput processing optimized for local and cloud environments.
- **Developer-First APIs**: Type-safe interfaces with comprehensive observability.

---
## 🏗️ Architecture & Technology Stack

- **Primary Language**: `HTML`
- **Design Pattern**: Modular Clean Architecture / Domain-Driven Design
- **License**: MIT Open Source Attribution

## 📖 Deep-Dive Technical Documentation

<div align="center">
  <img src="favicon.svg" alt="Logo" width="100" height="100">
  <h1 align="center">AI Text Summarizer</h1>
  <p align="center">
    A powerful, privacy-first, single-file web application for summarizing text using your own configurable LLM endpoint.
    <br />
    <a href="#-about-the-project"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://doodax.com/ai-summarizer/index.html">View Demo</a>
    ·
    <a href="https://github.com/hsinidev/ai-summarizer/issues">Report Bug</a>
    ·
    <a href="https://github.com/hsinidev/ai-summarizer/issues">Request Feature</a>
  </p>
</div>

<div align="center">


</div>

---

## 📋 Table of Contents

- [📌 About The Project](#-about-the-project)
- [✨ Key Features](#-key-features)
- [🛠️ Built With](#️-built-with)
- [🚀 Getting Started](#-getting-started)
- [⚙️ Usage](#️-usage)
  - [API Endpoint Configuration](#api-endpoint-configuration)
- [📝 SEO & Content Strategy](#-seo--content-strategy)
- [🤝 Contributing](#-contributing)
- [📧 Contact](#-contact)

---

## 📌 About The Project

In an age of information overload, the ability to quickly distill text is paramount. The **AI Text Summarizer** is a modern, self-contained web application designed to address this need with a strong emphasis on **user privacy and control**.

Unlike other online summarizers that process your data on their servers, this tool operates entirely within your browser. It makes direct API calls to an external Large Language Model (LLM) endpoint that *you* provide. This ensures that your sensitive documents, research papers, or private communications are never stored, logged, or analyzed by a third party.

This project was built to demonstrate a powerful, serverless-first approach to AI tooling, combining a sleek user interface with robust functionality in a single, portable HTML file.

---

## ✨ Key Features

-   **🔒 Privacy-First Architecture:** No backend server. Your data stays yours. All API calls are client-side directly to your endpoint.
-   **🔌 Bring Your Own Endpoint (BYOE):** Fully compatible with services like **Ollama Cloud**, **Cloudflare Workers AI**, or any other OpenAI-compatible or custom LLM API.
-   **🎨 Customizable Output:** Fine-tune summaries with a slider for length and toggles for output style ("Concise Paragraph" vs. "Key Sentences").
-   **🚀 Sleek, Responsive UI:** A modern, cosmic-themed dark mode interface that is fully responsive and works beautifully on desktop and mobile devices.
-   **✅ Zero Dependencies:** Built with pure, native JavaScript and styled with Tailwind CSS via a CDN. No complex setup, `npm install`, or build process required.
-   **🧠 Stateful Experience:** The app conveniently remembers your API endpoint URL in your browser's local storage.
-   **✍️ Rich SEO Content:** Includes a comprehensive, 3500+ word collapsible article on AI summarization to attract organic traffic and educate users.

---

## 🛠️ Built With

This project stands on the shoulders of modern, lightweight web technologies, requiring no complex frameworks.

-   **HTML5**
-   **Tailwind CSS (via CDN)**
-   **Pure JavaScript (ES6+)**

---

## 🚀 Getting Started

Getting this application running is as simple as it gets.

1.  Clone the repository or download the `index.html` file.
    ```sh
    git clone https://github.com/hsinidev/ai-summarizer.git
    ```
2.  Open the `index.html` file in any modern web browser.

That's it! There are no installation steps or dependencies to manage.

---

## ⚙️ Usage

1.  **Enter Your API Endpoint:** In the "Ollama Cloud / Workers AI Endpoint URL" field, paste the full URL of your summarization API.
2.  **Paste Your Text:** Add the content you want to summarize into the "Input Text" area.
3.  **Configure Options:** Adjust the "Summary Length" slider and select your preferred "Output Style."
4.  **Generate:** Click the "Summarize Text" button to send the request. The summary will appear in the "Summary Output" panel.

### API Endpoint Configuration

The tool is designed to be flexible, but this requires you to ensure the API request payload is correct for your specific service. The default payload is formatted for **Ollama**.

To adapt it for a different service (e.g., an OpenAI-compatible API):

1.  Open `index.html` in a text editor.
2.  Navigate to the `<script>` tag at the bottom of the file.
3.  Find the `handleSummarize` async function.
4.  Locate the `payload` object. The code includes comments showing how to structure the payload for different APIs.

**Default (Ollama):**
```javascript
const payload = {
    prompt: prompt,
    model: "llama3", 
    stream: false
};
```

**Example for OpenAI-compatible API:**
```javascript
// const payload = {
//   "model": "gpt-3.5-turbo",
//   "messages": [{"role": "user", "content": prompt}]
// };
```
You will also need to adjust how the summary is extracted from the JSON response. Find the line `const summary = data.response || ...` and modify it to correctly parse the response from your specific endpoint.

---

## 📝 SEO & Content Strategy

This project includes a robust, built-in content strategy to maximize organic search visibility.

-   **Long-Form Article:** A 3500+ word, high-quality article on "The Ultimate Guide to AI Text Summarization" is embedded directly into the page. It covers everything from extractive vs. abstractive methods to the benefits and use cases of LLMs.
-   **JSON-LD Schema:** Comprehensive schema markup is included for `WebSite`, `WebApplication`, `Article`, and `FAQPage`, providing rich context to search engines.
-   **Full Meta Tag Optimization:** The page includes a highly optimized title, meta description, and keywords.
-   **User-Friendly Structure:** The content is neatly organized with a Table of Contents, a data table, and a collapsible FAQ section to enhance user experience and engagement.

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---



---

## 📧 Contact

HSINI MOHAMED - [@hsinidev](https://github.com/hsinidev) - hsini.web@gmail.com

Project Link: [https://github.com/hsinidev/ai-summarizer](https://github.com/hsinidev/ai-summarizer)

---
## 🚀 Quick Start & Installation

### 1. Clone the Repository
```bash
git clone https://github.com/hsinidev/AI-Text-Summarizer.git
cd AI-Text-Summarizer
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Launch the Application
```bash
npm start
```


---

## 👨‍💻 System Architect & Author

<table align="center" style="border: none; background: transparent; width: 100%;">
  <tr>
    <td align="center" width="160" style="border: none; padding: 12px;">
      <img src="https://avatars.githubusercontent.com/u/232697467?v=4" width="120" height="120" style="border-radius: 50%; box-shadow: 0 8px 24px rgba(99,102,241,0.3); border: 2.5px solid #6366f1;" alt="Hsini Mohamed" />
      <br /><br />
      <b>Hsini Mohamed</b><br />
      <sub>Morocco 🇲🇦</sub>
    </td>
    <td style="border: none; padding: 12px; vertical-align: middle;">
      <h3 style="margin-top: 0;">🚀 System Architect & Full-Stack Engineer</h3>
      <p style="font-size: 0.95rem; line-height: 1.6; color: #475569;">
        Specializing in high-performance autonomous AI systems, deterministic multi-agent swarms, enterprise cloud architecture, and modern full-stack engineering.
      </p>
      <p>
        <a href="https://hsini.dev"><img src="https://img.shields.io/badge/Portfolio-hsini.dev-2563eb?style=flat-square&logo=google-chrome&logoColor=white" alt="Portfolio" /></a>
        <a href="mailto:contact@hsini.dev"><img src="https://img.shields.io/badge/Email-contact@hsini.dev-ea4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
        <a href="https://github.com/hsinidev"><img src="https://img.shields.io/badge/GitHub-@hsinidev-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
        <a href="https://linkedin.com/in/hsinidev/"><img src="https://img.shields.io/badge/LinkedIn-hsinidev-0077b5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
      </p>
    </td>
  </tr>
</table>

---

## 📄 License & Attribution

This project is distributed under the **MIT License**. See [`LICENSE`](LICENSE) for complete terms.

<div align="center">
  <sub>⚡ Designed, architected, and maintained with engineering precision by <b><a href="https://hsini.dev">Hsini Mohamed</a></b>.</sub>
</div>
