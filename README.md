# IOHVideoPlayer

First you need insert your YouTube Video ID into `:46`, like

```javascript
var player;
      function onYouTubeIframeAPIReady() {
        player = new YT.Player('player', {
          height: '390',
          width: '640',
          videoId: '', //Insert you youtube video id right here!
          playerVars: { 'autoplay': 1, 'controls': 1},
          events: {
            'onStateChange': onPlayerStateChange
          }
        });
      }
```

 All Done! You just need deploy to your server now.
