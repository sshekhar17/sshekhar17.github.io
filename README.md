# Personal website

A static HTML website. No build step is required.

## Layout

- `index.html`: home page.
- `demos/index.html`: demo listing; interactive demo pages live alongside it.
- `blog/index.html`: blog listing. Add future posts as `blog/post-slug/index.html` and link them from this listing.
- `files/`: downloadable documents, including tutorial PDFs.
- `assets/`: shared images, audio, CSS, and JavaScript as needed.
- `ITW2026tutorial.html`: tutorial landing page, kept at its existing URL.

The root demo HTML files and `Demos.html` are compatibility redirects for previously shared URLs. Edit the actual demos in `demos/`.

Tutorial PDFs now live at `files/tutorial.pdf` and `files/tutorial-part2.pdf`; old direct PDF URLs need to be updated wherever they were shared.

The demos optionally load `assets/audio/beethoven_symphony5_movement1.ogg` and `assets/audio/joplin_the_entertainer.mp3`. These recordings are not included; the demos fall back to their existing Wikimedia URLs.

Use relative links so the site works when served from a subdirectory. A post at `blog/post-slug/index.html`, for example, links home with `../../index.html` and to shared assets with `../../assets/`.

## Local preview

Run `python3 -m http.server 8000` from this directory, then visit <http://localhost:8000>.
