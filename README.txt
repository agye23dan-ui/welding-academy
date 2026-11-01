Welding & Fabrication Academy (PWA)

HOW TO DEPLOY
1. Upload ALL files in this folder (not _legacy) to any HTTPS host (GitHub Pages, Cloudflare Pages, Netlify).
2. Open index.html on that site. On a phone use "Add to Home screen". After the first visit it works offline.

FILES
index.html      app shell
academy.js      shared engine (routes, dashboard, quizzes, exams, calculators, job sheets, C&G centre). Same file as plumbing-academy.
config.js       this app's settings: name, module groups, exams, calculators, job sheets, C&G units
data.js         course content: modules (notes, figures, questions) and glossary
hero.js         photographic hero scenes and textures
cgdata.js       City & Guilds practice banks (units 201, 202 multiple choice; 212 short answer)
manifest.json, icon.svg, sw.js    install and offline support
_legacy/        the previous version of the app, kept for reference (do not deploy)

UPDATING: when you change any file, change the cache name in sw.js (weld-vN -> weld-vN+1, currently weld-v20).
If you add a file, add it to index.html and the list in sw.js.
Progress is stored in the browser (localStorage); learners can export and import it from the Modules page.
Progress from the previous version carries over as module passes (70%).

STANDARDS
Aligned to City & Guilds 2850 Level 2 (units 201, 202, 212) and general welding practice. Not accredited by any awarding body. Practice questions are original, not real C&G papers. Check current local rules and your equipment maker's data before relying on any figure.
