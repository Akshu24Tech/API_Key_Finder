# 🔑 API Key Finder

An elegant and efficient web application designed to help developers quickly find the API key and documentation pages for hundreds of popular services. This tool solves the common problem of wasting time navigating complex websites just to get started with an API.

![API Key Finder Screenshot](https://postimg.cc/ykSp4DGV) 

---

## ✨ Features

* **Instant Search:** A powerful search bar that filters through a comprehensive, curated list of APIs in real-time.
* **Smart Search Fallback:** If an API isn't in our curated database, the app provides smart Google search links to help you find the API page and documentation instantly.
* **Categorized Filtering:** Filter the entire list by popular categories like `ai`, `payment`, `hosting`, `social`, and more with a single click.
* **Detailed Guides:** Each entry includes a quick, step-by-step guide on how to obtain the API key on the target website.
* **"Hello World" Snippets:** For many popular services, the app provides ready-to-use code snippets in both Python and JavaScript to get you started immediately.
* **One-Click Copy:** Easily copy guides and code snippets to your clipboard.
* **Community Submissions:** A user-friendly modal form allows the community to submit new API guides, helping the library grow.
* **Modern & Responsive Design:** A beautiful, animated interface built with Tailwind CSS that looks great on all devices.

---

## 🚀 Tech Stack

This project is built with modern, lightweight web technologies, making it fast, efficient, and easy to maintain.

* **HTML5:** For the core structure and content.
* **[Tailwind CSS](https://tailwindcss.com/):** For all styling, layout, and responsive design.
* **JavaScript (ES6+):** For all the client-side logic, including search, filtering, and interactivity.
* **[Prism.js](https://prismjs.com/):** For beautiful and readable syntax highlighting of the code snippets.

---

## 🛠️ How to Use

This is a pure front-end application. You can run it locally with any simple web server.

1.  **Clone the repository (or download the files):**
    ```bash
    git clone [https://github.com/your-username/api-key-finder.git](https://github.com/your-username/api-key-finder.git)
    ```

2.  **Navigate to the project directory:**
    ```bash
    cd api-key-finder
    ```

3.  **Open the `index.html` file:**
    You can open the `index.html` file directly in your web browser. For full functionality (especially if you add features that require it), it's best to use a local server.

    * **Using VS Code's Live Server:** If you use Visual Studio Code, you can install the [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) to launch a local development server with one click.
    * **Using Python's HTTP Server:** If you have Python installed, you can run a simple server from your terminal:
        ```bash
        # For Python 3
        python -m http.server
        ```
        Then, open your browser and go to `http://localhost:8000`.

---

## 🤝 How to Contribute

Contributions are welcome and encouraged! The easiest way to contribute is by adding new API guides to our database.

1.  **Open the `index.html` file.**
2.  **Locate the `apiDatabase` array** inside the `<script>` tag.
3.  **Add a new object** to the array for the API you want to add. Follow the existing structure:

    ```javascript
    { 
        name: 'Name of Service', 
        description: 'A brief description of what it does.', 
        authType: 'API Key / OAuth 2.0 / etc.', 
        link: 'Direct link to the API key page', 
        docs: 'Direct link to the main documentation page', 
        guide: [
            "First step of the guide.", 
            "Second step of the guide.", 
            "Third step."
        ], 
        tags: ['tag1', 'tag2', 'category'],
        codeSnippets: {
            python: `print("Hello, Python!")`,
            javascript: `console.log("Hello, JavaScript!");`
        }
    }
    ```
    *If there are no code snippets, you can set `codeSnippets: null`.*

4.  **Submit a Pull Request** with your changes!

Alternatively, you can use the **"+ Submit a Guide"** button on the website and open a GitHub Issue with the details from the form.
