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

## Content provenance and remaining input

Primary source: JaysalManchanda_Resume2027 (1).docx, supplied October 3, 2026. LinkedIn was recovered from its embedded hyperlink. Education uses the resume's 2024–2028 dates.

The Task Manager description and its additional technologies come from the user's previously shared project background. It has not been independently audited against a source repository. Project visuals are labeled architecture and conceptual treatments; they are not fabricated application screenshots.

Outstanding inputs:
1. GitHub profile URL.
2. Actual repository URLs and optional live demo URLs for each project.
3. Optional real project screenshots and a finalized PDF resume.

The site does not repeat the resume's percentage improvement claims. The downloadable supplied resume is unchanged and still contains its original quantitative claims. Review it before broadly sharing the portfolio.

## Deploy to Vercel

`vercel.json` provides the Vite framework, `npm run build` command, and `dist` output directory. No environment variables are required.

Create a NEW GitHub repository named `jaysal-portfolio` if that name is available, push this source, and import it as a new Vercel project. Do not overwrite an existing repository or project. Alternatively, use the official Vercel CLI from this directory after authenticating:

```sh
npx vercel
npx vercel --prod
```

Once a production URL exists, add its canonical URL and `og:url` to `index.html`. No deployment URL is invented in this version. Public resume downloads expose the original resume's email and phone number, as requested; replace the file if you prefer a public-specific version.

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

## Design references

Research references: https://brittanychiang.com/ and https://raunofreiberg.com/ — emphasis on readable project narratives and restrained interaction. This portfolio uses an original editorial layout; no reference site's code or assets were copied.

## Delivery status

The updated project passes its TypeScript and production build checks. Vercel CLI created a READY temporary deployment at https://temporary-rapid-tin-4hkfl3s.vercel.app on October 3, 2026 (Pacific time). This anonymous deployment expires about one hour after creation unless claimed; the private claim link was supplied in the conversation, not committed here. After claiming, verify the permanent domain in your Vercel account.

GitHub publishing remains pending: its provider actions were not exposed to this execution session. No remote repository was created. Project and GitHub URLs remain for owner confirmation. PwC dates and responsibilities have been updated from the latest supplied resume.
