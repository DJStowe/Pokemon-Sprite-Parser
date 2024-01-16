README
Overview

This tool is a specialized Python program designed to assist in the creation of custom maps for a Tabletop Role-Playing Game (TTRPG) based on the Nintendo property Pokemon Mystery Dungeon. It processes sprite sheets containing various wall and floor sprites and separates each sprite into individual, smaller pieces. These pieces can then be used to craft custom maps for the game.
Features

    Sprite Extraction: Extracts individual sprites from a larger sprite sheets downloaded from https://www.spriters-resource.com

Requirements

    Python 3.x
    png Python library (for handling PNG files)

Installation

    Ensure Python 3.x is installed on your system.
    Install the png library using pip:

    pip install pypng

Usage

    Place the sprite sheet(s) in the src folder.
    Run the script from the command line:

    python path_to_script.py

    Extracted sprites will be saved in the output folder, organized into subfolders named after the original sprite sheet file.

Code Structure

    ImgProcessor: Class that handles the image processing logic.
        isTile: Determines if a given part of the sprite sheet is a valid tile.
        PixelAddition: Calculates the position of the next pixel to be processed.
        CurrPixelLocation: Determines the current pixel's coordinates.
        WriteTile: Writes an individual tile as a PNG file.
    main: Orchestrates the overall process, handling file operations and user feedback.
    OpenFile: Opens a sprite sheet file and initiates the extraction process.

Limitations and Notes

    This tool is specifically designed for sprite sheets of a certain format, as used in Pokemon Mystery Dungeon from https://www.spriters-resource.com
    The tool does not provide a GUI and requires basic knowledge of command line operations.
    The tool is part of a larger project and may require context from other components for full functionality.

Contributing

    Contributions to the project are welcome. Please follow standard GitHub pull request procedures for contributions.

License

    Distributed under the GNU General Public License v3.0. See LICENSE for more information.

Disclaimer

This tool is not officially affiliated with Nintendo or the Pokemon franchise. It is intended for fan-made, non-commercial use only.