# Markdown to PDF Converter Script

## Description

This shell script uses Pandoc to convert Markdown files to PDF. You can specify options such as output file name, font family, font size, and even execute the conversion recursively in a directory.

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

- `-h`: Display help information
- `-o`: Specify the output file name
- `-f`: Specify the font family
- `-s`: Specify the font size
- `-m`: Specify the monospaced font family
- `-r`: Execute recursively in a directory

### Examples

Convert single file with default settings:

```bash
./mdtopdf.sh example.md
```

Convert single file with custom font:

```bash
./mdtopdf.sh -f 'Times New Roman' example.md
```

Convert all `.md` files in a directory:

```bash
./mdtopdf.sh -r ./markdown_files/
```

## Functions Explained

1. `Convert()`: This function performs the main conversion using Pandoc and takes in various variables for customization like fonts, paper size, etc.

2. `Help()`: Displays the help menu.

3. `ntharg()`: Gets the nth argument from the shell input.

## Limitations

- Ensure the file extension is `.md`
- The script assumes Pandoc and XeLaTeX are installed.

## Contributing

Feel free to fork the project and submit a pull request with your changes!

## License

MIT License
