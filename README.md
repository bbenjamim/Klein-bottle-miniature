# Klein-bottle-miniature
A Klein bottle miniature figure in a LaTeX package


# kleinbottle

A tiny LaTeX package for drawing customizable Klein bottle miniatures.

**Author:** Benjamim Lima Neto  
**Version:** 1.0  
**Release date:** 2026-11-26  
**License:** LPPL 1.3c or later

## Overview

The `kleinbottle` package provides a simple, customizable
vector illustration of the Klein bottle using TikZ.

It allows users to insert a miniature representation of
the Klein bottle into LaTeX documents through a single
command, with four independent customization options.

## Features

- Custom colors and color mixing.
- Percentage-based opacity.
- Proportional scaling.
- Counterclockwise rotation.
- Vector graphics without external image files.
- Independent customization of each miniature.
- Support for inline and displayed illustrations.

## Installation

Place `kleinbottle.sty` in the same directory as your
main LaTeX document.

Load the package in the preamble:

```latex
\usepackage{kleinbottle}
```

## Usage

The default miniature is produced by:

```latex
\klein
```

The complete syntax is:

```latex
\klein[color=blue, opacity=75, scale=2, rotate=45]
```

All options are optional and may be specified
in any order.

| Option  | Default | Accepted values |
|---------|---------|-----------------|
| color   | black   | Valid xcolor expressions |
| opacity | 100     | Numbers from 0 to 100 |
| scale   | 1       | Positive numbers |
| rotate  | 0       | Degrees from 0 to 360 |

Numerical values are subject to the precision
and dimensional limits of PGF and TeX.

## Minimal Working Example

```latex
\documentclass{article}
\usepackage{kleinbottle}

\begin{document}

The Klein bottle \klein\ is a non-orientable surface.

\begin{center}
    \klein[color=blue, scale=5]
    \qquad
    \klein[color=red, opacity=50, scale=3, rotate=45]
\end{center}

\end{document}
```

## Dependencies

The package automatically loads:

- TikZ/PGF
- xcolor
- graphicx

No external image files or special fonts are required
to use the package.

## Documentation

The complete user manual is available in
[kleinbottle.pdf](kleinbottle.pdf).

The LaTeX source of the documentation is provided
in `kleinbottle.tex`.

## Maintenance

The author and current maintainer of this package
is Benjamim Lima Neto.

Bug reports and suggestions are welcome through
the Issues section of this GitHub repository.

## License

Copyright (C) 2026 Benjamim Lima Neto.

This work may be distributed and/or modified under
the conditions of the LaTeX Project Public License,
either version 1.3c of this license or (at your option)
any later version.

The latest version of this license is available at:

https://www.latex-project.org/lppl.txt

This work has the LPPL maintenance status `maintained`.

The Current Maintainer of this work is Benjamim Lima Neto.

This work consists of the files:

- kleinbottle.sty
- kleinbottle.tex
- README.md

and the derived file:

- kleinbottle.pdf

The accompanying LICENSE file contains the official
LPPL license text.

## Version History

### Version 1.0 — November 26, 2026

Initial release.
