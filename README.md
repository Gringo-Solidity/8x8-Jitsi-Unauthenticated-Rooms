# 8x8 Jitsi – Unauthenticated Room Access

Proof of Concept for unauthorized access to public/internal 8x8 Jitsi rooms via predictable URLs such as `/dev`, `/marketing`, `/test123`.

##  Summary

This report demonstrates how anyone can join certain 8x8-hosted Jitsi meetings without authentication or moderator approval, using publicly guessable URLs.

- No login or PIN required.
- No moderator presence or control.
- Room chat sometimes active and logs preserved.
- Exposed PINs for phone dial-in observed.

##  Tested URLs

- `https://jitsi.8x8.vc/test123`
- `https://8x8.vc/marketing`
- `https://8x8.vc/dev`

##  Screenshots

See `/screenshots` for visual PoC:
- Open access to rooms
- Live chat access
- Room controls enabled
- Public dial-in PINs visible

##  HackerOne Response

Marked as duplicate — original report confirmed similar vector. See `hackerone-response.md`.

##  Files

- `report-details.md` — full submission text
- `hackerone-response.md` — reply from triage
- `screenshots/` — visual evidence

---

##  HackerOne Submission

 This vulnerability was responsibly disclosed via HackerOne.  
 Report ID: `#3242067` — submitted to **8x8 Bounty** on July 9, 2025  
 Status: **Closed as Duplicate**  
 Severity Rated: **Medium (6.7)** by the triage team  
 Private submission (not publicly visible on HackerOne)

Although marked as duplicate, this submission independently discovered and documented the issue in detail, including PoC, reproduction steps, and screenshots.

 This report demonstrates hands-on ability to:
- Discover authentication flaws via URL predictability
- Validate findings without automated tools
- Prepare formal bug bounty submissions with evidence

##  Screenshots

 Proof of unauthenticated access to public/internal rooms:

### 1. Entered "Marketing" room  
![Entered marketing](screenshots/IMG_0336%20-%20entered%20marketing.png.PNG)

### 2. Chat message sent ("Test Gringo")  
![Test Gringo chat](screenshots/IMG_0338%20-%20test%20gringo%20chat.png.PNG)

### 3. SLA claim on 8x8 public site  
![8x8 SLA claim](screenshots/IMG_0341%20-%208x8%20SLA%20claim.png.PNG)

### 4. Room controls visible without login  
![Room controls](screenshots/IMG_0342%20-%20room%20controls%20shown.png.PNG)

### 5. Disconnected screen  
![Disconnected](screenshots/IMG_0344%20-%20disconnected%20proof.png.PNG)

### 6. Public PIN exposed  
![Public PIN](screenshots/IMG_0345%20-%20public%20PIN%20visible.png.PNG)

### 7. Entered "Dev" room unauthenticated  
![Open Dev Room](screenshots/IMG_0346%20-%20open%20dev%20room.png.PNG)
