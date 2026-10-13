[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

# Electron + React + TS + Vite Boilerplate

A production-ready starter template designed to quickly launch the development of modern, cross-platform desktop applications.

## ✨ Key Features

- **⚡ Blazing-Fast Development**: **Vite** for near-instant startup and high-performance Hot Module Replacement (HMR).
- **🔒 Secure by Design**: Secure Inter-Process Communication (IPC) using `contextBridge`, with no Node.js APIs exposed to the frontend.
- **💪 End-to-End Type Safety**: **TypeScript** configured for both the Main (backend) and Renderer (frontend) processes, with working path aliases (`@/*`).
- **🎨 Modern UI Ready to Go**: **TailwindCSS** and **ShadCN/UI** are integrated to build beautiful interfaces effortlessly.
- **✅ Built-in Validation**: The "Zod as a source of truth" pattern is encouraged for robust data management.
- **📦 Comprehensive Build Scripts**: Generate installers for Windows, macOS, and Linux with a single command.

## 🛠️ Tech Stack

- **Application Framework**: Electron
- **User Interface**: React + TypeScript
- **Build Tooling**: Vite
- **Styling**: TailwindCSS + ShadCN/UI
- **Data Validation**: Zod (recommended)

## 🚀 Quick Start

### Prerequisites

- Node.js (version 20 or higher recommended)
- npm or yarn

### Installation

1.  Clone this repository (or use it as a template on GitHub).
2.  Install the dependencies:
    ```sh
    npm install
    ```

### Running in Development Mode

This command starts the Vite server and the Electron application simultaneously with hot-reloading enabled.

```sh
npm run dev
```

## 🧠 AI-Assisted Development

This project includes a utility script to streamline working with large-context AI assistants (like Gemini, Claude, etc.).

The `npm run concat` command reads all important project files (source code, configs, documentation) and merges them into a single text file: `PROJECT_CONTEXT.md`.

Providing this comprehensive file to an AI gives it a complete overview of the architecture, code, and dependencies, enabling it to provide more relevant and accurate responses.

### Usage

1.  **Generate the context file:**

    ```sh
    npm run concat
    ```

2.  **Use the output:**
    Open the generated `PROJECT_CONTEXT.md` file located in the project's `/build` directory, copy its entire content, and paste it at the beginning of your conversation with the AI.

## 📦 Build Scripts

To package your application for distribution:

- **For Windows:**
  ```sh
  npm run dist:win
  ```
- **For macOS:**
  ```sh
  npm run dist:mac
  ```
- **For Linux:**

  ```sh
  npm run dist:linux
  ```

  The packaged files will be located in the `dist-electron` directory.

## 📂 Project Structure

```
src/
├── backend/      # Electron's Main process code ('system' logic)
├── ui/           # React application code (user interface)
├── components/   # Shared UI components (ShadCN)
└── types.ts      # Central file for types and schemas
```

## 📄 License

This project is licensed under the [MIT License](LICENSE).
