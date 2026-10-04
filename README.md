# Jaysal Manchanda — Portfolio

A dark, responsive software engineering portfolio built with React, TypeScript, Vite, Tailwind CSS, Motion, and Lucide. No database, authentication, or backend is required.

## Run locally

Requires Node.js 22.12+ (validated using Node 24) and npm.

```sh
npm ci
npm run dev
```

Open the localhost URL printed by Vite (port 4173).

```sh
npm run build
npm run preview
```

The build type-checks the application and generates `dist/`.

## Change content

- `src/data/profile.ts`: name, email, LinkedIn, GitHub, resume path.
- `src/data/experience.ts`: internships, dates, responsibilities, technologies.
- `src/data/projects.ts`: projects, engineering notes, source/demo URLs.
- `src/data/skills.ts`: skill categories.
- `src/App.tsx`: section copy and reusable components.
- `src/styles.css`: palette, typography, layout, responsive rules.
- `public/Jaysal-Manchanda-Resume.docx`: original provided resume download.
- `index.html`: title, description, Open Graph and Twitter metadata.

Set GitHub and project URLs from `null` to verified HTTPS URLs to activate links. Project source/demo links appear inside Engineering notes. To switch to a PDF resume, add the PDF to `public/`, change the path in `profile.ts`, and change the DOCX label in the Resume component.


## Validation performed

- TypeScript checks and Vite production build passed.
- Rendered Chrome review at desktop width and 390px / 768px iframe viewports.
- Mobile menu open/close and section navigation checked.
- Project Engineering notes disclosure checked.
- Mobile and tablet document widths matched their viewports: no horizontal overflow.
- No application console warnings/errors observed; unrelated browser extension metadata errors were excluded.
- The live Vercel homepage, JavaScript, CSS, and resume URL returned HTTP 200. The live resume bytes match the latest supplied attachment. Earlier browser download-event verification timed out.
- CSS and Motion respect reduced-motion preferences by implementation; OS-level emulation was not available in this browser.

This is a focused manual check, not a full accessibility audit or cross-browser/device certification. No automated unit tests were added for the presentational content.



