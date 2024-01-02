# Documentation for Transcribing Audio to SRT using Whisper

## Introduction
This Python script utilizes the Whisper ASR (Automatic Speech Recognition) library to transcribe audio files and generate corresponding SRT (SubRip Subtitle) files. The script provides a command-line interface for ease of use.

## Prerequisites
Make sure you have the necessary libraries installed before running the script. You can install them using the following command:
```bash
pip install whisper
```

## Usage
To transcribe an audio file to an SRT file, use the following command format:
```bash
python script_name.py input_audio output_srt model
```

- `input_audio`: Path to the input audio file.
- `output_srt`: Path to the output SRT file.
- `model`: Name of the Whisper ASR model. Choose from the available models: [List of available models]

## Functions

### `format_time(seconds)`
This function takes a time in seconds and returns a formatted string in HH:MM:SS,mmm format.

#### Parameters
- `seconds` (float): Time in seconds.

#### Returns
- `formatted_time` (str): Formatted time string.

### `transcribe_audio(input_audio, output_srt, model)`
This function transcribes the provided audio file using the Whisper ASR model and saves the result as an SRT file.

#### Parameters
- `input_audio` (str): Path to the input audio file.
- `output_srt` (str): Path to the output SRT file.
- `model` (str): Name of the Whisper ASR model.

#### Raises
- `Exception`: If the specified ASR model is not available.

## Example
```bash
python script_name.py path/to/audio.wav path/to/output.srt model_name
```

## Note
Ensure that the specified ASR model is supported by Whisper. You can choose from the available models by running:
```bash
python script_name.py --help
```

## License
This script is released under [License Name]. See the [LICENSE](link_to_license_file) file for more details.
