## scripts

a place to store some small on/off scripts i use.

### `file-pdf`

this script needs [ocrmypdf](https://github.com/ocrmypdf/OCRmyPDF) and expects 2
parameters: a pdf file and a archive directory. once called it will:

- run `ocrmypdf` on the pdf to enrich the pdf with text
- the new file is named `YYYY-MM-DD_original.pdf`
- the new file is moved into a yearly folder in the archive
- original file is deleted

meant to be used with an
[automator action](https://support.apple.com/en-gb/guide/automator/welcome/mac),
listening on a folder.
