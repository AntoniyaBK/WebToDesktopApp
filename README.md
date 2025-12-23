# Web To Desktop


This is a **desktop application** built with [Electron](https://www.electronjs.org/) that wraps your Web Instance site and makes it available as a standalone desktop app for Windows, Mac and Linux.

---

## 📌 Description

- Opens your Web in a standalone window.  
- Can be run locally without a browser.  
- URL can be easily changed in `main.js` or `config.json`.

---

## 🛠️ Installation

1. Clone the repository:

> git clone https://github.com/AntoniyaBK/Web-To-Desktop.git

2. Install dependencies:

> npm install

## ▶️ Running the App

To start the desktop app:

> npm start

This will open a window with your Web Instance URL.
You can change the URL directly in main.js.

## ⚙️ Deployment / Packaging
To create an executable for Windows, Mac or Linux, use electron-packager or electron-builder

Example with electron-packager:

1. Install:

> npm install electron-packager --save-dev

2. Package the app:

> npx electron-packager . WebApp --platform=win32 --arch=x64 --overwrite

This will create a folder WebApp-win32-x64 with a ready .exe for Windows.
Change --platform to darwin (Mac) or linux for other platforms.

## 📁 Project Structure

WebApp-Desktop/
<br> │ </br>
<br> ├─ main.js           # Main Electron script </br>
<br> ├─ package.json      # Node.js dependencies and scripts </br>
<br> ├─ node_modules/     # Installed libraries </br>
<br> ├─ .gitignore        # Ignore node_modules and other files </br>

## 🔧 Changing the URL

In main.js add URL for Web Instance
>  win.loadURL('https://your-web-instance.com'); 


## 📄 License

MIT License
