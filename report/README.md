# Report Generation Instructions

This is a general overview of how I'm generating the PDF version of the project report.

## Dependencies

- Docker
- Pandoc/Extra Image
- Eisvogel Template

## Instructions

- Run the following command(s) from the root directory of this repository

    ```shell
    alias pandock='docker run --rm -v "$(pwd):/data" -u $(id -u):$(id -g) pandoc/extra'
    pandock --listings -o report/report.pdf --metadata-file=report/meta.yaml --citeproc "report/report.md" --template eisvogel
    ```

## Credits / Resources / Many Thanks To

* [Pandoc-Latex-Template](https://github.com/Wandmalfarbe/pandoc-latex-template)