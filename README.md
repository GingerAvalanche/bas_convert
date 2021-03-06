# Breath of the Wild Binary Animation Sequence Convert
Converts Binary Animation Sequence (.bas) files from machine code to human-readable format and replaces TypeIndex values with names (or vice versa). For LoZ:BotW

Note: Only one of the TypeIndex enums has official names. These names are listed on https://zeldamods.org/wiki/Bas. The other TypeIndex enums have been given unofficial names, also listed on that page. (NOTE: unofficial name conversion has not been implemented yet)

## Dependencies
* A dumped copy of Legend of Zelda: Breath of the Wild (for Wii U or Switch)
* Python 3.7+ (64-bit, added to system PATH)

The following `pip` packages, which will be automatically installed:
* oead

## Setup
1. Download and install Python 3.7+, 64-bit. You must choose the "Add to System PATH" option during installation.
2. Open a command line and run `pip install bas_convert`

### How to Use
```bas_convert [file] [output] [-n] [-d]```
* `file` - The name of the file to convert. You can select multiple files by using wildcards. (e.g. `*.yml` will select all `.yml` files in the directory)
* `output` - The type to output as. Accepts `yml`, `yaml`, `bas`, and `aamp`. `yml` and `yaml` are YAML, human-readable. `bas` and `aamp` are AAMP, machine-readable.
* `-n` - Outputs the file with TypeIndex conversions to names.
* `-d` - Outputs the file with TypeIndex conversions to digits (numbers).

* All permutations of conversion have been supported, for use with tools such as `hyrule_builder` which will convert to YAML for you.

## Contributing
* Issues: https://github.com/GingerAvalanche/bas_convert/issues
* Source: https://github.com/GingerAvalanche/bas_convert

This software is in early, but usable, beta. There are many TypeIndex types that are not yet converted, or even mapped out. Any support is appreciated.

## License
This software is licensed under the terms of the GNU Affero General Public License, version 3+. The source is publicly available on Github.
