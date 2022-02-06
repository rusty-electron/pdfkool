# pdfkool

a simple wrapper script to compress pdfs using ghostscript

Poor humour: `In the world of pdf tools, be a pdf kool`

## Requirements
Platform: `*NIX`
* `ghostscript`
* GNU utils like `du, awk, getopt`, etc that are installed by default on most *nix distros

## Installation

1. **Temporary method**: Copy the `pdfkool` script to a directory which in in your PATH

> I will add an install script soon

2. Make it executable

```bash
chmod +x pdfkool
```

## Usage

```
pdfkool [OPTION]...

A simple wrapper script to compress pdfs using ghostscript

 Options:
  -i, --input          Path to input pdf file
  -o, --output         Path to output pdf file
  -Q, --quality        Specify quality setting for output file (See QUALITY below)
  -q, --quiet          Quiet (no output)
  -p, --preserve-links Preserve hyperlinks
  -l, --log            Print log to file
  -h, --help           Display this help and exit
  -v, --version        Output version information and exit

 QUALITY:
    screen   (screen-view-only quality, 72 dpi images)
    ebook    (low quality, 150 dpi images)
    printer  (high quality, 300 dpi images)
    prepress (high quality, color preserving, 300 dpi imgs)
    default  (compatible for various use case, large file usually)
```

## Features

[x] compress files
[ ] rotate pages

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](./LICENSE)
