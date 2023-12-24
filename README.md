# nanotes

![GitHub Action Status](https://img.shields.io/github/actions/workflow/status/nareal/nanotes/publish.yml)

This is a [Quarto](https://quarto.org/) extension to provide a PDF template to create handout notes. It adds a header to the standard quarto template, so it supports all the features of this  [Tufte like handout](https://quarto-dev.github.io/quarto-gallery/page-layout/tufte.pdf) from the [quarto Gallery](https://quarto.org/docs/gallery/).

## Installation

If you want to start with a template do:
```bash
quarto use template nareal/nanotes
```

You just want to add the extension use:
```bash
quarto add  nareal/nanotes
```

This command installs the extensions under the `_extension` subdirectory.

If you want you can specify the version number:
```bash
quarto add nareal/nanotes@v1.0
```

To update the extension use:
```bash
quarto update extension nareal/nanotes
```

and to remove it:
```bash
quarto remove extension nareal/nanotes
```

## Usage

You can use the following metadata fields:

```yaml
title: "Notes title"
subtitle: "Notes subtitle"
author: "Author name"
date: "2022-10-06"
format:
  nanotes-pdf: 
    keep-tex: true
    coursename: "Course name"
    academicyear: 2022/2023
    degree: "Degree in XXX"
    university: "University Name"
    school: "School Name"
    logofilepath: file_path_to_logo.pdf
    #mainfont: SF Pro Text # Make sure you select a font installed in your system
    #sansfont: SF Pro Text #  Make sure you select a font installed in your system
    logofilepath: um-eeg.pdf
bibliography: bibliography.bib
```

## Example

Here is the source code of an example file: [template.qmd](template.qmd) and the [rendered PDF file](https://nareal.github.io/nanotes).
