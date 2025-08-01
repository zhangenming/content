---
title: "VTTCue: size property"
short-title: size
slug: Web/API/VTTCue/size
page-type: web-api-instance-property
browser-compat: api.VTTCue.size
---

{{APIRef("WebVTT")}}

The **`size`** property of the {{domxref("VTTCue")}} interface represents the size of the cue as a percentage of the video size.

## Value

A number representing the size of the cue as a percentage of the video size.

## Examples

In the following example a new {{domxref("VTTCue")}} is created, then the value of `size` is set to `50`. The value is then printed to the console.

```js
let video = document.querySelector("video");
let track = video.addTextTrack("captions", "Captions", "en");
track.mode = "showing";

let cue = new VTTCue(0, 0.9, "Hildy!");
cue.size = 50;
console.log(cue.size);

track.addCue(cue);
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
