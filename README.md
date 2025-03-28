# Wubby VOD Downloader (aka **Wubby Snatch**)

A simple script to snatch those autism VODs from the Wubby TV archive.

## Install this barely functioning ADHD fueled masterpiece

You can install this stupid package using pip from pypi

```bash
pip install wubby-vod-downloader==1.1.0
```

## Usage

Navigate to the directory where you want to store the VODs. The script will create a new folder named `vod_downloads` where the files will be saved

To download the latest VODs, run the following command

```bash
wubby-snatch month -c number_of_vods
```

## Arguments

- Month: Specify the month (in MMM_YYYY format) from which you want to download VODs

-c number_of_vods: Specify how many VODs you want to download. For example if you want the 5 most recent VODs, use `-c 5`

## Example

```bash
wubby-snatch mar_2025 -c 5
```

This will download the 5 most recent VODs from March 2025

## Important

- If a VOD has already been downloaded, the script will skip it and move on to the next one.

- After installing via pip, if you receive a warning about wubby-snatch not being in PATH, you may need to add ~/.local/bin to your PATH manually. This typically happens on Linux systems, and you can do it by adding

```bash
export PATH="$HOME/.local/bin:$PATH"
```

to the end of your `.bashrc` or `.zshrc`

## License

This project is licensed under the MIT License - see the LICENSE file for details if you care
