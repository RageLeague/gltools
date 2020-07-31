# Griftlands Tools

A set of two command line converter tools for the [Griftlands](https://store.steampowered.com/app/601840/Griftlands/) video game created by [Klei Entertainment](https://klei.com/).

## Requirements

Both tools require [Python 3.8 (or higher)](https://www.python.org/downloads/) with the [Pillow](https://python-pillow.org/) fork of the Python Imaging Library.

## Griftlands Tex to PNG Converter (glt2p.py)

This tool converts Griftlands .tex files to .png files.

#### General Usage:

To convert `atlas0.tex` to `atlas0.png`:

    $ python glt2p.py atlas0.tex

To convert all `*.tex` files located in a directory named `folder` to `*.png` files:

    $ python glt2p.py folder

#### Full Usage:

    $ python glt2p.py [-h] [-ver] <input-file/input-directory>
    
    -h, --help
        Displays usage information and exits
    -ver, --version
        Displays version information and exits

## Griftlands Bin to SCML Converter (glb2s.py)

This tool converts Griftlands anim.bin, atlas0.tex, and build.bin files to a [BrashMonkey Spriter](https://brashmonkey.com/spriter-pro/) (.scml) file.

As Spriter does not support free-form deformations nor does it support references between animations within a single project, the resultant Spriter file may not always have perfect animation fidelity to what's displayed within Griftlands.

#### General Usage:

To convert `anim.bin`, `atlas0.tex`, and `build.bin` located in a directory named `folder` to a `.scml` file and its associated images:

    $ python glb2s.py folder
    
#### Full Usage:

    $ python glb2s.py [-h] [-ver] <input-directory>
    
    -h, --help
        Displays usage information and exits
    -ver, --version
        Displays version information and exits
        
## Notice

These tools are provided by the author "AS IS" and WITHOUT WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
