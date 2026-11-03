# Rushyaant Bandaru / portfolio comparisons

**Latest Royal: one transition per navigation and clearer crimson glass.** Run `npm run dev` and open the printed Local URL with `/royal.html`. The entry is now a quick introduction, verified competition results and selected projects, including this portfolio. The illustrated menu is at `/royal.html#/menu`. [GRADIENT_TRANSITIONS.md](GRADIENT_TRANSITIONS.md) records the latest connected reveal, gradient surfaces and fallback behavior. [HOME_AND_PACING.md](HOME_AND_PACING.md) records this pass and its checks. Earlier Royal, Overdrive and Cipher comparisons remain available; the default `/` still opens Overdrive. Nothing has been deployed.

## Overdrive

An exaggerated, original Persona-inspired cybersecurity portfolio, built locally in `bestVer`. Deforming cyan selection, outlined italic commands, directional paper/ink transitions and selection-driven procedural 3D replace the restrained Cipher presentation. The footer links to `cipher.html`, a frozen comparison of that earlier version. The approved `../final/` website and separate AWS-STEG app are preserved.

See MOTION.md for choreography and resource mapping; research/CPK_FINDINGS.md records actual archive evidence and its limits.

## Run locally

Use Node 24 (`nvm use` when nvm is installed). From this folder:

```sh
npm ci
npm run dev
```

For an existing installation, `npm run dev` is enough. `npm run browsers:install` is only needed for browser QA when its disposable cache is missing. Open the Local URL printed by Vite. This React version uses a development server; opening the source `index.html` directly is not supported.

```sh
npm run build
npm run preview
```

The production output is `dist/`. Relative build URLs and hash routes support static hosting under a repository subdirectory. No deployment was performed. Cloudflare Pages can use `npm run build` and output directory `dist`; GitHub Pages needs the built output rather than the source folder. Verify the selected host's settings and free-plan terms before publishing. `_headers` applies on hosts that support it; GitHub Pages does not interpret that file. The production HTML also carries a CSP meta policy.

## Explore

- Home: pointer/touch navigation, or focus a menu link and use Up/Down then Enter.
- Projects: select one of five inventory entries, read the overview, open its case study, or follow a supplied public GitHub link. ClearAuth's source remains private.
- Profile, Arsenal and The Record: biography, toolkit, ongoing preparation, experience and a downloadable plain-text profile. The download is not represented as an official résumé PDF.
- Calling Card: a preview in this tab only. Nothing is delivered, persisted or sent to a backend. Email and social links provide real contact destinations.
- Escape returns to Home, or from a case study to its overview. Native browser Back and deep-link refresh are supported.
- Settings: optional original sound, off by default, and reduced motion. Preferences are session-only. System reduced motion takes precedence.

The procedural Three.js/R3F emblem is lazy-loaded on desktop, capped at 1.5 DPR, demand-rendered and paused while the tab is hidden. Mobile, reduced-motion and unavailable-GPU paths use the original static vector emblem. Arrow buttons rotate the 3D object without requiring pointer movement. Overdrive itself uses no extracted Persona assets or fan fonts. The separate Royal entry and its copied public assets have the local-only limits documented above.

## Edit

`src/data.ts` owns verified project content, links, training, route validation and the profile download. `src/App.tsx` owns the six screens, navigation, settings, focus and the local Calling Card. `src/components/` contains original geometry, diagrams and lazy 3D. `src/index.css` contains fonts and core tokens; `src/App.css` supplies common structure; `src/Overdrive.css` is authoritative for the new visual world. `src/cipher-original/` is the frozen comparison, not the place to edit the current site. See DESIGN.md for the visual system and BUILD_NOTES.md for scope and evidence.

## Verify

```sh
npm run verify
npm run test:perf
node scripts/visual-review.mjs
node scripts/motion-review.mjs
```

See TESTING.md for coverage and limitations. The browser helper uses a private, space-free temporary cache on Linux because WebKit's upstream wrapper mishandles paths containing spaces. Re-run `npm run browsers:install` if that disposable cache is cleared. No global npm or system browser configuration is changed.

The local design resources are Taste, Impeccable, Animation Forge and img2threejs. They are authoring resources, not public runtime dependencies. Motion and R3F/Three are used; Lenis and Drei are installed but are not imported into the site. Experimental img2 vision adapters remain unselected. ASSET-LICENSES.md records provenance.

## Release limits

This is a substantial working local version, not a claim of a 100/100 finished release. Real project screenshots, a reviewed résumé PDF, representative physical-device/GPU testing and screen-reader review remain useful release work. Public source destinations are retained from the supplied portfolio; no new authenticated private-repository review was performed in this build. Keep the private CPK research archives out of deployment output.
