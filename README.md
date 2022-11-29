# AGU Quarto Template

This is a Quarto template that assists you in creating a manuscript for AGU journals. Please note that neither I nor this Quarto template are associated with AGU; this is simply a Quarto port of their [provided LaTeX template](https://www.agu.org/Publish-with-AGU/Publish).

## Creating a New Article

You can use this as a template to create an article for an AFT journal. To do this, use the following command:

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

## Format Options

This format does not have specific format option. Include documentation of such option otherwise. See <https://github.com/quarto-journals/elsevier#format-options> for an example.
