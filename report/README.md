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
    ```

    ```shell
    pandock --listings \
    --template https://raw.githubusercontent.com/Wandmalfarbe/pandoc-latex-template/master/eisvogel.tex \
    --output=report/report.pdf "report/report.md"
    ```

## Credits / Resources / Many Thanks To

* [Pandoc-Latex-Template](https://github.com/Wandmalfarbe/pandoc-latex-template)