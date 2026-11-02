# PharmaTools guide — instructions for editors and agents

## About this project

- The PharmaTools user guide, built on [Mintlify](https://mintlify.com). Readers are pharmacists,
  technicians, assistants and pharmacy owners in Ontario, Canada, plus PharmaTools partners.
- Pages are MDX files with YAML frontmatter (`title`, `description`, `icon` from lucide).
- Configuration and navigation live in `docs.json`: one dropdown per module, groups inside.
- One folder per module (`getting-started/`, `settings/`, `communications/`, `rxlink/`, `campaigns/`,
  `rx-texts/`, `todo/`, `forms/`, `compounding/`, `narcotics/`, `blister-packs/`, `central-fill/`,
  `desktop/`, `partner-portal/`); images in `images/<same folder>/` as `.webp`.
- Preview with `npx mint dev`; check links with `npx mint broken-links`; check the build with `npx mint validate`.
- When a page moves, add a `redirects` entry in `docs.json` for its old address.

## Screenshots

- Screenshots come from the real PharmaTools app, never mock-ups.
- Replace test data before capturing: the sample pharmacy is "Maple Street Pharmacy" (other modules use
  "Riverside Pharmacy"); no real people's names, phone numbers or emails.
- Use `<Frame caption="...">![alt](/images/<folder>/<name>.webp)</Frame>`, and write alt text that says what the screen shows.

## Style

- Second person, active voice, sentence-case headings, one idea per sentence.
- Bold UI labels exactly as the app spells them: click **Send fax**. Name places as a path: **Comms › eFax**.
- No vague wording: never "Needs you", "On its way", "All good", "Action needed", "on the page", "here",
  "elsewhere". Say the exact state, the exact screen, and who sees it (pharmacy staff, patient, prescriber,
  partner pharmacy, fax recipient).
- Every example date includes the year.

## Content boundaries

- Never name pharmacy software vendors — say "your pharmacy software".
- Never name compounding suppliers or branded bases — say "supplier catalogues" and "cream base".
  Health Canada DPD and LNHPD may be named. Ask before naming any other third-party company.
- Never write "No credit card required". The trial is a "30-day free trial".
- Don't document the PharmaTools internal admin portal, stub screens or code internals.
