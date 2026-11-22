# The Byrdes — A Living Christmas Card

A Christmas card where each photo comes to life. Scan the QR code on the
card, point your phone camera at any photo, and that photo's scene plays
over it. One page, one QR code, five photos, five videos.

## How it works

- **Image tracking:** [MindAR](https://hiukim.github.io/mind-ar-js-doc/)
  (open-source, runs in the phone browser — no app needed). The printed
  photos are the "targets"; the page matches what the camera sees against
  them and pins each video to its photo.
- **One URL, five targets:** a single compiled target file (`targets.mind`)
  holds all five photos, each mapped to its own video.
- **Clips:** short scenes from Netflix's *Ozark* featuring the Byrde
  family (Marty, Wendy, Charlotte, Jonah). Personal, non-commercial
  Christmas card — not for distribution.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The AR page. Open it on your phone, tap Start, point at a photo. |
| `targets.mind.b64.part1` + `.part2` | Compiled MindAR image targets (the 5 card photos), base64 text in two parts. The page joins and decodes them in the browser. |
| `videos/*.mp4.b64` | The five clips, ~9–15 s each, 16:9 landscape, base64 text. The page decodes each one in the browser. |
| `images/` | The five printed card photos (frames from the clips). |
| `qr.png` / `qr.svg` | QR code linking to this page. |
| `card.pdf` | Printable letter-size card: 5 photos + QR code. Print on card stock, matte finish works best for tracking. |

## The five scenes

1. **Marty and the bank** — Marty demands his $7.9 million in cash. (15 s)
2. **Couples therapy** — Marty and Wendy both try to bribe the therapist. (9 s)
3. **Jonah's new business** — Jonah starts laundering money. (12 s)
4. **Ben has questions** — Ben tells Marty he talked to Helen's kid. (13 s)
5. **Breakfast at the lake house** — Charlotte confronts her parents, then the dock. (12 s)

## Tips

- Print matte, not glossy — glare hurts tracking.
- Give the card good light when scanning.
- Point at one photo at a time; its video plays and loops while tracked.
- If a photo won't catch, move the phone a little closer and hold steady.

## Live page

https://thejohnnyconnor.github.io/kindle-paper/ar-christmas-card/
