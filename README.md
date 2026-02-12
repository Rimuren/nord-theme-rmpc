# 🎧 rmpc Minimal GNOME Theme

Minimal and functional rmpc layout with album art + cava pane.

## Preview
![preview](nord-ish/rmpc_1.png)

**Layout**

* Queue on the left
* Album art on the right
* Cava visualizer under album art
* Clean header + progress bar

---

## Features

* Minimal nord-ish colors
* Album art support
* Built-in cava pane inside rmpc

---

## Requirements

You need:

* `rmpc`
* `mpd`
* `cava` *(optional but enabled by default)*

> If you don’t want cava, disable it in the `.ron` config.

---

## Install

```bash
git clone https://github.com/Rimuren/nord-ish-rmpc.git
```

Then place the config in your rmpc config directory.

---

## MPD FIFO (for cava)

This is the FIFO setup I personally use.
Feel free to change the path or settings to match your own MPD configuration.

Make sure your `mpd.conf` includes something like:

```
audio_output {
    type            "fifo"
    name            "fifo"
    path            "/tmp/mpd.fifo"
    format          "44100:16:2"
}
```

The FIFO path in the rmpc config should match whatever you use in MPD.
In my case, it is:

```
/tmp/mpd.fifo
```

---

## Notes

* This repo only provides **rmpc layout + theme**
* MPD must already be configured
* Cava is only required if you want the visualizer pane

---

## warning

uploaded with zero polish.

if you know, you know.
if it breaks, you fix it.
use at your own risk.
