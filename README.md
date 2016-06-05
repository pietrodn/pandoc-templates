# pandoc-templates

Did you know that you can create beautiful [LaTeX](https://www.latex-project.org) documents without writing in LaTeX?
Thanks to [Pandoc](http://pandoc.org), one can write in Markdown (the same simple markup language used to write this README) and then "compile" the file in LaTeX to produce a PDF.
In this way you write less code and the source is more readable.

You can still add LaTeX code directly in the Markdown files, or in a custom preamble.

I created two examples of the use of this tool:
* **article**: a simple LaTeX article demo
* **beamer**: a simple slideshow using the Beamer LaTeX package

## How to install (OS X)

1. Install LaTeX, simply downloading and installing the latest version of [MacTeX](https://tug.org/mactex/).
1. Install Xcode, or at least [Xcode Command Line Tools](http://osxdaily.com/2014/02/12/install-command-line-tools-mac-os-x/), if not already installed.
1. Install [Homebrew](http://brew.sh).
1. Install `pandoc` using Homebrew:
    `brew install pandoc`

## Usage

1. Clone a template.
1. Edit it with your favorite editor.
1. Run `make` to run pandoc.

## Files

* `header.tex`: your custom LaTeX header. Useful for including packages and make customizations. It will be included at the end of the preamble, before `\begin{document}`.
* `main.md`, `slide.md`: Markdown files with the content of the document.
* `main.pdf`, `slide.pdf`: the final output of Pandoc.
* `Makefile`: the [Makefile](https://www.gnu.org/software/make/) specifying Pandoc options and input files.
* `metadata.yaml`: a YAML file containing settings and metadata for Pandoc. here you can customize things like title, author, paper format, etc. For a full list of options, refer to the [Pandoc guide](http://pandoc.org/README.html#extension-yaml_metadata_block).

## License

All the material in this repository is in the **public domain** and freely reusable.
No rights reserved.

## References

* [Pandoc manual](http://pandoc.org/README.html)
* [Presentations with Beamer](http://rmarkdown.rstudio.com/beamer_presentation_format.html)
* [Talks with LaTeX Beamer, written in Markdown](http://nval.andreasherten.de/2016/01/26/latex-beamer-with-markdown.html)
