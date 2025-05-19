# SPL Parser

SPL Parser is a command-line application for parsing Splunk’s Search Processing
Language (SPL).\
Its main feature is generating a `tmLanguage` grammar for SPL to enable syntax
highlighting in various text editors.\
It can also interactively display details about any SPL command.

## Features

- Generate `tmLanguage` grammar for SPL for syntax highlighting
- View details about any SPL command
- Use a remote Splunk server or local files

## Installation

To install using [`uv`](https://github.com/astral-sh/uv):

```bash
uv pip install --extra-index-url https://test.pypi.org/pypi spl_parser

Or clone this repository and install in editable mode:

git clone https://github.com/kotlaluk/spl-parser
cd spl-parser
uv pip install -e .

Usage

The SPL Parser CLI can be invoked via:

spl_parser --help

It works in two modes:
- remote: connect to a live Splunk server (URL required)
- local: use a local searchbnf.conf or .json file

Credentials for remote mode can be supplied via prompt or the SPLUNK_USERNAME and SPLUNK_PASSWORD environment variables.

### Example (remote, view command)

This repo contains a VSCode extension for SPL syntax highlighting:
	1.	Generate the grammar file (spl.tmLanguage.json)
	2.	Copy it into: spl-highlighter/syntaxes/
	3.	Install the extension by copying the spl-highlighter/ folder into your VSCode extensions directory (e.g. ~/.vscode/extensions/)

Files ending in .spl will be highlighted automatically.
The extension includes an optional “SPL Theme” with colours inspired by Splunk Web.

This repo contains a VSCode extension for SPL syntax highlighting:
1. Generate the grammar file (spl.tmLanguage.json)
2. Copy it into: spl-highlighter/syntaxes/
3. Install the extension by copying the spl-highlighter/ folder into your VSCode extensions directory (e.g. ~/.vscode/extensions/)
uv pip install -e ".[test]"
pytest

Documentation
## Testing

To run tests:
Then open docs/_build/html/index.html in your browser.

Author

Lukáš Kotlaba (lukas.kotlaba@gmail.com)

License

To build locally:
Lukáš Kotlaba (lukas.kotlaba@gmail.com)

## License
```
