# fullscreenxray
## Enable fullscreen mode for x-ray bonus content (such as for Wheel of Time episodes) on Amazon Prime
If you pause a video on Amazon Prime, you can access bonus content for that video by clicking "x-ray" in the upper left corner. Videos in this section are often impossible to play in fullscreen, despite an icon in the built-in video player indicating this should be possible. Reddit user u/malesca posted a console-based workaround for this issue on r/WoTShow: https://www.reddit.com/r/WoTshow/comments/r87cy6/how_to_get_prime_video_xray_content_in_fullscreen/

[link](javascript: setInterval(() => { const xx = document.querySelector("iframe[allow]"); if (!xx || xx.flurped) return; xx.allowFullscreen = true; xx.src = xx.src; xx.flurped = true }, 1000))
