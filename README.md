# About

This Component allows you to add Youtube-Videos to your Svelte Project

The orginal Component template comes from [HERE](https://github.com/sveltejs/component-template)
The Youtube stuff comes from [HERE](https://developers.google.com/youtube/iframe_api_reference)

---

# How to use it ?

Just

```bash
npm install --save-dev @sveltecasts/svelte-youtube@0.0.5

````

And in your Source Code under Script:

```
import Youtube from "@sveltecasts/svelte-youtube";

<Youtube videoId="..." />
```


# Btw

Here is a youtube video about this component:

https://www.youtube.com/watch?v=Ank3IdQHOuE

# Changelog
0.0.5 Fixed some errors when YT-Component gets destroyed and re-initialized, the problem was that YT replaced my div with an iframe and then on the component-destroy Svelte searches for an inexistent div ¯\_(ツ)_/¯ , an other problem was that the YouTubeIframeAPIReady only get called once when the first YT-Component is used, so when we recreate a Player the 'new YT.Player' function got never called
0.0.4 Update svelte version
0.0.2 Changed descripton
0.0.1 Init
