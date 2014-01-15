---
project:  svg_parser
tagline:  svg parser to a cairo scene graph object
---

## `local svg_parser = require'svg_parser'`

A SVG 1.1 parser implemented in Lua. There's a handy collection of svg files to test the parser with.

Some notable features are not yet implemented:

  * patterns
  * radial gradient has issues
  * text
  * markers
  * constrained transforms: ref(svg,[x,y])
  * external references
  * use tag

Low-priority missing features:

  * icc colors
  * css language

## `svg_parser.parse(source) -> object`

Parses a SVG into a cairo scene graph object that can be rendered with [sg_cairo sg_cairo]. <br>

  * `source` is an [expat] source.

