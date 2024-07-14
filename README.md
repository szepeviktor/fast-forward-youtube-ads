# Bookmarklet to fast-forward YouTube ads

1. Seek to the end
2. Click the <kbd>Skip ad</kbd> button

## Usage

Add a bookmark to your browser with the URL in the [`bookmarklet.url`](./bookmarklet.url) file.
Set name to ⏩

## Source code

```javascript
var skipButton = document.querySelector("[id^=skip-button].ytp-skip-ad-button");
if (skipButton !== null) {
    skipButton.click();
} else {
    var video = document.querySelector("video.html5-main-video[src]");
    video.currentTime = video.duration - 1;
    video.playbackRate = 2;
}
```

Made with `chriszarate/bookmarkleter`
