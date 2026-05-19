# Part 107.wiki

Free, single-page study hub for the FAA Part 107 Remote Pilot Certificate.

Sky High Study is a self-contained `index.html` site with plain-language study modules, curated FAA resources, checklists, and a randomized practice quiz for people preparing for the FAA Unmanned Aircraft General - Small (UAG) knowledge test.

## Features

- 14 Part 107 knowledge modules
- Randomized practice quiz with answer explanations
- Sectional chart and airspace study notes
- Weather, METAR, TAF, AIRMET, and SIGMET review
- Registration, preflight, and exam-day checklists
- Curated official FAA resources and free study links
- Responsive mobile navigation
- Light and dark themes
- SEO metadata, FAQ content, and JSON-LD structured data
- No build step, framework, login, or paid dependency

## Live Hosting

This project is designed to work well on GitHub Pages.

To publish it:

1. Push `index.html` and `README.md` to a public GitHub repository.
2. Open the repository settings.
3. Go to **Pages**.
4. Choose the branch and folder that contain `index.html`.
5. Save and wait for GitHub Pages to publish the site.

Once published, add the final GitHub Pages URL as a canonical URL in the `<head>` of `index.html` for better SEO.

## Local Use

No install is required. Open `index.html` directly in a browser.

If you prefer a local server, run one from the project folder:

```bash
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Project Structure

```text
.
├── index.html      # Main website, styles, quiz logic, and content
└── README.md       # Project overview
```

Other PDFs, notes, and source materials may be kept in the repository for reference, but the website itself only needs `index.html`.

## Customizing

Most content lives directly inside `index.html`.

- Add quiz questions by editing the `QUESTIONS` array near the bottom of the file.
- Add resources by editing the resource directory section.
- Add or revise study modules by editing the relevant `<section>`.
- Update SEO text in the `<head>`.
- Add your live URL as a canonical link after publishing.

Example canonical tag:

```html
<link rel="canonical" href="https://YOUR-USERNAME.github.io/YOUR-REPO/" />
```

## Important Disclaimer

This project is unofficial study material. It is not affiliated with, endorsed by, or approved by the Federal Aviation Administration.

Always verify regulations, testing requirements, fees, and procedures against current FAA sources before relying on them for an actual operation or exam plan.

Useful official sources:

- [FAA Part 107](https://www.ecfr.gov/current/title-14/chapter-I/subchapter-F/part-107)
- [FAA Remote Pilot Study Guide](https://www.faa.gov/sites/faa.gov/files/regulations_policies/handbooks_manuals/aviation/airman_testing/remote_pilot_study_guide.pdf)
- [FAA Remote Pilot ACS](https://www.faa.gov/training_testing/testing/acs/media/uas_acs.pdf)
- [FAA UAG Sample Questions](https://www.faa.gov/sites/faa.gov/files/training_testing/testing/test_questions/uag_questions.pdf)

## License

Free to use, mirror, fork, and improve. Credit is appreciated.
