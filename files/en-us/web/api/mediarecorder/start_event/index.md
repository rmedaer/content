---
title: 'MediaRecorder: start event'
slug: Web/API/MediaRecorder/start_event
tags:
  - API
  - Audio
  - Media Capture
  - Media Recorder API
  - MediaRecorder
  - Event
  - Reference
  - Video
  - start
browser-compat: api.MediaRecorder.start_event
---
{{APIRef("Media Recorder API")}}

The `start` event is fired when
{{domxref("MediaRecorder.start()")}} is called. At this point, the data
starts being gathered into a {{domxref("Blob")}}.

## Syntax

Use the event name in methods like {{domxref("EventTarget.addEventListener", "addEventListener()")}}, or set an event handler property.

```js
addEventListener('start', event => { });

onstart = event => { };
```

## Event type

A generic {{domxref("Event")}}.

## Example

```js
...

  record.onclick = function() {
    mediaRecorder.start();
    console.log("recorder started");
  }

  mediaRecorder.onstart = function() {
    // do something in response to
    // recording being started
  }

...
```

## Properties

None.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [Using
  the MediaRecorder API](/en-US/docs/Web/API/MediaStream_Recording_API/Using_the_MediaStream_Recording_API)
- [Web Dictaphone](https://mdn.github.io/web-dictaphone/): MediaRecorder +
  getUserMedia + Web Audio API visualization demo, by [Chris Mills](https://twitter.com/chrisdavidmills) ([source on GitHub](https://github.com/mdn/web-dictaphone/).)
- [simpl.info MediaStream Recording
  demo](http://simpl.info/mediarecorder/), by [Sam Dutton](https://twitter.com/sw12).
- {{domxref("Navigator.getUserMedia")}}
