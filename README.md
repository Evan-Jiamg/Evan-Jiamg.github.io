# evan-jiamg.github.io

Personal academic homepage of Ming-Zhi (Evan) Jiang, built with [AcademicPages](https://github.com/academicpages/academicpages.github.io) (Jekyll).

## Where things live

| What | File |
|---|---|
| Home page (bio, recent research, news) | `_pages/about.md` |
| Research | `_pages/research.md` |
| CV (web version) | `_pages/cv.md` |
| Honors + certificates | `_pages/honors.md`, `images/awards/` |
| Memorable Moments (Nepal photos) | `_pages/moments.md`, `images/nepal/` |
| Publications (one file per paper) | `_publications/` |
| Resume PDF | `files/Ming-Zhi_Jiang_Resume.pdf` |
| Sidebar (name, photo, links) | `_config.yml` → `author:` |
| Top menu | `_data/navigation.yml` |
| Custom styles | `_sass/layout/_custom.scss` |

## Add a news item
Add one `<li>` line at the top of the `news-list` in `_pages/about.md`.

## Add a paper
Copy a file in `_publications/`, change the date, title, venue and excerpt.

## Deploy
Push to the `main` branch of `Evan-Jiamg/Evan-Jiamg.github.io`; GitHub Pages builds it automatically.
