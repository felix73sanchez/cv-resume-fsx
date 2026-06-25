# Awesome CV — LaTeX Resume Template

A clean, professional LaTeX resume template based on [posquit0/Awesome-CV](https://github.com/posquit0/Awesome-CV), with bilingual support (English/Spanish) and modern tooling.

![Preview](https://img.shields.io/badge/LaTeX-XeLaTeX-blue?logo=latex)
![License](https://img.shields.io/badge/license-MIT-green)
![Build](https://img.shields.io/badge/build-passing-brightgreen)

## Features

- **Bilingual**: English (`resume_en.tex`) and Spanish (`resume_es.tex`) versions included
- **Modern design**: Clean, ATS-friendly layout with FontAwesome icons
- **XeLaTeX**: Full Unicode and font support
- **Customizable**: Easy color scheme, margins, and section configuration
- **FontAwesome 5**: Vector icons for contact info, skills, and social links
- **Self-contained**: All fonts bundled (Roboto, Source Sans Pro, FontAwesome)

## Quick Start

### Prerequisites

- **XeLaTeX** (part of TeX Live / MacTeX / MikTeX)
- **Git** (for cloning)

```bash
# Ubuntu/Debian
sudo apt install texlive-xetex texlive-fonts-recommended

# macOS (MacTeX)
brew install --cask mactex

# Windows
# Install MikTeX from https://miktex.org/download
```

### Build

```bash
# Clone the repo
git clone https://github.com/your-username/awesome-cv-resume.git
cd awesome-cv-resume

# Build English version
xelatex resume_en.tex

# Build Spanish version
xelatex resume_es.tex

# Build default (English)
xelatex resume.tex
```

Output: `resume_en.pdf`, `resume_es.pdf`, or `resume.pdf`

### Using latexmk (recommended)

```bash
# Install latexmk (usually included with TeX Live)
# Build with automatic dependency tracking
latexmk -xelatex resume_en.tex
latexmk -xelatex resume_es.tex

# Clean build artifacts
latexmk -c
```

## Project Structure

```
.
├── fonts/                    # Bundled fonts (Roboto, Source Sans Pro, FontAwesome)
│   ├── FontAwesome.otf
│   ├── Roboto-*.ttf
│   └── SourceSansPro-*.otf
├── awesome-cv.cls            # Document class (modified from Awesome-CV)
├── fontawesome.sty           # FontAwesome LaTeX package
├── resume.tex                # Default resume (English)
├── resume_en.tex             # English version
├── resume_es.tex             # Spanish version
├── .gitignore                # Git ignore rules
├── LICENSE                   # MIT License
└── CONTRIBUTING.md           # Contribution guidelines
```

## Customization

### Colors

Edit the color in your `.tex` file:

```latex
% Predefined: awesome-red, awesome-blue, awesome-green, awesome-orange, etc.
\colorlet{awesome}{awesome-blue}

% Or define custom:
\definecolor{awesome}{HTML}{2C3E50}
```

### Fonts

The template uses bundled fonts via `\fontdir[fonts/]`. To use system fonts instead, remove the `fonts/` directory and comment out `\fontdir[fonts/]`.

### Sections

Add/remove sections by editing the `\cvsection{}` blocks in `resume_en.tex` or `resume_es.tex`.

## Credits

- Original template: [posquit0/Awesome-CV](https://github.com/posquit0/Awesome-CV)
- FontAwesome: [Font Awesome](https://fontawesome.com/)
- Roboto: [Google Fonts](https://fonts.google.com/specimen/Roboto)
- Source Sans Pro: [Adobe Fonts](https://fonts.adobe.com/fonts/source-sans-pro)

## License

MIT License — see [LICENSE](LICENSE) for details.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.