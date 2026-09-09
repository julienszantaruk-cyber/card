# UTTOP international delegation card site

This is the **same GitHub repository** as the existing card: upload these files into the same `card/` folder (replace the former personal `index.html` with the team hub). It is pure static HTML/CSS/vanilla JS: no CDN, external script, build step or network dependency.

## File list

HTML: `index.html`, `julien.html`, `fabien.html`, `karen.html`, `noemie.html`, `qr.html`, `julien-qr.html`, `fabien-qr.html`, `karen-qr.html`, `noemie-qr.html`.

User-supplied images to upload into this folder: `photo.jpg`, `fabien.jpg`, `karen.jpg`, `noemie.jpg`, `qr.png`, `julien-qr.png`, `fabien-qr.png`, `karen-qr.png`, `noemie-qr.png`.

## QR destinations

- `qr.png` must encode `https://www.uttop.fr/en/card/index.html` (the team hub).
- `julien-qr.png` must encode `https://www.uttop.fr/en/card/julien.html`.
- `fabien-qr.png` must encode `https://www.uttop.fr/en/card/fabien.html`.
- `karen-qr.png` must encode `https://www.uttop.fr/en/card/karen.html`.
- `noemie-qr.png` must encode `https://www.uttop.fr/en/card/noemie.html`.

The existing `qr.png` already targeting `/card/index.html` is therefore correct for the new team page. Regenerate Julien's personal QR to point to `julien.html`.

## Important

Filenames are lowercase/case-sensitive on GitHub Pages/Linux. Keep every filename exactly as written, including `noemie.jpg` and `julien-qr.png`.

## Test checklist

1. Upload all HTML files and the nine image files to the same `card/` directory.
2. Open `index.html` and test each member row, shared email, UTTOP link and team QR link.
3. On each personal card, test vCard download, email, LinkedIn, UTTOP International and share/clipboard fallback.
4. Open each QR page and scan each QR code from a second device.
5. Test on a narrow mobile viewport, dark mode, offline, and print preview.
6. Confirm all profile photos load; if one is absent, the card shows initials as a fallback.
