# Web To Desktop


This is a **desktop application** built with [Electron](https://www.electronjs.org/) that wraps your Web Instance site and makes it available as a standalone desktop app for Windows, Mac and Linux.

---

## 📌 Description

- Opens your Web in a standalone window.  
- Can be run locally without a browser.  
- URL can be easily changed in `index.js` or `config.json`.

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

## 📁 Project Structure

```
WebApp-Desktop/
│
├── index.js          # Main Electron script
├── package.json      # Node.js dependencies and scripts
├── config.json       # App configuration (URL, settings)
├── .gitignore        # Ignore node_modules and other files
└── node_modules/     # Generated after npm install
```

## 🔧 Changing the URL

In index.js add URL for Web Instance
>  win.loadURL('https://your-web-instance.com');

<br> OR In config.json add your web instance </br>

> "appUrl": "https://your-web-instance.com"

## 🤝 Contributing

Contributions are welcome!

If you want to improve this project:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m "Add new feature"`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a Pull Request

Feel free to open issues for suggestions, bugs or improvements.

## 📄 License

MIT License
