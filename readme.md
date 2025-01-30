# Open Captable Protocol (OCP) Whitepaper

### VS Code Setup

1. Install the "LaTeX Workshop" extension by James Yu

   - Open VS Code
   - Go to Extensions (or press `Cmd+Shift+X`)
   - Search for "LaTeX Workshop"
   - Click Install

2. Restart VS Code after installation

## Building the Document

Once everything is set up:

1. Open `draft_1.tex` in VS Code
2. Click the "Build LaTeX Project" button (or use the keyboard shortcut)
3. A PDF preview should appear automatically

If you don't see the preview:

- Look for "View LaTeX PDF" button in the LaTeX Workshop sidebar
- Or find `draft_1.pdf` in your file explorer

## Prerequisites

To build this document locally, you'll need:

- A LaTeX distribution
- A text editor with LaTeX support (VS Code recommended)

### Installing LaTeX (MacOS)

1. Install BasicTeX using Homebrew:

```bash
brew install --cask basictex
```

2. Install required LaTeX packages:

```bash
sudo tlmgr update --self
sudo tlmgr --verify-repo=none install latexmk
sudo tlmgr install geometry
sudo tlmgr install hyperref
sudo tlmgr install listings
sudo tlmgr install amsmath
sudo tlmgr install xcolor
sudo tlmgr install graphics
sudo tlmgr install tools
```

3. Create build directory:

```bash
mkdir build
```

## Repository Structure

- `draft_1.tex` - Main LaTeX source file
- `build/` - Directory containing compiled PDF and auxiliary files
- `.gitignore` - Configured to exclude LaTeX auxiliary files

## Contributing

1. Make changes to `draft_1.tex`
2. Build to verify changes (press the Play button top right)
3. Commit only the source files (auxiliary files are ignored)
