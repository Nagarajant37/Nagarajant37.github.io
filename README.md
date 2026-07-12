# Nagarajan Thathasamy — Cybersecurity Portfolio

A single-file, dependency-free portfolio website for a Security Engineer / SOC & Digital Forensics
professional. Everything (HTML, CSS, JS) lives inside `index.html`, so it runs anywhere with **no
build step** — perfect for GitHub Pages.

---

## Files

- `index.html` — the entire site (open directly in a browser to preview).
- `logos/` — *(optional, you create this)* official product logos for the "Tools & Platforms" wall.
- `Nagarajan-Thathasamy-Resume.pdf` — *(you add this)* your résumé, so the download buttons work.
- `README.md` — this file.

---

## Preview locally

Double-click `index.html`, or serve it:

```bash
cd ~/cybersecurity-portfolio
python3 -m http.server 8080     # then open http://localhost:8080
```

---

## Adding the product logos  ⭐

The "Tools & Platforms" section shows a clean **brand wordmark** for each product by default.
To swap in the **official logos**, create a `logos/` folder next to `index.html` and drop in
**transparent PNG** files (SVG also works — keep the same names) using these exact filenames. Each
logo appears automatically the moment its file exists — no code changes needed.

The wall **auto-normalizes every logo** to a uniform, same-size silhouette (white on the dark theme,
dark on the light theme) so mismatched brand colours — the white CrowdStrike logo, the black Fortinet
logo, the colourful AWS logo — all look like one neat, consistent set. On hover, a logo returns to its
full original colour. So **any transparent logo works** regardless of its native colour.

| File to add | Product | You already have this logo ✓ |
|---|---|---|
| `logos/qradar.png` | IBM QRadar | ✓ |
| `logos/crowdstrike.png` | CrowdStrike Falcon | ✓ |
| `logos/cynet.png` | Cynet XDR | ✓ |
| `logos/forcepoint.png` | Forcepoint DLP | ✓ |
| `logos/fortinet.png` | Fortinet (used for both FortiSIEM &amp; FortiGate tiles) | ✓ |
| `logos/aws.png` | AWS | ✓ |
| `logos/azure.png` | Microsoft Azure | ✓ |
| `logos/nessus.png` | Tenable Nessus | ✓ |
| `logos/sentinel.png` | Azure Sentinel | reuse the Azure logo, or Microsoft Sentinel icon |
| `logos/trendmicro.png` | Trend Micro Apex | trendmicro.com brand resources |
| `logos/qualys.png` | Qualys | qualys.com brand |
| `logos/spycloud.png` | SpyCloud | spycloud.com brand |
| `logos/magnet-axiom.png` | Magnet AXIOM | magnetforensics.com brand |
| `logos/cellebrite.png` | Cellebrite | cellebrite.com brand |
| `logos/servicenow.png` | ServiceNow | servicenow.com brand |

**How to save:** use a **transparent-background PNG** (or SVG). Filenames must match exactly (lowercase).
For the two Fortinet tiles, save the single Fortinet logo as `logos/fortinet.png`. Vendor logos are
trademarks of their owners — using them to describe tools you've worked with is standard on a
résumé/portfolio; use official assets and don't alter the marks.

---

## Deploy to GitHub Pages

1. Create a **public** repo (e.g. `portfolio`) and push:

   ```bash
   cd ~/cybersecurity-portfolio
   git init && git add . && git commit -m "Add cybersecurity portfolio"
   git branch -M main
   git remote add origin https://github.com/<your-username>/portfolio.git
   git push -u origin main
   ```

2. **Settings → Pages → Build and deployment** → Source: *Deploy from a branch* → Branch: `main` / `(root)` → **Save**.
3. Live in ~1 minute at `https://<your-username>.github.io/portfolio/`.

*(For a root-domain URL, name the repo `<your-username>.github.io` instead.)*

---

## Before you publish — fill in

| Placeholder in `index.html` | Replace with |
|---|---|
| `YOUR_LINKEDIN_URL` | Your LinkedIn profile URL (appears twice: hero + contact) |
| `YOUR_GITHUB_URL` | Your GitHub profile URL |
| `Nagarajan-Thathasamy-Resume.pdf` | Add this PDF to the repo (or delete the two résumé buttons) |

Already filled in from your résumé: **name, email (nagarajan.thathasamy@gmail.com), phone (+91 63740 99735)**,
both roles (Zoho, Intellect Design Arena), certifications (SC-200, Seceon), education, and the Vuln-MS project.
Review the metrics and case-study wording and adjust anything you'd phrase differently before publishing.

---

## Notes

- Fully responsive; **light + dark themes** (auto-detects the visitor's OS preference; toggle in the header overrides).
- No external requests, no trackers — loads fast and passes strict privacy/CSP setups.
