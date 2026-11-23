# Awake or Asleep Detector

A school project (VG1 IT, Haugaland) where an image model recognizes whether I am **awake** or **asleep** using my webcam.

## How it works
- The model was trained with [Teachable Machine](https://teachablemachine.withgoogle.com/) using webcam images of me awake and asleep.
- The web page (`index.html`) loads the model, turns on the webcam, and shows the prediction live.
- The page code was made with the help of Claude (Anthropic).

## Files
- `index.html` – the web page with the code
- `my_model/` – the exported Teachable Machine model (`model.json`, `metadata.json`, `weights.bin`)

## How to run
1. Put the exported model files in the `my_model` folder.
2. Open the GitHub Pages link for this repository (or run a local web server), click **Start**, and allow the webcam.

## Classes
- Awake
- Asleep
- Nobody (optional)

## Alarm
When the model is at least 80% sure I am asleep, the page plays a beep every second.
