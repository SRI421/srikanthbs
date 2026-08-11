# Gap Analysis — Portfolio & Resume (August 2026)

A review of sri421.github.io/srikanthbs and your resume against what impresses recruiters and passes ATS screening, for Senior Software Engineer / AI Engineer / Backend Engineer targets.

---

## 1. Gaps found and FIXED in this round

### Portfolio

| Gap | Why it mattered | Fix applied |
|---|---|---|
| Project cards showed only emoji | Zero technical signal at first glance — recruiters scan projects in seconds | All 6 projects now open with a **data-flow diagram** (same style as the flagship architecture diagrams) |
| No resume access from the hero | Recruiters won't scroll to the footer to find your resume | **Download Resume** button added to the hero CTA row |
| GitHub missing from the Contact grid | The one link tech recruiters always click | GitHub card added (github.com/SRI421) |
| No `og:image` / canonical URL | Links shared on LinkedIn/WhatsApp showed a bare text preview | Branded **og_banner.png** (1200×630) + `og:url`, `twitter:card`, canonical tag |
| Contact form used Netlify on GitHub Pages | The form **silently did nothing** when submitted — lost leads | Rewired to open the visitor's email app with the message pre-filled (works on GitHub Pages, no service needed) |
| "5 Years Experience" | Your own timeline starts Sep 2019 → that's 6+ years; underselling | Hero stat and Experience subtitle now say **6+** |
| Layout shift while diagrams lazy-load | Janky scroll on slow connections | Aspect-ratio reserved for diagram slots |

### Resume

| Gap | Why it mattered | Fix applied |
|---|---|---|
| "Technical Expertise" header | ATS parsers reliably detect the standard header "Skills" | Renamed to **TECHNICAL SKILLS** |
| No compact keyword block | ATS keyword-matches against the JD; scattered keywords score lower | New **Core Competencies** line under the summary (LLM Automation & Generative AI, RAG, Intent Classification, Temporal, pgvector, Microservices, Cloud, Full Stack, Leadership) |
| Target job titles absent | Matching the JD's title lifts ranking | Summary now names **Senior Software Engineer / AI Engineer / Backend Engineer** roles |
| "Machine Learning" never spelled out | Only "AI/ML" appeared — misses exact-phrase matches | Skills now say **Machine Learning (TensorFlow, PyTorch, Scikit-learn)** |
| Dot separators in skills lists | Some parsers tokenize commas more reliably than "·" | Skills section separators switched to commas |
| "5+ years" | Same undersell as the site | Now **6+ years** |

### ATS audit — current state (verified by machine-extracting the PDF text)

Single column, no tables/text-boxes/images in the parse path, standard Calibri, standard section headers (Professional Summary / Professional Experience / Technical Skills / Education / Certifications), parseable date ranges, contact + LinkedIn + GitHub + portfolio in plain text, 2 pages, and every key term extracts cleanly: LLM, RAG, Generative AI, Machine Learning, Temporal, pgvector, Gemini, Python, React, PostgreSQL, Microservices, Docker, Kubernetes, Azure, AWS, CI/CD. The DOCX also passes OOXML schema validation, so ATS portals that parse Word files read it identically.

---

## 2. Remaining gaps — only you can close these (ranked by impact)

1. **Real numbers for the two flagship platforms.** This is the single biggest upgrade available. Wherever you can, measure and send me: tickets/messages analyzed, distinct intents discovered, classification accuracy or agreement rate, % faster first-response using templates, docs synced, sync latency, Ask Wiki questions answered per week / deflection rate. I left the copy metric-free rather than fake — one round of real numbers makes both site and resume dramatically stronger.
2. **Public proof for the flagships.** Recruiters click GitHub and find mostly old repos. Even if the code is proprietary: create a public "architecture + write-up" repo per project (README with these same diagrams, the problem, your design decisions), or record a 2-minute demo walkthrough. Pin both repos (plus FlowForge) on your GitHub profile, and add a profile README.
3. **The `SRI421.github.io` placeholder site.** Anyone visiting `sri421.github.io` (without `/srikanthbs`) sees "aa" placeholders — that's the first impression for the root URL. Either make it redirect to `/srikanthbs`, or replace it with this new site.
4. **LinkedIn mirror.** Same headline ("AI Automation Engineer · Python Backend · LLM & RAG Systems"), both flagship projects in the Featured section (the diagrams work great as media), og_banner.png as your banner image, and 2–3 recommendations from Perfecter.ai colleagues.
5. **Tailor per application.** Keep `Srikanth_BS_Resume.docx` as the master; for each JD, swap 3–5 terms in the Core Competencies line to mirror the posting's exact words (e.g., "Vector Databases" vs "Semantic Search", "GCP" if asked). Exact-phrase matches are how you go from good to top-ranked in ATS.
6. **A current certification.** Your listed certs are early-career. One 2026-relevant cert — Azure Solutions Architect (AZ-305), Azure Developer (AZ-204), or a recognized GenAI/ML engineering cert — reinforces the AI-architecture positioning.
7. **Write the story once.** A short case-study post per flagship (LinkedIn article or dev.to) — problem → architecture → what broke → results. Recruiters and hiring managers read these; they also give your name search results beyond GitHub.
8. **Consistency check on contact email.** gmail is fine; just use the same email everywhere (site, resume, LinkedIn, GitHub) so profile-matching tools connect them.

---

## 3. Suggested 7-day plan

Day 1–2: fix root GitHub Pages site + pin repos + profile README. Day 3: LinkedIn headline, Featured section, banner. Day 4–5: gather flagship metrics, send them to me → I update site + resume in minutes. Day 6: publish first case-study post. Day 7: pick 5 target JDs and tailor the competencies line for each.

*Everything in section 1 is already live in your files — commit and push the `srikanthbs` folder to deploy.*
