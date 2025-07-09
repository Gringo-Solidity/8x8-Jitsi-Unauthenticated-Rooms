# Vulnerability: Unauthenticated access to Jitsi meetings via predictable URLs on `jitsi.8x8.vc` and `8x8.vc`

## Summary

Certain Jitsi rooms hosted on 8x8’s domain are accessible to any external user without requiring login, moderator approval, or PIN — as long as the room name is known or guessable.

## Proof of Concept (PoC)

Tested rooms:
- https://jitsi.8x8.vc/test123
- https://8x8.vc/dev
- https://8x8.vc/marketing

Observed behavior:
- Unauthenticated access to room with video/audio/chat capability
- No CAPTCHA or moderator confirmation
- Chat history visible in some rooms
- In some cases, dial-in PINs were displayed on screen (`6968`, `3821`, etc.)

## Supporting Material

See attached screenshots (mobile):
- `IMG_0336 – Entered /marketing room`
- `IMG_0342 – Room controls visible`
- `IMG_0345 – Public PIN visible`
- `IMG_0344 – Disconnected proof`
- `IMG_0346 – Open /dev room`

## Impact

- Unauthorized access to internal or private meetings
- Exposure of chat logs and PINs
- Lack of compliance with enterprise security expectations