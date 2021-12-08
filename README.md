# fullscreenxray
## Enable fullscreen mode for x-ray bonus content (such as for Wheel of Time episodes) on Amazon Prime
Huge hat-tip to reddit user [u/malesca](https://www.reddit.com/user/malesca) who [shared this workaround](https://www.reddit.com/r/WoTshow/comments/r87cy6/how_to_get_prime_video_xray_content_in_fullscreen/). This post is for those who want an even quicker way to apply it.

If you pause a video on Amazon Prime, you can access bonus content for that video by clicking "x-ray" in the upper left corner. Videos in this section can be impossible to play in fullscreen, despite an icon in the built-in video player indicating this should be possible. Reddit user [u/malesca](https://www.reddit.com/user/malesca) posted a javascript-based workaround that can be applied through the built-in javascript console.

Here's how you can create a bookmarklet you can keep in your bookmarks toolbar that lets you apply this workaround whenever you like with a single click:

Right-click on your bookmarks toolbar, and click "add page".

Choose a name for your bookmarklet (eg. "Fullscreen X-Ray").

Copy and paste the following code into the bookmark URL field:

```javascript
javascript:void(location.href='javascript:setInterval(() => { const xx = document.querySelector("iframe[allow]"); if (!xx || xx.flurped) return; xx.allowFullscreen = true; xx.src = xx.src; xx.flurped = true }, 1000)')
```

Now open a video on Prime (such as an episode of Wheel of Time), pause, click X-Ray in the upper left corner, click "bonus content", click your new bookmarklet in the bookmarks bar, start playing one of the videos, and click the fullscreen mode icon in the small video player's upper right corner.

I had to change the original code a little in order to get it to work in Chrome as a bookmarklet. I'm sure someone can simplify it (let me know in that case).

Hopefully this solution will keep working until the folks at Prime fix this bug. The bonus content is often really neat, and it's a shame they haven't made it easier to enjoy.
