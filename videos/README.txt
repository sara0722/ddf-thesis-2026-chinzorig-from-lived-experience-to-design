Put your compressed web videos here.

Faculty policy: thesis videos are NOT hosted on YouTube or other external
platforms. They live in this repository and play via the native HTML5
player in index.html.

Rules:
- Format: MP4, H.264 video + AAC audio (plays everywhere)
- Resolution: 1080p; drop to 720p if needed to hit the size target
- Size: target <= 50 MB per file. GitHub HARD-REJECTS files over 100 MB.
- Length: demo max. 2 minutes; optional longer walkthrough
- Always reference a poster image (images/video-poster.jpg) in the
  <video> tag so the page loads fast
- These compressed files count toward your repository ZIP - keep it lean

Compression recipe (ffmpeg):
  ffmpeg -i master.mov -c:v libx264 -crf 26 -preset slow \
         -vf "scale=-2:1080" -c:a aac -b:a 128k -movflags +faststart demo.mp4
  (raise -crf to 28-30 for smaller files; -movflags +faststart enables
  instant playback in the browser)

Too big even at 720p / crf 30?
  Shorten the video. HARD LIMIT: every file in this repository must stay
  under 100 MB - GitHub rejects larger files, no exceptions. The web page
  needs a concise demo; the full-length master is handed in separately.

Master files:
  The uncompressed masters are handed in separately via the faculty
  upload channel - the versions here are for the web page, not the archive.
