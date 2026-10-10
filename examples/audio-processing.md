# Audio Processing examples

## Transcribe a local recording

```bash
python tool.py transcribe --file_path meeting.m4a --model base
```

Returns JSON containing transcript text and timestamped segments. Audio stays local after the model is available.

## Generate remote TTS only with consent

```bash
python tool.py tts --text "Hello" --output_path hello.mp3 --lang en --allow-network
```

This sends the text to Google. Do not use the network flag for confidential text.
