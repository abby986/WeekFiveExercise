# Customer Reviews Feature — Build Plan

Interactive star rating + written review form with a testimonial slider/carousel.
Each step is designed to be reviewable and testable in 5–10 minutes.

---

## Step 1 — Reviews section skeleton (HTML only)
Add a new `<section>` to `index.html` with a heading and empty placeholder divs
for the carousel and form. No styling or JS yet.

**Test:** Section appears in the page flow.

---

## Step 2 — Style the section shell
Add CSS for the section background, heading, and layout container using the
existing design tokens (`--cream`, `--red`, Palatino font, etc.).

**Test:** Section looks on-brand and fits the page.

---

## Step 3 — Build a single testimonial card (HTML + CSS)
Create the HTML for one hardcoded review card: star display (e.g. `★★★★☆`),
quote text, and reviewer name. Style it with a white card, shadow, and serif
typography.

**Test:** One card renders correctly.

---

## Step 4 — Carousel structure and CSS
Duplicate the card into 3–4 hardcoded samples. Wrap them in a sliding track,
add prev/next arrow buttons, and use CSS (`overflow: hidden` + `transform: translateX`)
to show only one card at a time.

**Test:** Only one card is visible; buttons appear correctly.

---

## Step 5 — Carousel navigation JavaScript
Wire up the prev/next buttons to shift the track by the card width.

**Test:** Clicking arrows cycles through the hardcoded reviews.

---

## Step 6 — Auto-play with pause on hover
Add a `setInterval` to advance the carousel automatically. Pause on
`mouseenter`, resume on `mouseleave`.

**Test:** Carousel advances on its own and pauses when hovered.

---

## Step 7 — Review submission form (HTML + CSS)
Add a form below the carousel with fields for name, review text, and a row of
5 clickable star icons. Style it to match the existing contact form.

**Test:** Form is visible, styled, and stars are clickable (no logic yet).

---

## Step 8 — Interactive star rating JavaScript
On star hover: highlight stars up to the hovered one. On star click: lock in
the selection and store the rating value.

**Test:** Hover and click behavior works visually.

---

## Step 9 — Form submission logic
On submit: validate required fields, dynamically build a new card from the form
data, inject it into the carousel track, reset the form, and show a brief
success message.

**Test:** Submitting a review adds it to the slider.

---

## Step 10 — Mobile polish and final CSS
Add responsive styles so the carousel and form look correct at tablet (`768px`)
and phone (`480px`) breakpoints, matching the existing media query structure.

**Test:** No layout breaks at small screen sizes.

---

## Summary

| Steps | Focus |
|-------|-------|
| 1–2   | Section structure and styling |
| 3–4   | Testimonial card and carousel layout |
| 5–6   | Carousel interactivity and auto-play |
| 7–8   | Review form and star rating widget |
| 9     | Form submission wired to carousel |
| 10    | Responsive / mobile polish |
