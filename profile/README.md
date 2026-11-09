# txtcv

**A better `$HOME` for your CV**

txtcv is a CLI-first plaintext CV builder for software developers. Keep your CV in YAML
or JSON following the [JSON Resume schema], edit it in your favorite `$EDITOR`, and
track changes in version control.

Validate your CV offline, preview it locally, and save it as a PDF from your browser. No
account, watermark, or export limit.

## Quick start

Install with [Homebrew](https://brew.sh) on macOS or Linux:

```sh
brew install --HEAD txtcv/tap/txtcv
```

This builds the latest `main` branch from source, with Go installed as a build
dependency.

Create a sample CV, replace the placeholder details in `cv.yaml`, then validate and
preview it:

```sh
txtcv init
txtcv validate
txtcv serve
```

Prefer JSON? Use `txtcv init --format json` to create `cv.json` instead.

Open http://localhost:9090. Refresh the page after editing your CV to see changes.

## Choose a theme

Choose from `default`, `minimal`, `code`, or `creative` in your CV:

```yaml
meta:
  txtcv:
    theme: code
```

Or override it for a preview with `txtcv serve --theme creative`.

## Save as PDF

Use your browser's **Print to PDF**. The preview includes A4 print styles with margins
and page-break rules. Use 100% scale, disable browser headers and footers, and enable
background graphics to preserve colors.

PDF creation happens locally in your browser.

Explore the [CLI source and documentation](https://github.com/txtcv/txtcv) or the
[Homebrew tap](https://github.com/txtcv/homebrew-tap).

[JSON Resume schema]: https://jsonresume.org
