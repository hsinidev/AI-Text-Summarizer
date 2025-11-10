
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

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-maintained-green.svg)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-yellow)
![CSS](https://img.shields.io/badge/CSS-Tailwind_CDN-38B2AC)
![HTML5](https://img.shields.io/badge/HTML-5-orange)

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
- [📄 License](#-license)
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

## 📄 License

Distributed under the MIT License. See the `LICENSE` file for more information (if available), or refer to the standard MIT License terms.

---

## 📧 Contact

HSINI MOHAMED - [@hsinidev](https://github.com/hsinidev) - hsini.web@gmail.com

Project Link: [https://github.com/hsinidev/ai-summarizer](https://github.com/hsinidev/ai-summarizer)
