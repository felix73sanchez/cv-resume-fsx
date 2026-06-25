# Contributing

Thank you for considering a contribution! This project is a LaTeX resume template. Here's how you can help.

## Ways to Contribute

- **Bug reports**: Found a compilation issue or layout bug? Open an issue.
- **Feature requests**: New sections, color schemes, or font options.
- **Documentation**: Improve README, add examples, or translate docs.
- **Code**: PRs for the `.cls` file, font handling, or build scripts.

## Development Setup

```bash
# Clone your fork
git clone https://github.com/your-username/awesome-cv-resume.git
cd awesome-cv-resume

# Install XeLaTeX (see README.md)
# Make your changes
# Test compilation
xelatex resume_en.tex
xelatex resume_es.tex
```

## Pull Request Guidelines

1. **One change per PR** — keep it focused
2. **Test both languages** — compile `resume_en.tex` and `resume_es.tex`
3. **No build artifacts** — don't commit `.pdf`, `.aux`, `.log`, etc.
4. **Update documentation** — if you add features, update README.md
5. **Conventional commits** — use `feat:`, `fix:`, `docs:`, `style:`, `refactor:`

## Code Style

- LaTeX: Follow existing patterns in `awesome-cv.cls`
- Indentation: 2 spaces (matches existing files)
- Comments: Use `%` for comments, `%%` for section headers
- Line length: Keep under 100 chars where practical

## Reporting Issues

When filing a bug, include:

- OS and TeX distribution (TeX Live, MacTeX, MikTeX)
- XeLaTeX version (`xelatex --version`)
- Minimal example that reproduces the issue
- Expected vs actual behavior

## License

By contributing, you agree that your contributions will be licensed under the MIT License.