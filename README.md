# Portfolio — Shubham Patthe

Static single-page portfolio generated from the resume PDF **“Resume from CareerZenith.pdf”** in the parent `Music` folder.

## Open locally

### Option A: open the file

Double-click `index.html`, or from this folder:

```bash
open index.html
```

Some browsers restrict `file://` for minor features; Option B avoids that.

### Option B: local HTTP server (recommended)

Python 3:

```bash
cd "/Users/shubhampatthe/Desktop/GitHub/portfolio"
python3 -m http.server 8080
```

Then visit [http://localhost:8080](http://localhost:8080).

Other tools work too (e.g. `npx serve`); this project has **no npm dependencies** by design.

## Files

| File        | Purpose                          |
| ----------- | -------------------------------- |
| `index.html` | Semantic markup, all sections   |
| `styles.css` | Layout, theme, responsive nav  |
| `script.js`  | Mobile nav + footer year        |
| `README.md`  | This file                       |

## Resume extraction note

Text was extracted with **Python `pypdf`** (`pip3 install pypdf`). Extraction succeeded for one page with full sections. The PDF header had minor spacing artifacts (“S HUBHAMP ATTHE”); the site uses **Shubham Patthe**, consistent with the IIT Kharagpur email handle.

**LinkedIn:** the site links to `https://www.linkedin.com/in/shubhampiitkgp` in `index.html`.

**BTP fraud project:** the resume mentions GitHub but not a specific repo URL; the site links to your GitHub profile — replace with the project repo when you publish it.
