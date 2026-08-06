# HTML Multimedia

## 📖 Introduction

HTML provides multimedia elements to display audio and video directly on a webpage without requiring external plugins.

Common multimedia includes:

- Audio
- Video
- YouTube Videos
- PDFs
- Maps

---

# Multimedia Tags

| Tag | Purpose |
|------|----------|
| `<audio>` | Play audio |
| `<video>` | Play videos |
| `<source>` | Specify media files |
| `<iframe>` | Embed external content |

---

# HTML Audio

Syntax

```html
<audio controls>

    <source src="audio/song.mp3"
            type="audio/mpeg">

    Your browser does not support audio.

</audio>
```

---

# Audio Attributes

| Attribute | Purpose |
|-----------|---------|
| controls | Shows play controls |
| autoplay | Starts automatically |
| muted | Starts muted |
| loop | Repeats continuously |

---

# HTML Video

Syntax

```html
<video
    controls
    width="500">

    <source
        src="video/sample.mp4"
        type="video/mp4">

    Your browser does not support video.

</video>
```

---

# Video Attributes

| Attribute | Purpose |
|-----------|---------|
| controls | Show controls |
| autoplay | Play automatically |
| muted | Start muted |
| loop | Repeat video |
| width | Video width |
| height | Video height |
| poster | Thumbnail before playback |

---

# Example: Poster Image

```html
<video
    controls
    width="500"
    poster="images/thumbnail.jpg">

    <source
        src="video/demo.mp4"
        type="video/mp4">

</video>
```

The `poster` image is displayed before the user starts the video.

---

# Embedding YouTube Videos

```html
<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/VIDEO_ID"
    title="YouTube Video"
    allowfullscreen>
</iframe>
```

Replace `VIDEO_ID` with the video's ID.

---

# Embedding Google Maps

```html
<iframe
    src="YOUR_GOOGLE_MAP_EMBED_LINK"
    width="600"
    height="450"
    loading="lazy">
</iframe>
```

---

# Supported Audio Formats

- MP3
- WAV
- OGG

---

# Supported Video Formats

- MP4
- WebM
- OGG

---

# Best Practices

- Use MP4 for videos.
- Use MP3 for audio.
- Always include fallback text.
- Avoid autoplay unless necessary.
- Compress media files for faster loading.

---

# Common Mistakes

❌ Very large media files

❌ Missing `controls`

❌ Incorrect file paths

❌ Using unsupported formats

---

# Interview Questions

### What is the purpose of the `<audio>` tag?

It embeds audio into a webpage.

---

### What is the purpose of the `<video>` tag?

It embeds videos into a webpage.

---

### Why do we use `<source>`?

To specify the media file and its format.

---

### What does the `controls` attribute do?

It displays playback controls like Play, Pause, and Volume.

---

### What is the `poster` attribute?

It displays a thumbnail image before the video starts.

---

# Summary

HTML multimedia elements allow websites to play audio and video without external plugins. They improve user engagement and are widely used in modern web applications.