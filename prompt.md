# Schedule Section — Generation Prompt

Prompt used to generate the "Schedule" section of the DevConf 2026 landing page.

---

Add a "Schedule" section to a developer-conference landing page (DevConf 2026). It's the natural next section because the nav links to Schedule but the page doesn't have one yet.

The page uses Inter throughout on a white background, with these tokens: blue accent `#2563EB`, dark navy `#0D1B2A` for emphasis, grey `#575757` for secondary text, 12px card radius, 1px `#E5E7EB` borders. There are existing shared utility classes: `.section-title` (56px bold dark heading) and `.text-center`. Reuse them so the heading matches the other sections exactly.

Structure: a centered 56px heading, a centered grey subtitle beneath it, then a vertical list of 5 time-ordered talk rows with a 16px gap. Each row is a horizontal flexbox with three parts — a bold start time on the left in a fixed 70px column so all times align vertically, the talk title (bold) and speaker/room line (grey) in the middle taking the remaining space, and a track label on the right. Rows are plain white cards: white background, 1px `#E5E7EB` border, 12px radius, 24px/32px padding.

The track label is a rounded pill (border-radius 999px, uppercase, 12px semibold). Give each of the five tracks its own soft color, applied via a `track-*` class on the row that colors the pill: a pale tinted background with the strong hue as text. Tracks and colors:

- AI / ML — indigo (`#EEF2FF` bg / `#4F46E5` text)
- Cloud & DevOps — cyan (`#ECFEFF` / `#0891B2`)
- Frontend — pink (`#FDF2F8` / `#DB2777`)
- Security — orange (`#FFF7ED` / `#EA580C`)
- Panel — green (`#F0FDF4` / `#16A34A`)

Keep the rest of the row neutral so only the pill carries color — subtle, not loud.

Write realistic but fictional talk titles and a witty one-line subtitle — no lorem ipsum, no real people or companies. Give me semantic HTML and vanilla CSS separately: Flexbox only, no frameworks, no CSS variables, kebab-case class names, with an Emmet abbreviation comment above the repeated row block.
