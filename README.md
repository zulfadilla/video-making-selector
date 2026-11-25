# Video Graphics Maker

A single-page tool for making motion-graphics videos: pick a style, write a script, press **Create Video**.

Everything runs in your browser. No server, no account and no uploads.

## How to use
1. Open `index.html` in Google Chrome or Microsoft Edge (double-clicking it works).
2. Pick the **video length** (Auto, or 15s up to 2 min).
3. Write the script. Each line is one scene.
4. Optionally add a voiceover, images, music and your own background.
5. Press **▶ Preview** to check it, or **Create Video** to record and download it. Chrome and Edge give MP4; other browsers give WebM.

> Keep the tab open while recording. The video is recorded in real time.

## Example scripts
The **Examples** menu in the Script section loads a ready-made script (with Undo):
Fun facts, Product launch, Tips list, Business results, Event promo, Motivational quote, and an Images demo.

```
# 5 Habits for a Productive Morning
Wake up at the *same time* every day
Drink a glass of water first
Your morning routine:
- Make your bed
- Move your body for 10 minutes
- Plan your top 3 tasks
Skip your phone for the first 30 minutes
Small habits, *big* results
```

## Online version
The same tool is published as a claude.ai artifact, so it also opens on a phone.
- The online version saves the finished video through the page's own save prompt.
- The microphone can't be used directly online. On a phone, record each line with the phone's voice recorder app, then press **⬆ Upload clip** on that scene (or upload one file with **Voice file**).

## Script format
| Write | Result |
|---|---|
| `# Title` | Big title scene with an accent underline |
| `- item` | List; items appear one by one (a line ending in `:` right before it becomes the list heading) |
| `*word*` | Word highlighted in the accent colour |
| Short line with a number (`60%`, `$5,000`, `33 million`) | Big number that counts up |
| `[image: logo, pop, left]` | Image inside the scene (see below) |
| Normal line | Text scene |

## Video length
Choose **Auto** (follows the script, max 2 minutes) or a fixed length: 15s, 30s, 45s, 1 min, 1.5 min or 2 min. All scenes are stretched or shortened to fit.

## Voiceover
- **Record your voice:** each scene has a 🎙 Record button. Read the scene's text, then press ■ Stop. Each scene is made at least as long as your recording, and silence at the start and end is trimmed. You can listen (▶), redo or remove a recording.
- **Voice file:** upload one MP3, WAV or M4A for the whole video, for example an AI voice from ElevenLabs or CapCut. Tick "Match video length to the voice" to make the video as long as the voice.
- Background music is lowered automatically while there is a voice.
- The browser's built-in robot voice can't be recorded into a video file, so it isn't offered.

## Images in scenes
Upload images, logos or icons under **Images in scenes**, below the script. Each image is named after its file name. To add one to the script:
1. Choose an animation, position, size and motion.
2. Put the cursor in the script.
3. Click **+ Insert** on the image.

Or type the command yourself:

```
[image: logo, bounce, right, large, float, 1s]
```

| Type | Options |
|---|---|
| Entrance animation | `pop` `fade` `zoom` `from-left` `from-right` `from-top` `from-bottom` `rotate` `bounce` |
| Position | `center` `top` `bottom` `left` `right` `full` (full-screen image behind the text) |
| Size | `small` `medium` `large` |
| Continuous motion | `float` `wiggle` `spin` |
| Timing | `1s`, `0.5s`, … = appear after that many seconds |

- You can use a number instead of a name: `[image: 2]` is the second image in the list.
- A line with only an image becomes a big image scene.
- Several image commands on one line place the images side by side.
- In a list, `- [image: icon] Item` uses the icon instead of the bullet.
- In 9:16 videos, `left` and `right` become `top` and `bottom` automatically.
- Malay commands from older versions, such as `[gambar: logo, lantun, kiri]`, still work.

## Style options
- **Colour themes (18):**
  - Dark: Neon Night, Dark Elegant, Green Nature, Sunset, Ocean, Aurora, Royal Purple, Crimson Night, Cyber Yellow, Coffee, Retro Wave, Monochrome
  - Light: Corporate, Pop Bright, Minimal Paper, Candy Pastel, Fresh Mint, Sky Blue
  - You can also set a custom accent colour.
- **Background source:**
  - **Theme**
  - **Custom colour:** one or two colours.
  - **Custom image:** several images in any order, shown one per scene or spread evenly. Includes a crossfade, slow zoom and a dark or light overlay.
- **Background decoration:** Gradient, Particles, Grid, Shapes, None
- **Text animation:** Word pop, Fade up, Typewriter, Slide, Zoom, Random
- **Scene transition:** Fade, Wipe, Slide, Zoom
- **Transition sound:** None, Whoosh, Swoosh, Pop, Click, Ding, Swipe, Riser, Glitch, Impact. Click one to hear it.
- **Background music:**
  - Chill or Upbeat, generated in the browser
  - Your own MP3, WAV, M4A or OGG, with volume, loop and start-at-second controls
- **Other:** format (16:9, 9:16, 1:1, 4:5), font, pace, quality (720p or 1080p), closing text, watermark, progress bar

Images, music and voice recordings are saved in the browser (IndexedDB), so they are still there next time you open the tool.
