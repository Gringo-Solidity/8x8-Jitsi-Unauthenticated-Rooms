# 8x8 Jitsi – Unauthenticated Room Access

Proof of Concept for unauthorized access to public/internal 8x8 Jitsi rooms via predictable URLs such as `/dev`, `/marketing`, `/test123`.

## ⚠️ Summary

This report demonstrates how anyone can join certain 8x8-hosted Jitsi meetings without authentication or moderator approval, using publicly guessable URLs.

- No login or PIN required.
- No moderator presence or control.
- Room chat sometimes active and logs preserved.
- Exposed PINs for phone dial-in observed.

## 🔍 Tested URLs

- `https://jitsi.8x8.vc/test123`
- `https://8x8.vc/marketing`
- `https://8x8.vc/dev`

## 🖼️ Screenshots

See `/screenshots` for visual PoC:
- Open access to rooms
- Live chat access
- Room controls enabled
- Public dial-in PINs visible

## 📬 HackerOne Response

Marked as duplicate — original report confirmed similar vector. See `hackerone-response.md`.

## 📁 Files

- `report-details.md` — full submission text
- `hackerone-response.md` — reply from triage
- `screenshots/` — visual evidence