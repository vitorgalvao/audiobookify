# Audiobookify

Audiobookify is a command-line tool to concatenate a folder of audio files into a single M4B audiobook file with chapters. Chapter markers are set at the starting point of each original file and use the file name as the title.

## Installation

Install with [Homebrew](https://brew.sh):

```shell
brew install vitorgalvao/tiny-scripts/audiobookify
```

Alternatively, download the executable at the root of this repository and call it directly. Ensure you have [`ffmpeg`](https://ffmpeg.org) and [`mp4v2`](https://mp4v2.org) installed and in your `PATH`.

## Usage

```
Concatenate folder of audio files into a single M4B audiobook file with chapters.
Chapter markers are set and the starting point of each original file and use the file name as the title.

Input and output are mandatory. Other flags are optional.
If no author, title, or cover are provided, audiobookify will attempt to extract them from the metadata of the first found audio file.

Usage:
  audiobookify --input <folder> --output <file> --title <name> --author <name> --cover <file>

Options:
  -i, --input    Folder of audio files to convert.
  -o, --output   Output file to save.
  -t, --title    Title to embed.
  -a, --author   Author name to embed.
  -c, --cover    Image to embed as cover.
  -h, --help     Show this help.
```

## License

3-Clause BSD
