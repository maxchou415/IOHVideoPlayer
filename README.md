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

## Options
You can add more buttons before any `<script>` tag, and HTML code like
```html
<button id="target4" class="btn btn-primary text-center">Jump to 10</button>
```
also, you need add control to your jQuery like,
```javascript
$( "#target4" ).click(function() {
        playerSeekTo(player, 600)
  });
```
