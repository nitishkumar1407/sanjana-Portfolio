# Sanjana Sahni Portfolio

A responsive editorial-style portfolio for Sanjana Sahni — Content Writer, Video Editor and Social Media Manager.

## Portfolio sections
- Home — personal introduction and rotating showcase.
- About Me
- Skills
- My Work
  - All
  - Writing
  - Videos
  - Posters
- Experience
- Contact

## Current work counts
- 18 poster portfolio cards
- 6 video portfolio cards
- 5 writing samples

## Video setup
The Videos section uses vertical 9:16 Reel-style frames. Each video has native HTML5 playback, a Reel number badge and a dedicated "View Reel on Instagram" button.

The six local video files are:
- `assets/videos/video-01.mp4`
- `assets/videos/video-02.mp4`
- `assets/videos/video-03.mp4`
- `assets/videos/Video-04.mp4`
- `assets/videos/Video-05.mp4`
- `assets/videos/Video-06.mp4`

### Add Instagram Reel URLs
Open `script.js` and edit the `instagramReelLinks` object near the top:

```js
const instagramReelLinks = {
  "01": "https://www.instagram.com/reel/YOUR_REEL_01/",
  "02": "https://www.instagram.com/reel/YOUR_REEL_02/",
  "03": "https://www.instagram.com/reel/YOUR_REEL_03/",
  "04": "https://www.instagram.com/reel/YOUR_REEL_04/",
  "05": "https://www.instagram.com/reel/YOUR_REEL_05/",
  "06": "https://www.instagram.com/reel/YOUR_REEL_06/"
};
```

The same URL is automatically applied wherever that Reel appears, including the All and Videos views.

Until a URL is supplied, the button opens the portfolio Instagram profile instead of a broken placeholder URL.

## Adding more videos
1. Put the MP4 file in `assets/videos/`.
2. Add a matching video card in the Videos view.
3. Add the Reel URL to `instagramReelLinks` in `script.js`.
4. If the video should appear in the Home showcase or All view, add it there too.

## Local preview
For reliable local video playback, run a small HTTP server from the project folder:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000/` in your browser.
