# Manual PCB Manufacturing Guide

[![Build PDF](https://github.com/USERNAME/manual_pcb_manufacturing_guide/actions/workflows/build-latex.yml/badge.svg)](https://github.com/USERNAME/manual_pcb_manufacturing_guide/actions/workflows/build-latex.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

A comprehensive, step-by-step practical guide on fabricating double-sided Printed Circuit Boards (PCBs) manually using photolithography, UV exposure, and chemical etching (without CNC milling).

Developed at the **Departamento de Tecnoloxía Electrónica (DTE)**, **Universidade de Vigo**.

---

## Authors

- **Fernando Flores** – `fernandoflores@ieee.org`
- **Miguel Salvatierra** – `miguelsalvatierra@ieee.org`
- **Elena Rodríguez** – `elenarlois@ieee.org`
- **Mateo González** – `mateo@ieee.org`
- **Óscar López** – `olopez@uvigo.es`

---

## Overview

This guide provides practical instructions starting from completed PCB layout artwork up to component assembly:

1. **Photolith Printing**: Laser transparency preparation, dual-sheet layering, and alignment.
2. **UV Exposure (Insolation)**: Copper-clad board preparation, vacuum sealing, and UV curing.
3. **Chemical Preparation**: Formulating caustic soda developer and acid etching mixtures.
4. **Photoresist Developing**: Caustic soda immersion, washing, and inspection.
5. **Acid Etching**: Accelerated chemical etching process, agitation, and hazardous waste disposal.
6. **Post-Processing & Drilling**: Edge trimming with guillotine shear, resist stripping, and vertical drill stand setup.
7. **Soldering & Component Assembly**: SMT & THT mounting, flux usage, and anti-oxidation coating.

---

## Building the Guide

### Prerequisites

Ensure you have a complete LaTeX distribution installed:
- **Windows**: [MiKTeX](https://miktex.org/) or [TeX Live](https://www.tug.org/texlive/)
- **Linux (Debian/Ubuntu)**: `sudo apt-get install texlive-latex-extra texlive-fonts-recommended latexmk`
- **macOS**: [MacTeX](https://www.tug.org/mactex/)

### Compilation

Compile the guide from the root directory:

```bash
pdflatex main.tex
pdflatex main.tex  # Second pass for cross-references and table of contents
```

Or using `latexmk`:

```bash
latexmk -pdf main.tex
```

The resulting document will be generated as `main.pdf`.

---

## Repository Structure

```text
.
├── .github/
│   └── workflows/
│       └── build-latex.yml     # Automated PDF compilation CI workflow
├── figures/
│   ├── generic/                # Logos (UVigo, GCode)
│   └── process_*.jpg           # High-resolution process photographs
├── .gitignore                  # LaTeX auxiliary and generated artifact filters
├── LICENSE                     # MIT License
├── main.tex                    # Document root, preamble, and styling
├── manual_pcb_manufacturing_guide.tex # Main instructional report content
└── README.md                   # Repository overview and instructions
```

---

## Safety Disclaimer

> [!CAUTION]
> This guide involves hazardous chemical processes using concentrated acids (hydrochloric acid), oxidisers (hydrogen peroxide), and corrosive bases (sodium hydroxide), as well as mechanical cutting and drilling tools. Always wear appropriate personal protective equipment (PPE)—nitrile gloves, chemical splash goggles, and a lab coat—and work inside a certified fume cupboard or well-ventilated extraction area. Follow all local safety and chemical waste disposal regulations. Proceed at your own risk.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
