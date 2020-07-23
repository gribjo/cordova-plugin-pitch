# cordova-plugin-pitch

This plugin captures the device's audio input stream and analyses it to return the maximum frequency.

It adds the following `window` event:

* audiofrequency

## Installation

```
cordova plugin add https://github.com/gribjo/cordova-plugin-pitch.git
```

## Supported Platforms

* iOS
* Android

## Example

```javascript
window.addEventListener("audiofrequency", onAudiofrequency, false);

function onAudiofrequency(e) {
    console.log("Frequency: " + e.frequency + " Hz");
}
```
