# inkscape_ext

Wrappers around the Inkscape command-line interaction

## Contents

<!-- MarkdownTOC -->

- [`svg2pdf`](#svg2pdf)
- [`svg2png`](#svg2png)
- [`svgfit`](#svgfit)
- [`svglayerswitch`](#svglayerswitch)

<!-- /MarkdownTOC -->

## `svg2pdf`

Convert a(n) (batch of) SVG image(s) to (a) PDF(s).

## `svg2png`

Convert a(n) (batch of) SVG image(s) to (a) PNG(s). Note that this script can use Inkscape, but it tries to use `rsvg` as the latter is usually faster.

## `svgfit`

Modify the canvas such that is exactly matches the size of the drawing.

## `svglayerswitch`

Use a single SVG-file to create 'frames' by selectively hiding/showing layers in the SVG-file. This can for example be used to 'build' a figure in several step for a presentation.


