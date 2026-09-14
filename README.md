# Auto Code Block Highlighter

A universal, lightweight, and copy-paste syntax highlighting engine powered by **Prism.js**. 

This tool is designed specifically for bloggers, content creators, and developers who want a zero-configuration way to add beautiful, desktop-grade code blocks to their websites without dealing with complex installation steps. It is highly lightweight, fast, and SEO-friendly.

---

## 📌 Table of Contents
* [✨ Features](#-features)
* [🎨 Modern Look & Feel (UI/UX)](#-modern-look--feel-uiux)
* [📋 Interactive Smart Copy Button](#-interactive-smart-copy-button)
* [💡 Language Class Conventions](#-language-class-conventions)
* [💻 How It Works & Usage](#-how-it-works--usage)
  * [🛠️ Step 1: Site-Wide Integration](#️-step-1-site-wide-integration)
  * [📝 Step 2: Use Pre Tags in Your Posts](#-step-2-use-pre-tags-in-your-posts)
* [📂 Project Structure](#-project-structure)
* [🛠️ Built With](#️-built-with)
* [👥 Author & Version Info](#-author--version-info)
* [📜 License & Acknowledgments](#-license--acknowledgments)

---

## ✨ Features
* **Plug-and-Play Setup:** Just copy the top engine code block, paste it into your website theme, and you're done.
* **Automatic Parsing:** Automatically targets and styles all standard HTML `<pre>` tags across any layout or post.
* **SEO-Friendly Architecture:** Uses clean, semantic HTML elements so search engine crawlers can perfectly read and index your code content.
* **Multi-Language Support:** Pre-configured to render syntax highlighting smoothly across Go, Python, C, C++, C#, Java, CSS, JavaScript, and SQL.

## 🎨 Modern Look & Feel (UI/UX)

The script transforms raw text into a sleek, premium developer experience styled after modern code editors:

![Auto Code Block Highlighter Preview](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgm1VDCFATdFHS4u3sIJpPuE78ATRZ5CMFYKu9g3DBSpO1nEDwyEq16juddQsZry5XIwLKeo0JHb9DcRHSDDiq-Px3OdV8rUxwJRB79671DVWRZa8CHek3TCZcfmpZFijzIyO2v0mkrg4q9hcNHkDsA8sVaacVnIeCgnxkkr2a1vg7cclZkccsVbgNuw-M/)


* **VS Code Dark Theme:** Code blocks utilize a deeply immersive, high-contrast dark theme optimized for readability and reducing eye strain.
* **Mac-Style Window Controls:** Each container renders desktop-grade details featuring classic top-left traffic-light window dots (Red, Yellow, Green).
* **Dynamic Header & Filenames:** If a `data-file` attribute is present, the header dynamically showcases the file name (e.g., `main.go`) to display your file structure cleanly.
* **Fully Responsive:** Micro-engineered layout engine that flexes fluidly down to mobile sizes without breaking text blocks or introducing layout shifting.

## 📋 Interactive Smart Copy Button
Every generated code card automatically embeds an interactive **Copy Button** in the upper-right corner:
* **One-Click Functionality:** Users can copy the clean, unformatted raw code snippet straight to their clipboard instantly without manually selecting text.
* **Visual States:** Supports active hover feedback states and responsive button labels that work perfectly out of the box.

## 💡 Language Class Conventions
To activate precise language tokenization via Prism.js, you **must include the standard Prism CSS class modifier** directly on your target block. Match your code's language by changing the suffix of the class identifier:
* **Go:** `class="language-go"`
* **Python:** `class="language-python"`
* **JavaScript:** `class="language-javascript"`
* **HTML/CSS:** `class="language-css"` or `class="language-html"`

## 💻 How It Works & Usage

Your project file (`auto-code-block-highlighter.html`) is structured as a complete, standalone utility split into two parts: the **Highlighter Engine** and the **Demo Snippets**.

### 🛠️ Step 1: Site-Wide Integration
Open your project's `auto-code-block-highlighter.html` file. Copy all the styles, scripts, and configurations located **above** this boundary marker:

```html
<!-- =================== END AUTO CODE BLOCK =================== -->
```

Paste that exact code block into your website or platform template:
* **Blogger / Blogspot:** Go to **Theme** -> **Edit HTML**, and paste it right before the closing `</head>` tag or inside your master layout file.
* **WordPress:** Paste it into a theme header/footer file, or drop it into a site-wide Custom HTML insertion panel.
* **Wix / Squarespace:** Use the **Embed HTML** or **Custom Code** dash tools to inject the code globally into your header.

### 📝 Step 2: Use Pre Tags in Your Posts
Once the engine is pasted into your website layout, you don't need to write any more scripts. When drafting your blog posts or pages, simply wrap your source code inside regular HTML `<pre>` tags, adding the appropriate language class alongside your `data-file` target name attribute:

```html
<pre class="language-go" data-file="main.go">
package main
import "fmt"
func main() { fmt.Println("Hello") }
</pre>
```

The background parser engine will seamlessly detect the tag at runtime, map the correct programming language tokens, attach window UI accents, and render a beautifully formatted developer code block automatically.

## 📂 Project Structure
```text
├── auto-code-block-highlighter.html   # Main template containing the core copy-paste engine and testing suite
└── README.md                          # Project documentation and integration manual
```

## 🛠️ Built With
* **HTML5 & CSS3 Variables:** Driven by clean custom properties for instant styling adjustments.
* **Vanilla JavaScript:** Event-driven engine running on standard DOM workflows to process rendering routines lightning-fast after page load.
* **Prism.js Core (v1.29.0):** Leverages a lightweight syntax tokenizer delivered safely via cdnjs.
* **Prism Autoloader Plugin:** Dynamically detects and injects grammar rules for specialized languages seamlessly at runtime, removing the need for manual script configuration.
* **Prism Tomorrow Night Theme:** Modern, eye-friendly production stylesheet theme mapping premium developer aesthetics.

## 👥 Author & Version Info
* **Author:** Ketan Kale (kketan77)
* **Current Version:** `v1.0.0`
* **Status:** Fully functional, stable, and production-ready.

## 📜 License & Acknowledgments
This project is open-source software distributed freely under the standard permissive terms of the **MIT License**. Core syntax styling algorithms and plugins are driven natively via **Prism.js v1.29.0** under identical open permission terms.
