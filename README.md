# kevinkuhl.github.io

Personal site. Plain HTML/CSS, no build step: `index.html` + `assets/style.css`.

## Run locally

    python3 -m http.server 8765
    # open http://localhost:8765

## Regenerate the CV PDF

The PDF is the print version of `index.html` (see the `@media print` rules in
`assets/style.css`). With the local server running:

    "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new \
      --no-pdf-header-footer --print-to-pdf=assets/docs/kevin-kuhl-cv.pdf \
      http://127.0.0.1:8765/

Rule for content: no employer or client names — describe them by sector.
