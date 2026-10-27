# Circle6 Slidev Presentation

A developer-focused presentation built with [Slidev](https://sli.dev) for Circle6.

---

## 🛠️ Installation Guide

Follow these steps to set up the project locally on your machine.

### Prerequisites
Make sure you have the following installed:
* **Node.js** (v18.0 or higher recommended)
* **npm**, **pnpm**, or **yarn**

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/el3mzwurld/circle6-slidev.git
   cd circle6-slidev
   ```

2. **Install dependencies:**
   Using `npm`:
   ```bash
   npm install
   ```
   Using `pnpm`:
   ```bash
   pnpm install
   ```

---

## 🚀 Usage Guide

### 1. Start the Development Server
To launch the presentation in development mode with live-reload enabled:
```bash
npm run dev
# or using pnpm
pnpm dev
```
Open your browser and navigate to `http://localhost:3030` to view the slides.

### 2. Presenter Mode
While the development server is running, press **`p`** in your browser to open Presenter Mode, where you can view speaker notes, timers, and slide previews.

### 3. Build & Export
* **Build static hosting version:**
  ```bash
  npm run build
  ```
* **Export slides to PDF:**
  ```bash
  npm run export
  ```

---

## 🤝 Contribution Guide

We welcome contributions to the presentation! Please follow these guidelines to ensure a smooth workflow.

### Contribution Workflow

1. **Switch to the work branch:**
   Ensure you are working on the designated `work` branch before making changes:
   ```bash
   git checkout work
   git pull origin work
   ```

2. **Edit the slides:**
   * All presentation content and updates must be made directly inside **`slides.md`**.
   * Use standard Markdown and Slidev syntax (use `---` to separate individual slides).

3. **Preview your changes:**
   Run the dev server to verify your layout and content:
   ```bash
   npm run dev
   ```

4. **Commit and push:**
   Commit your changes and push them directly to the `work` branch:
   ```bash
   git add slides.md
   git commit -m "docs: update slides content"
   git push origin work
   ```
