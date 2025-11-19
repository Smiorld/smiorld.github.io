# Qiye Zhou - Resume Website

This is a personal resume website built with [JSON Resume](https://jsonresume.org/) format and automatically deployed to GitHub Pages using GitHub Actions.

## 🌐 Live Site

Visit the live resume at: [https://smiorld.github.io](https://smiorld.github.io)

## 📋 Features

- **JSON Resume Format**: Uses the standard JSON Resume schema for portability
- **Automatic Deployment**: GitHub Actions automatically builds and deploys on push to main branch
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Print-Friendly**: Optimized for printing to PDF

## 🚀 Setup

### Prerequisites

- Node.js 20 or higher
- npm

### Local Development

1. Clone this repository:
   ```bash
   git clone https://github.com/smiorld/smiorld.github.io.git
   cd smiorld.github.io
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run serve
   ```

4. Open your browser to `http://localhost:4000` to view your resume

### Building

To build the resume to HTML:

```bash
npm run build
```

This will generate an `index.html` file from your `resume.json`.

## 📝 Updating Your Resume

1. Edit the `resume.json` file with your information
2. Commit and push to the main branch:
   ```bash
   git add resume.json
   git commit -m "Update resume"
   git push origin main
   ```
3. GitHub Actions will automatically rebuild and deploy your site

## 🎨 Changing the Theme

This project uses the `jsonresume-theme-even` theme. To change themes:

1. Find a theme from [JSON Resume Themes](https://jsonresume.org/themes/)
2. Install it: `npm install jsonresume-theme-[name]`
3. Update the build script in `package.json`:
   ```json
   "build": "resume export index.html --theme [theme-name]"
   ```

Popular themes:
- `jsonresume-theme-elegant`
- `jsonresume-theme-stackoverflow`
- `jsonresume-theme-kendall`
- `jsonresume-theme-flat`

## 🔧 GitHub Pages Setup

To enable GitHub Pages for this repository:

1. Go to your repository settings
2. Navigate to "Pages" in the left sidebar
3. Under "Build and deployment":
   - Source: Select "GitHub Actions"
4. The workflow will automatically deploy on the next push to main

## 📄 File Structure

```
.
├── .github/
│   └── workflows/
│       └── deploy.yml       # GitHub Actions workflow
├── resume.json              # Your resume data (JSON Resume format)
├── index.html              # Generated resume HTML
├── package.json            # Node.js dependencies and scripts
└── README.md               # This file
```

## 🛠️ Technologies Used

- [JSON Resume](https://jsonresume.org/) - Open source resume schema
- [resume-cli](https://github.com/jsonresume/resume-cli) - Command line tool for JSON Resume
- [GitHub Actions](https://github.com/features/actions) - CI/CD automation
- [GitHub Pages](https://pages.github.com/) - Static site hosting

## 📜 License

MIT License - feel free to use this template for your own resume!

## 👤 Contact

**Qiye Zhou**
- Email: JuliusQiyeZhou@gmail.com
- GitHub: [@smiorld](https://github.com/smiorld)
- LinkedIn: [qiyezhou](https://linkedin.com/in/qiyezhou)
