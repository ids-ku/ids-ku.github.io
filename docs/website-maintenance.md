# Maintaining the IDS Lab website

The site is built with Jekyll and GitHub Pages. The target production source is the `master` branch of `ids-ku/ids-ku.github.io`.

## Address migration

This branch prepares the site for `https://ids-ku.github.io/`. Publish and verify the destination site before replacing the old `https://byungjincho.github.io/` site with redirects. Preserve paths, query strings, and anchors when redirecting. The GitHub organization and repository must be created before deployment; their availability is confirmed by GitHub during creation.

## Main files

| Content | File |
| --- | --- |
| Home introduction and research overview | `_pages/about.md` |
| Research descriptions | `_pages/research.md` |
| News, newest first | `_data/news.yml` |
| People | `_pages/people.md` |
| Publications | `_pages/publications.md` |
| Teaching | `_pages/teaching.html` |
| Talks and professional service | `_pages/talks.html` |
| Contact details and map | `_pages/contact.md` |
| Main navigation | `_data/navigation.yml` |
| Shared layout and metadata | `_layouts/lab.html`, `_config.yml` |
| Typography and responsive styling | `assets/css/lab.css` |

Recruitment appears only in the homepage Join IDS Lab strip. People lists the lab members and keeps the PI's Google Scholar and ORCID links; Publications starts directly with the publication list.

## Adding news

Add an entry at the top of `_data/news.yml`. The homepage shows the latest six entries from the complete chronological list; its All news link opens the complete archive at `/news/`. Both use the same data, without a separate featured selection.

```yaml
- date_label: "Oct. 2026"
  text: "A confirmed update written in Markdown."
  link: /research/
  link_label: Read more
```

Use a confirmed month and year for each news entry. Do not infer an acceptance date from a publication date. An optional `source` URL records the evidence for a news item without displaying it as another link.

Seonghyeon Kim’s capstone Excellence Award (최우수상) is confirmed by the lab PI; the supplied poster and the official KU Sejong SW initiative notice verify the event name and May 27, 2026 date. “Spring 2026 Industry-Linked Capstone Design Competition” and “Excellence Award” are descriptive English translations; the Korean award tier is retained for precision. His name uses the romanization “Seonghyeon Kim.”

The student air-combat competition participation and finalist milestone are confirmed by the lab PI; organizer sources verify the event name and schedule (qualifiers: August 27–28; finals: September 17, 2026). The news keeps one announcement for this competition: advancement to the finals in September 2026. Student profile keywords describe reinforcement learning and decision-making in air-combat simulation, without implying real-aircraft deployment.

Publication months for the symbiotic and multi-UAV news are IEEE's Date of Publication (September 8 and April 22, 2026). Aeacus news refers explicitly to its July 2025 journal issue, rather than its February online publication. Do not substitute DOI deposit or indexing dates for publication dates.

## Publication records

Keep published papers separate from work in progress and proposals. Verify bibliographic changes against a publisher or institutional record. The 2025 TMC and TIV records and three older bibliographic entries were updated from Aalto University's publication database. The news entries retain source URLs. AcademicPages demonstration posts, example CV, and other sample pages are excluded from publishing in `_config.yml`; their source remains in git.

## Research scope and recent papers

The introduction explicitly names three application domains: communication networks, edge computing and AI systems, and quantum information systems. The three research themes describe questions across these domains, not mutually exclusive paper categories. Symbiotic radio/ISAC and UAV data collection sit primarily in communication networks; air-ground computing offloading and CORAL sit primarily in edge computing and AI systems. UAV is a platform that can appear in either domain.

The 2026 CORAL, secure symbiotic radio, multi-UAV data collection, and air-ground offloading entries were checked against IEEE-deposited Crossref records at `https://api.crossref.org/works/{DOI}`. These are published records; the CORAL preprint is linked as an alternate version rather than a duplicate publication. Relevant primary records:

- Symbiotic radio: https://tiedejatutkimus.fi/fi/results/publication/0710449126
- CORAL program: https://icfec2026.hanyang.ac.kr/
- CORAL manuscript: https://arxiv.org/abs/2603.14577

Research descriptions link to stable publication anchors. Keep the anchors when editing or reordering entries. Experimental improvements in CORAL are not presented as mathematical guarantees. Carbon-aware edge fleet work is described as a research direction rather than a published result.

## Design assets

The homepage uses `assets/images/nds-research-hero.webp`, a decorative conceptual illustration, not a photograph of a campus or a scientific diagram. Its generation prompt is recorded in `docs/hero-image-prompt.txt`.

Source Sans 3 and Source Serif 4 are self-hosted as Latin-subset variable WOFF2 fonts. The text-only IDS badge uses white Source Sans 3 text with 0.12em letter spacing on a black rectangle, aligned to the left edge of “Information & Decision Systems Lab.” below it. The homepage moves directly from the banner to the introduction and News columns, with no separate central lab-name heading. Site typography, navigation, links, dates, research numbers, and the recruitment rule share the same black color. Body paragraphs, news text, publication and other list entries, and contact descriptions use justified text on desktop and mobile. Paragraph endings and explicit line breaks remain left aligned; headings, navigation, and dates keep their existing alignment. Automatic hyphenation and emergency long-word wrapping keep the text within its column.

The shared type scale uses 29px page titles, 20px section headings, 16px body text, and 14px small text. The header subtitle is 13px. News entries, dates, and inline links use a separate 13px size on desktop and mobile; the News heading and All news link follow the standard heading and small-text sizes.

The SIL Open Font Licenses are stored alongside the fonts in `assets/fonts/`. The page uses no external font service.

## Preview and deployment

With Ruby and Bundler installed, run `bundle install`, then `bundle exec jekyll serve`. Check the homepage and navigation at desktop and mobile widths. Pushing to the GitHub Pages source branch triggers the repository's Pages build.
