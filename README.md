# My Resume

[![CircleCI](https://circleci.com/gh/iqueiroz/resume.svg?style=shield)](https://circleci.com/gh/iqueiroz/resume)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue.svg)](https://www.linkedin.com/in/ivan-queiroz)
[![Resume](https://img.shields.io/badge/Resume-pdf-blue.svg)](https://github.com/iqueiroz/resume/releases/download/latest/resume.pdf)

Repository created to host my resume. It's written in LaTeX the template [YAAC: Another Awesome CV](https://github.com/darwiin/yaac-another-awesome-cv) with some customizations to fit my needs.

## Getting Started

These instructions will allow you to generate a PDF version of my resume on your local machine.

### Prerequisites

The easiest way to build this document locally is using Docker.  
To install Docker in your system follow these instructions:

* Official website: https://docs.docker.com/install/

## Building

Pull the [latexmk](https://hub.docker.com/r/iqueiroz/latexmk/) image, this image has everything needed:

```bash
docker pull iqueiroz/latexmk
```

Run the image to generate the PDF:

For linux:

```bash
docker run -v $(pwd):/work iqueiroz/latexmk resume.tex
```

For Windows, in command prompt:

```bash
docker run -v "%cd%":/work iqueiroz/latexmk resume.tex
```