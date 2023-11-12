# Bookmarklet to fast-forward YouTube ads

1. Set video speed to 10
2. Click the <kbd>Skip ad</kbd> button

## Usage

Add a bookmark to your browser with the URL in the [`bookmarklet.url`](./bookmarklet.url) file.
Set name to ⏩

## Source code

```javascript
document.querySelector("#container video.html5-main-video").playbackRate = 10;
document.querySelector("[id^=ad-text].ytp-ad-skip-button-text").click();
```

Made with `chriszarate/bookmarkleter`
