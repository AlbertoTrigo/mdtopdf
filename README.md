
# Markdown to PDF Converter Script

## Introduction
This script is designed to convert Markdown files to PDFs using Pandoc. It's suitable for users who need to quickly transform their Markdown documents into a professionally formatted PDF file.

## Installation
Ensure that Pandoc and LaTeX are installed on your system. If not, you can install them using your package manager. For example, on Ubuntu:

```bash
sudo apt-get install pandoc texlive
```

Clone the script from the GitHub repository:

```bash
git clone [URL to GitHub repository]
```

Make the script executable:

```bash
chmod +x mdtopdf.sh
```

## Usage
To use the script, navigate to the directory containing the script and run it with the following syntax:

```bash
./mdtopdf.sh [OPTIONS]... FILE
```

Where `FILE` is the path to the Markdown file you want to convert.

### Options
- `-h`: Display the help menu.
- `-o`: Specify the output file name for the PDF.
- `-f`: Set the font family for the PDF.
- `-s`: Set the font size for the PDF.
- `-m`: Set the monospaced font family for the PDF.
- `-p`: Set the paper size for the PDF (default is A4).
- `-r`: Execute the script recursively in a directory.

### Examples
Convert a single file:

```bash
./mdtopdf.sh -o output.pdf -f "Arial" -s 12pt -m "Courier New" -p a4paper input.md
```

Convert all Markdown files in a directory:

```bash
./mdtopdf.sh -r /path/to/directory
```

## Contributions
Contributions are welcome. Please fork the repository and submit a pull request with your improvements.

## License
This script is distributed under the [MIT License](LICENSE). See the `LICENSE` file in the repository for more details.
