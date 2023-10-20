# Markdown to PDF Converter Script

## Description

An enhanced shell script that leverages Pandoc and XeLaTeX to convert Markdown files into PDFs. The script comes with a variety of customizable options such as font size, font family, output file name, and paper size. It even supports batch conversion within a directory.

## Prerequisites

- Pandoc
- XeLaTeX

## Table of Contents

1. [Usage](#usage)
    - [Basic Usage](#basic-usage)
    - [Options](#options)
    - [Examples](#examples)
2. [Functions Explained](#functions-explained)
3. [Limitations](#limitations)
4. [Contributing](#contributing)
5. [License](#license)

## Usage

### Basic Usage

```bash
./mdtopdf.sh <input_file.md>
```

### Options

- `-h`: Display help information.
- `-o`: Specify the output file name.
- `-f`: Specify the font family.
- `-s`: Specify the font size.
- `-m`: Specify the monospaced font family.
- `-p`: Specify the paper size (default: a4).
- `-r`: Execute recursively in a directory.

### Examples

Convert a single file with default settings:

```bash
./mdtopdf.sh example.md
```

Convert a single file with a custom font and paper size:

```bash
./mdtopdf.sh -f 'Times New Roman' -p 'letter' example.md
```

Convert all `.md` files in a directory:

```bash
./mdtopdf.sh -r ./markdown_files/
```

## Functions Explained

1. `Convert()`: Handles the main conversion via Pandoc, and accepts various customization options.
2. `Help()`: Displays the help menu.
3. `ValidateInput()`: Validates that the input file exists and has the correct extension.

## Limitations

- Make sure the file extension is `.md`.
- Ensure Pandoc and XeLaTeX are installed on your system.

## Contributing

Feel free to fork the project and submit a pull request with your changes!

## License
MIT License
