# Don't Be Afraid Of The Terminal — Slidev

A [Slidev](https://sli.dev) version of the workshop deck. Content is copied
verbatim from the original Claude Design HTML deck; the theme is intentionally
plain (Slidev's `default` theme) so it's easy to edit.

## Run

```bash
npm install
npm run dev      # opens at http://localhost:3030
```

## Edit

All slides live in `slides.md` — one file, separated by `---`. Images are in
`public/media/` and `public/images/`.

## Export

```bash
npm run build    # static site -> dist/
npm run export   # PDF -> slides.pdf
npm run build:artifacts
```

The published workshop site serves the built deck from
`/app-in-an-evening/slides/dist/`, so the build command includes that base path.

On pushes to `main`, GitHub Actions runs `npm run build:artifacts`, force-adds
the ignored generated outputs (`dist/` and `slides.pdf`), and commits them back
to the branch when they change. The Pages workflow uses the same command before
deploying.
