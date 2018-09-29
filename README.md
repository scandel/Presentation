# Presentation

This repository is a template for scientific presentations based on [Reveal.js](https://revealjs.com/#/).

See the [demo here](https://labojeanperrin.github.io/Presentation/).

## General Usage

Clone or download the repository on your local machine and modify `index.html` according to your needs. Please read the [Reveal.js presentation page](https://github.com/hakimel/reveal.js/) for information on basic editing.

Any text editor should work for this, but [Brackets](http://brackets.io/) is a smart choice since it is designed for web applications and has convenient live preview capabilities.

## Content

This template has several plugins already activated:

- **Equations** with [Katex](https://github.com/Khan/KaTeX). Embed your LaTeX-syntaxed equations in `$...$` for inline equations and in `$$...$$` for page-wide equations.
- **Local camera stream** with [reveal-embed-video](https://github.com/ThomasWeinert/reveal-embed-video)
- **Animated svg** with [Snap.svg](http://snapsvg.io/).

Audio, video and iframes are natively supported by your browser (html5).

## Specific features

This template has several specific features, listed below.

### Manage logos 

The institutional and funding logos can be changed in a straightforward manner with the `<logo>` tags defined in the `index.html` file. These tags are then converted to proper html at runtime by the javascript in `LJP.js`.

### Code \<snippet\>

Code snippets can be easily inserted with the `<snippet>` tag. This tag is then converted to proper html at runtime by the javascript in `LJP.js`.

### Two columns slides

The `<left>` and `<right>` tags are also interpreted at runtime to create left and right columns.

### Citations and bibliography

The `<cite>` tag allows to insert a citation in a slide. The bibliographic reference appears at the bottom of the page, with a maximum of 4 citations per slide (other citations are not displayed).

Then, a bibliography can be automatically generated in a specific slide by creating an empty bibliography section:

```
<section data-state='bibliography'></section>
```

A series of slides containing packets of 10 bibliographic references are then created at runtime. All references appear in the same order as in the `index.html` file.

## Misc notes

- This template has been developped for the Laboratoire Jean Perrin but it can be easily adaptated to other laboratories or institutions. One just have to put its own logos in the `Media/Images/Logos` directory and change the logos tags in `index.html`:

```
<logo class='institution' src='Media/Images/Logos/SU_Sciences.png'></logo>
<logo class='institution' src='Media/Images/Logos/LJP.png'></logo>
<logo class='institution' src='Media/Images/Logos/CNRS.png'></logo>
```
