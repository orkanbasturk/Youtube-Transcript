YouTube Transcript Downloader

A Python-based terminal application to download transcripts of YouTube videos. This application supports multi-language transcript selection and saves the transcript as a text file in the `output` directory.

## Features

- Extracts transcripts from YouTube videos using video links.
- Supports multiple video links separated by commas.
- Allows language selection for transcripts.
- Automatically creates an `output` directory for saving text files.
- Fetches video titles to name the transcript files.
- Removes unwanted text like `[Applause]`, `[Music]`, etc., from transcripts.

## Prerequisites

- Python 3.7 or higher

### Required Libraries
Install the required libraries using `pip`:

```bash
pip install youtube-transcript-api requests beautifulsoup4
```

## How to Use

1. Clone this repository or copy the code to your local machine.
2. Navigate to the directory containing the script.
3. Run the script using Python:

```bash
python youtube_transcript_app.py
```

4. When prompted, enter YouTube video links separated by commas. For example:

```
https://youtu.be/abc123, https://youtu.be/def456
```

5. For each video, the application will list available languages. Enter the language code (e.g., `en` for English, `tr` for Turkish) to download the transcript.
6. The transcripts will be saved in the `output` directory with the video title as the file name.

## Notes

- If a video does not have transcripts available, the application will skip it and proceed to the next video.
- For videos with disabled transcripts, you will see an error message, and the application will continue processing other links.

## Example Output

```
[INFO] Created output folder at /path/to/output
[INFO] Processing: https://youtu.be/abc123
Available languages:
- English (en)
- Turkish (tr)
Enter the language code you want to download the transcript in: en
[INFO] Transcript saved to /path/to/output/Video_Title.txt
```

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Contributions

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/orkanbasturk/Youtube-Transcript/issues).

## Author

Developed by Orkan Baştürk
basturkorkan@gmail.com

