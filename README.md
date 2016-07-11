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
### Add button
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
### Resize video size
First, should be you don't need resize it, because this plugin has RWD (Responsive Web Design) already, but if you just want resize it, just change here:

```javascript```
var player;
      function onYouTubeIframeAPIReady() {
        player = new YT.Player('player', {
          height: '390', //here is your height
          width: '640', //here is your width
          videoId: '', 
          playerVars: { 'autoplay': 1, 'controls': 1},
          events: {
            'onStateChange': onPlayerStateChange
          }
        });
      }
```

### More options
You can see [YouTube Player API Reference for iframe Embeds](https://developers.google.com/youtube/iframe_api_reference)
