# Free VAST/VMAP JS Plugin JW Player
## without any License key
<a target="_blank" href="https://camo.githubusercontent.com/3f3ead5def54346308bb4604debc31c039c85cb5/687474703a2f2f7777772e6a77706c617965722e636f6d2f77702d636f6e74656e742f75706c6f6164732f4a57502d4769744875622d42616e6e65722d312e706e67"><img height="70px" style="max-width:100%;" data-canonical-src="http://www.jwplayer.com/wp-content/uploads/JWP-GitHub-Banner-1.png" title="JW Player Logo" alt="JW Player Logo" src="https://camo.githubusercontent.com/3f3ead5def54346308bb4604debc31c039c85cb5/687474703a2f2f7777772e6a77706c617965722e636f6d2f77702d636f6e74656e742f75706c6f6164732f4a57502d4769744875622d42616e6e65722d312e706e67"></a>
### VAST/VPAID Advertising For The Most Popular HTML5 Player And Video Platform
<br>
Cross-platform, free and open-source VAST jwPlayer


# Usage
<ul>
<li>clone the project</li>
<li>call jwplayer and config it</li>
<li>upload VmapJwPlayer.js to your server</li>
<li>Enjoy it :)</li>
</ul>

```javascript
<script type="text/javascript">
    var playerInstance = jwplayer("video");
    playerInstance.setup({
        aspectratio: "16:9",
        stretching:'uniform',
        playlist: [{
            sources: [

                {
                    file:  'http://example.com/video.mp4'  ,
                    label: '240',
                    type:"video/mp4"
                    ,"default": "true"
                }

            ],
            title: "Your Video Title",
            description: "Your Video Description",
            image: "Your Video Poster"
        }],
        plugins: {
            "http://example.com/VmapJwPlayer.js": {},
        }
        ,advertising:{
            client:"vast",
            schedule:"VMAP XML DATA URL",
        }
        primary: "html5",
    });
</script>
```

| FORMAT  | TYPE |
| ------------- | ------------- |
| Linear  | MP4, FLV,MP4,JPG,PNG,GIF  |
| Non-linear  | MP4, FLV,MP4,JPG,PNG,GIF  |
| Skippable Linear	  | MP4, FLV,MP4,JPG,PNG,GIF  |


# Note
    ES6 Version and NPM Package coming soon :)

## License
    Attribution-NonCommercial 3.0 Unported (CC BY-NC 3.0)
    (C) 2016 - miladheydari.ir @iammilaad
    https://creativecommons.org/licenses/by-nc/3.0/
