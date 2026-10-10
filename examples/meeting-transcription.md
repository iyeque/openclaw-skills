# Meeting Transcription examples

## Create a local transcript package

```bash
python3 skills/meeting-transcription/meeting.py \
  --input meeting.m4a \
  --model base \
  --language en \
  --output-dir meeting-output \
  --format all
```

The workflow writes JSON with timestamped segments, SRT subtitles, and Markdown notes. It does not call a cloud transcription API; first-time Whisper model acquisition may require network access.

## Extract a transcript only

```bash
python3 skills/meeting-transcription/meeting.py \
  --input interview.wav \
  --model small \
  --format json
```

Use the timestamps in `transcript.json` when citing decisions or action-item candidates.
