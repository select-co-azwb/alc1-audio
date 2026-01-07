# Minimal Listening Template (GitHub Pages)

This is a tiny, no-tracking listening page:
- HTML5 audio player
- Transcript in a dropdown
- Transcript highlights as the audio plays
- Click a line to jump to that time

## Folder structure
- index.html
- styles.css
- script.js
- /audio/
  - sample.mp3  (you replace this)
- /vtt/
  - sample.vtt  (you replace this)

## How to add your own track
1) Put your MP3 in `/audio/` (example: `audio/01_story.mp3`)
2) Create a matching WebVTT file in `/vtt/` (example: `vtt/01_story.vtt`)
3) In `index.html`, copy the Track section and update:
   - `<source src="audio/01_story.mp3" ...>`
   - `<track ... src="vtt/01_story.vtt" ...>`
   - Title text (Track name)

## Making a .vtt transcript
Format:

WEBVTT

00:00.000 --> 00:03.200
First line of dialogue.

00:03.200 --> 00:06.900
Second line of dialogue.

Tips:
- Use periods in timestamps (00:03.200), not commas.
- Keep lines short-ish for phone readability.

## GitHub Pages quick publish
- Put these files in a repo (root).
- Settings → Pages → Deploy from branch (main / root).
- Your site URL will appear there.
