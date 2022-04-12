# Tikz-Feynman Examples

Some examples for creating Feynman diagrams with the LaTeX package tikz-feynman. Using externalisation, changing the style of multiple images at once is made convenient.

A basic description is included below, for further instructions, see the document `Examples-tikz-feynman.pdf`, which also includes example images.

## main-general.tex

This document should be used to generate multiple figures at once, whose styles can be changed through the `config` files. By using the tikz library `external`, the individual `pdf` files are stored in the `/outputs` directory, and only recompiled when the corresponding input is changed.

When the global configurations are changed, this must be overriden by uncommenting the line `\tikzset{external/force remake}`.

To clean up the `/outputs` directory, a `.sh` script is included.

## main-standalone.tex

This document can be used to compile a single input, like `partonshowermedium.tex`. The pdf border can be adjusted in a case-by-case basis.
