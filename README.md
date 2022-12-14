# AGU Quarto Template

This is a Quarto template that assists you in creating a manuscript for AGU journals. Please note that neither I nor this Quarto template are associated with AGU; this is simply a Quarto port of their [provided LaTeX template](https://www.agu.org/Publish-with-AGU/Publish).

On Linux, use of this package may require the `texlive-bibtex-extra` package. On Ubuntu, install via:

```bash
sudo apt install texlive-bibtex-extra
```

## Creating a New Article

You can use this as a template to create an article for an AGU journal. To do this, use the following command:

```bash
quarto use template mikemahoney218/quarto-agu
```

This will install the extension and create an example qmd file and bibiography that you can use as a starting place for your article.

## Installation For Existing Document

You may also use this format with an existing Quarto project or document. From the quarto project or document directory, run the following command to install this format:

```bash
quarto install extension mikemahoney218/quarto-agu
```

## Usage

To use the format, you can use the format names `agu-pdf` and `agu-html`, for manuscripts, and `agu-supps-pdf` and `agu-supps-html` for supplementary materials. For example:

```bash
quarto render article.qmd --to agu-pdf
```

or in your document yaml

```yaml
format:
  pdf: default
  agu-pdf:
    keep-tex: true    
```

You can view a preview of the rendered template at <https://mike.quarto.pub/demo-agu-template/>.


## In The Wild

Use this template for a paper or a preprint? [Let me know,](https://github.com/mikemahoney218/quarto-tandf/issues/new) and I'll add it to this section!
