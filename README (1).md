# Custom Cowgirl Animation — RedM / RDR2

A custom female cowgirl loop animation for RedM, using a native RDR2 `.ycd` animation dictionary.

## Preview

[Watch the animation showcase on YouTube](https://youtu.be/NEmwtDYzmDw)

## Features

- One custom female cowgirl animation.
- Loop playback support.
- Native RDR2 animation dictionary (`.ycd`).
- Designed for RM Emotes and compatible emote, pose, or animation resources.
- Intended for VORP, RSG, RedEM:RP, and standalone RedM servers.

## Animation Details

| Property | Value |
|---|---|
| Animation ID | `cowgirl` |
| Dictionary | `rm@cowgirl@f` |
| Clip | `cowgirl` |
| Duration | `7.967` seconds |
| Play mode | `loop` |
| Root motion | `false` |
| Body version | Female |

## Installation

1. Back up your existing resource before making changes.
2. Place `rm@cowgirl@f.ycd` in the `stream` folder of the resource that will stream the animation.
3. Ensure the resource is configured and started by your RedM server.
4. Add the following entry to your animation configuration, if your animation script uses this format.
5. Restart the resource/server and test the animation.

```lua
{
    id = 'cowgirl',
    label = 'Cowgirl',
    dict = 'rm@cowgirl@f',
    clip = 'cowgirl',
    category = 'Custom Animations',
    duration = 7.967,
    mode = 'loop',
    rootMotion = false,
    bodies = {
        female = 'rm@cowgirl@f'
    },
    blendIn = 2.0
},
```

**Important:** Adapt the resource path and configuration to the animation script you use. This README does not include a complete RedM resource manifest or an emote script.

## Requirements

- A RedM server running the RDR3 environment.
- The animation file included in this repository.
- An emote or animation resource that supports custom animation dictionaries.

## Compatibility

Designed for RedM and intended for use with:

- VORP
- RSG
- RedEM:RP
- Standalone setups

Compatibility may depend on your particular emote or animation resource.

## More Custom RedM Animations

Explore more custom animations for your server at **[RedMorrow — RedM Animations](https://redmorrow.com/custom-redm-animations)**.

## Permissions and Credits

Only use, modify, or redistribute these files in accordance with the creator's permissions and the applicable license. If you are not the rights holder, obtain permission before publishing or redistributing the animation.

## Disclaimer

This is a community-made animation asset. It is not affiliated with or endorsed by Rockstar Games. RedM compatibility depends on the server setup and resources in use.
