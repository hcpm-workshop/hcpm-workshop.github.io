# HCPM Summer School 2026

Website for the **1st German-Japanese Summer School on Human-Centred Perception Modelling in XR**, 14–18 September 2026, NAIST, Ikoma, Nara, Japan.

Live at: [hcpm-workshop.github.io](https://hcpm-workshop.github.io)

---

## Structure

```
index.html              ← the entire website (single file)
images/
  organisers/           ← organiser portrait photos
    alexander-marquardt.png
    biying-fu.png
    dirk-voelz.png
    isidro-butaslac.png
    martin-weier.jpg
    monica-perusquia.jpg
    taishi-sawabe.jpg
```

No build step, no framework, no dependencies. GitHub Pages serves `index.html` directly from the `main` branch root.

---

## Editing content

All content lives in `index.html`. Open it in any text editor.

The top of the file has three configuration lines:

```html
<script>window.EVENT_DATE  = "2026-09-14T09:00:00";</script>
<script>window.CONTACT_URL = "mailto:marquardt@ieee.org?subject=HCPM%20Summer%20School%202026";</script>
```

`EVENT_DATE` drives the live countdown in the hero. `CONTACT_URL` sets where the contact button points.

All other content (schedule, bios, lecture topics, venue details) is plain HTML further down in the file — search for the section comment (e.g. `<!-- ── 05 ORGANISERS`) to find what you need.

---

## Updating organiser photos

Photos must be placed in `images/organisers/` and referenced in `index.html` as:

```html
<img class="org-photo" src="images/organisers/firstname-lastname.jpg" alt="Full Name" />
```

Recommended size: at least 200 × 200 px, square crop. The site displays them at 76 × 76 px in a circle.

---

## Deployment

The site deploys automatically when changes are pushed to `main`.

GitHub Pages settings: **Settings → Pages → Source: Deploy from a branch → main → / (root)**

No workflow file is needed. Changes are live within about one minute of pushing.

---

## Organisers

Jointly organised by:

- **CARE Lab** and **IMD Lab** — Nara Institute of Science and Technology (NAIST), Japan
- **LAVIS Lab** — Hochschule RheinMain (HSRM), Germany

Contact: [marquardt@ieee.org](mailto:marquardt@ieee.org)
