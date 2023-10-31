# vobsub-to-srt

Script takes a videofile and exteracts subtitles, saves them to .srt. It's using tesseract for OCR and because it's OCR it's inherently not perfect.

```
Usage: ./vobsub-to-srt [OPTIONS] FILE
  -h, --help        Display this help message
  --id ID           Set the ID of subtitle stream (optional)
  --lang LANG       Set the language (optional, default: eng)
  --all             Use the --all flag extract all vobsubs (takes a long time)

Example:
  ./vobsub-to-srt --id 6 /path/to/file
  ./vobsub-to-srt --lang eng /path/to/file
  ./vobsub-to-srt --all /path/to/file
```

## Dependencies
These are needed to run: `jq, ogmrip, tesseract-ocr`
To install them run: `sudo apt install jq ogmrip tesseract-ocr`

## Installation:
```
git clone https://github.com/JSubelj/vobsub-to-srt.git vobsub-to-srt
chmod u+x vobsub-to-srt/vobsub-to-srt
sudo apt update && sudo apt install jq ogmrip tesseract-ocr
```
