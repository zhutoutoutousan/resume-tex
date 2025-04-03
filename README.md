# 🚀 Modern One-Page Resume Template

A minimalist, developer-friendly LaTeX resume template optimized for readability and efficient space usage. Perfect for tech professionals who appreciate clean typography and proper visual hierarchy.

## ✨ Features

- **Clean Typography**: Carefully chosen font sizes and spacing for optimal readability
- **Smart Layout**: Efficient use of space without compromising aesthetics
- **Developer-Friendly**: Modular structure with separate files for different sections
- **Responsive Design**: Automatically adjusts spacing to keep content on one page
- **Modern Elements**: Support for hyperlinks, custom styling, and Unicode characters

## 🎯 Perfect For

- Software Engineers
- Full Stack Developers
- Technical Program Managers
- UX/UI Designers
- Tech Leads

## 📁 Project Structure

```
resume-tex/
├── resume.tex              # Main LaTeX file
├── subsections/
│   ├── work_ex.tex        # Work experience section
│   ├── education.tex      # Education section
│   └── others.tex         # Skills and additional info
└── README.md
```

## 🛠️ Usage

### On Overleaf

1. Create a new project
2. Upload these files maintaining the directory structure
3. Set compiler to pdfLaTeX
4. Click 'Recompile' to generate your resume

### Local Development

Requirements:
- TeX Live or MiKTeX
- Any LaTeX editor (VS Code + LaTeX Workshop recommended)

```bash
# Clone the repository
git clone https://github.com/yourusername/resume-tex.git

# Compile the document
pdflatex resume.tex
```

## 📝 Customization

### Margins and Spacing
```latex
\usepackage[top=0.4in,bottom=0.4in,right=0.6in,left=0.6in]{geometry}
```

### Section Headers
```latex
\renewcommand{\section}[1]{%
    \vspace{0.8em}%
    \noindent{\Large\textbf{\uppercase{#1}}}\hrulefill\par
    \vspace{0.2em}%
}
```

### Job Entries
```latex
\subsection{COMPANY}{LOCATION}{JOB TITLE}{DATE}
```

## 🎨 Typography

- Main Font: Helvetica (via tgbonum package)
- Section Headers: Large, bold, uppercase
- Company Headers: Normal size, bold
- Body Text: 10pt with 13pt leading
- Links: Black, no underlining

## 💡 Pro Tips

1. Keep entries concise and impactful
2. Use action verbs to start bullet points
3. Quantify achievements where possible
4. Maintain consistent formatting
5. Use `\vspace` for fine-tuned spacing adjustments

## 🔧 Troubleshooting

### Common Issues

1. **Overfull hbox warnings**
   - Use `\small` for long lines
   - Break URLs across lines
   - Adjust margins slightly

2. **Content overflow**
   - Reduce `\vspace` values
   - Shorten bullet points
   - Use abbreviations in skills section

## 📄 License

MIT License - Feel free to modify and use for your own resume!

## 🤝 Contributing

Contributions welcome! Feel free to:
- Report bugs
- Suggest improvements
- Add features
- Fix typos

## 🌟 Star History

If you find this template useful, please consider giving it a star! It helps others discover this resource.

---
Made with ❤️ by developers, for developers 