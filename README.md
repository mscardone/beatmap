# BeatMap

An animated, plain-language guide to normal heart rhythm and common arrhythmias, built as a bedside teaching tool for patients.

Live site: https://projects.scottcardone.com/beatmap/

## What it does

- Animated heart showing the atria, ventricles, sinus node, AV node, bundle of His, and bundle branches, with the electrical signal travelling through the conduction system in real time.
- Live EKG tracing (lead II style) drawn from the same timing as the animation, so the P wave, QRS, and T wave line up with what the chambers are doing.
- Rhythms: normal sinus rhythm, atrial fibrillation, atrial flutter, ectopic atrial tachycardia, AVRT, AVNRT, ventricular tachycardia, and sinus rhythm with right or left bundle branch block.
- Each rhythm marks where the rogue signal starts and shows how it spreads.
- Pause and play, plus half and quarter speed for walking a patient through the conduction pathway.
- Patient education text below the animation for every rhythm: what it is, what it feels like, risk factors, and the principles of treatment.

## Files

- `index.html`: the whole app. No build step, no dependencies.
- `favicon.svg`: tab icon.
- `.nojekyll`: tells GitHub Pages to serve the files as they are.

## Editing the content

All patient text lives in `index.html` inside the `<section class="edu">` block, one `<details>` card per rhythm. The one-line "where the beat comes from" summaries shown above the EKG are in the `R` object in the script (`origin:` fields). Rhythm timing lives in the `GEN` object.

## Publishing

The site is served by GitHub Pages. Any commit to `main` updates the live page within a minute or two.

## Disclaimer

BeatMap is a simplified illustration for education and is not a diagnostic tool. It does not replace the advice of a physician.

© 2026 Cardone Medical Consulting, LLC. Code is released under the MIT License (see `LICENSE`). Text and graphics may be reused for patient education with attribution.
