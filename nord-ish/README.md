# 🎧 rmpc Minimal GNOME Theme

Minimal, functional rmpc theme with album art + cava pane.
Designed for **GNOME + WezTerm** with a cool minimal dark look.

## Preview

![preview](rmpc_1.png)

Layout:

* Queue on left
* Album art on right
* Cava visualizer under album art
* Clean header + progress bar

---

## Features

* Minimal nord-ish colors
* Album art support
* Built-in cava pane inside rmpc

---

## Requirements

You must have:

* `rmpc` + `cava`

---

## Install

Clone repo:

```bash
git clone https://github.com/Rimuren/nord-theme-rmpc/edit/main/nord-ish.git
cd rmpc-theme
```

## Notes

* This repo only provides **rmpc theme + layout**
* You must already have MPD configured
* Cava is required for visualizer pane (if you want it, deactivate it in the .ron files )
* FIFO must match:

```
/tmp/mpd.fifo
```

Make sure your `mpd.conf` contains:

```
audio_output {
    type            "fifo"
    name            "fifo"
    path            "/tmp/mpd.fifo"
    format          "44100:16:2"
}
```

## 📜 License

MIT

