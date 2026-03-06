# solidity-by-example-offline

> A print-ready, fully compiled reference of [solidity-by-example.org](https://solidity-by-example.org) — **129 lessons across 7 categories** — in a single Markdown file with real contract code and explanations.

Built for offline study. No browser needed.

---

## What's Inside

| File | Description |
|------|-------------|
| `solidity-by-example.md` | All 129 lessons compiled into one structured Markdown file |

### Coverage

| Chapter | Category | Lessons |
|---------|----------|---------|
| 1 | Solidity Basics | 52 |
| 2 | Applications | 24 |
| 3 | Hacks & Vulnerabilities | 18 |
| 4 | EVM Internals | 2 |
| 5 | Testing (Echidna) | 1 |
| 6 | Foundry | 10 |
| 7 | DeFi Protocols | 21 |

---

## Convert to PDF

You need [Pandoc](https://pandoc.org/installing.html) and a LaTeX engine (`pdflatex` or `xelatex`).

```bash
# Install Pandoc (Ubuntu/Debian)
sudo apt install pandoc texlive-latex-recommended texlive-fonts-recommended

# Convert
pandoc solidity-by-example.md -o solidity-by-example.pdf \
  --highlight-style=tango \
  --toc \
  --number-sections \
  -V geometry:margin=1in \
  -V fontsize=10pt \
  -V documentclass=article
```

For a cleaner result with a cover page:

```bash
pandoc solidity-by-example.md -o solidity-by-example.pdf \
  --highlight-style=tango \
  --toc \
  --toc-depth=2 \
  --number-sections \
  -V geometry:"top=1in, bottom=1in, left=1.2in, right=1in" \
  -V fontsize=10pt \
  -V linkcolor=blue \
  -V documentclass=article
```

---

## Source

All contract code is sourced from the official open-source repository:
[github.com/solidity-by-example/solidity-by-example.github.io](https://github.com/solidity-by-example/solidity-by-example.github.io)

This repo is an **unofficial compiled reference** — not affiliated with solidity-by-example.org.

---

## License

Contract source code: [MIT](https://opensource.org/licenses/MIT) — solidity-by-example.org  
This compilation: MIT
