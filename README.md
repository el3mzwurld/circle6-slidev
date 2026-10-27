# Circle6 Slidev Presentation

A developer-focused presentation built with [Slidev](https://sli.dev) for Circle6.

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

You can make contributions to the presentation! Please follow these guidelines to keep the workflow clean and consistent.

### 🌿 Branch Naming Conventions

When creating a new branch, adhere to the following prefix naming structure based on your task:

1. **`sld-<topicname>`**: Use for adding a slide or a combination of multiple slides representing a contribution toward a specific topic.
   * *Example:* `sld-intro-to-docker`
2. **`fix-<topicname>`**: Use for tweaks, removals, style corrections, or fixes made to already existing slides.
   * *Example:* `fix-typo-slide-3`

---

### 🔀 Pull Request (PR) Practices

* **Target Branch:** All PRs **MUST** be directed to the `work` branch. **Never submit a PR directly to `main`**.
* **Clear & Concise PR Naming:** Ensure your PR title clearly describes the change (e.g., `sld: add overview slides for state management` or `fix: resolve overflow issue on slide 5`).
* **PR Scope:** Keep PRs focused on a single logical change or topic to make reviews quick and straightforward.

---

### 🔄 Contribution Workflow

1. **Base your branch off `work`:**

   ```bash
   git checkout work
   git pull origin work
   ```

2. **Create your feature branch using the proper prefix:**

   ```bash
   # For new slide content
   git checkout -b sld-your-topic-name

   # For fixes or tweaks
   git checkout -b fix-your-topic-name
   ```

3. **Edit the slides:**
   * All presentation content updates must be made directly inside **`slides.md`**.
   * Use standard Markdown and Slidev syntax (use `---` to separate individual slides).
   * You can absolutely use traditional html within it, but ensure it falls between the proper slidev syntax and doesn't break your local deployment before opening a PR.

4. **Preview your changes:**
   Run the dev server to verify layout and formatting:

   ```bash
   npm run dev
   ```

5. **Commit and push your branch:**

   ```bash
   git add slides.md
   git commit -m "sld: add topic slides"
   git push origin sld-your-topic-name
   ```

6. **Open a Pull Request:**
   Submit a PR from your feature branch targeted into the **`work`** branch with a clear title and description.
