# Hồ Ngọc Phương - Personal Website

This is a personal website built with Docusaurus and deployed on GitHub Pages.

## 📋 System Requirements

To run this website on your local machine, you need one of the following:

- **Python 3** (available on most operating systems)
- **Node.js** and npm (recommended for web development)
- Or any other web server (Apache, Nginx, etc.)

## 🚀 How to Run the Website Locally

### Method 1: Using Python (Simplest)

Python is usually pre-installed on macOS and Linux. On Windows, you can download it from [python.org](https://www.python.org/downloads/).

#### Python 3:
```bash
# Navigate to the project directory
cd hongocphuong.github.io

# Run the web server
python3 -m http.server 8000

# Or on Windows:
python -m http.server 8000
```

Then open your browser and visit: **http://localhost:8000**

### Method 2: Using Node.js and npx

If you have Node.js installed, you can use these packages:

#### Using serve (Recommended):
```bash
# Navigate to the project directory
cd hongocphuong.github.io

# Run with npx (no installation needed)
npx serve

# Or install globally:
npm install -g serve
serve
```

#### Using http-server:
```bash
# Navigate to the project directory
cd hongocphuong.github.io

# Run with npx
npx http-server

# Or install globally:
npm install -g http-server
http-server
```

Then open your browser and visit the displayed address (usually http://localhost:3000 or http://localhost:8080)

### Method 3: Using PHP

If you have PHP installed:

```bash
# Navigate to the project directory
cd hongocphuong.github.io

# Run PHP development server
php -S localhost:8000
```

Then open your browser and visit: **http://localhost:8000**

### Method 4: Using Live Server (VS Code Extension)

If you use Visual Studio Code:

1. Install the "Live Server" extension by Ritwick Dey
2. Open the project folder in VS Code
3. Right-click on `index.html`
4. Select "Open with Live Server"

## 📁 Project Structure

```
hongocphuong.github.io/
├── index.html          # Homepage
├── blog.html           # Blog page
├── search.html         # Search page
├── 404.html            # 404 error page
├── assets/             # Directory for CSS, JS, and images
│   ├── css/            # Stylesheet files
│   ├── js/             # JavaScript files
│   └── images/         # Images
├── blog/               # Blog posts
├── docs/               # Documentation
├── img/                # General images
├── vi/                 # Vietnamese content
└── .nojekyll           # GitHub Pages configuration file
```

## 🛠️ About Docusaurus

This website is built with Docusaurus - a static documentation site generator by Facebook/Meta. This is the pre-built version (static HTML/CSS/JS), ready to deploy.

### If you want to edit and rebuild the website:

You need to find the original source code (usually in another branch or repository) that contains:
- `package.json`
- `docusaurus.config.js`
- `docs/`, `blog/`, `src/` directories

Then run these commands:
```bash
npm install           # Install dependencies
npm run start         # Run development server
npm run build         # Build static files
```

## 📝 Notes

- This is a static website, it doesn't require a database or backend server
- All content is pre-built and can be run directly
- This website is hosted on GitHub Pages at: https://hongocphuong.github.io

## 🔗 Useful Links

- [Docusaurus Documentation](https://docusaurus.io/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

## ❓ Frequently Asked Questions

**Q: Do I need to install Docusaurus?**
A: No, this website is already built. You only need a simple web server to run the HTML files.

**Q: Why do I see a 404 error when navigating pages?**
A: Make sure you're running the web server from the project root directory (where `index.html` is located).

**Q: How can I edit the website content?**
A: To edit content, you need the original Docusaurus source code. This repository only contains the built version.

**Q: Port 8000 is already in use, how do I change the port?**
A: Change the port number in the command, for example: `python3 -m http.server 3000`

## 📧 Contact

If you have any questions, please create an issue on this GitHub repository.
