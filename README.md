# XMAIL - AI Email Threat & Forensic Intelligence

A modern web application for email security analysis, forensic header inspection, URL safety scanning, and full mailbox synchronization with Google Mail styling.

## Prerequisites

Before running the project locally, make sure you have:
- **Node.js**: v18 or higher (v20+ recommended)
- **npm** (comes with Node.js)

---

## Getting Started Locally (VS Code / Terminal)

If you downloaded or extracted this project into a folder on your computer:

### 1. Open the project folder in VS Code
Open VS Code, then go to **File > Open Folder...** and select the project directory:
`xmail---ai-email-threat-&-forensic-intelligence`

### 2. Open the Terminal
In VS Code, press `` Ctrl + ` `` (or go to **Terminal > New Terminal**).

### 3. Install Dependencies
Run the following command to download and install all required packages into `node_modules`:

```bash
npm install
```

> **Note:** If you see an error like `Cannot find module ... vite.js` or `command not found: vite`, running `npm install` installs Vite and all dependencies locally into `node_modules`.

### 4. Start the Development Server
Once installation completes, run:

```bash
npm run dev
```

### 5. Open in Your Browser
Open your browser and visit:
```
http://localhost:3000
```

---

## Available Scripts

- `npm run dev`: Starts the local Vite development server on port 3000.
- `npm run build`: Compiles and bundles the application for production into `dist/`.
- `npm run preview`: Locally previews the production build.
- `npm run lint`: Runs TypeScript type checks (`tsc --noEmit`).

---

## Troubleshooting Common Issues

### 1. "Cannot find module ... vite.js" or "vite is not recognized"
This happens when `node_modules` is missing or was excluded from the ZIP download.
Run:
```bash
npm install
```
If the error persists on Windows PowerShell, run:
```bash
npm install vite --save-dev
npm run dev
```

### 2. PowerShell Script Execution Policy Error
If PowerShell gives an error about `running scripts is disabled on this system`:
Run this in PowerShell as Administrator:
```powershell
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```
Or run using `npx`:
```bash
npx vite
```
