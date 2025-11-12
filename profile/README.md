# txtcv

**A better `$HOME` for your CV**

Keep your CV in plain text in your favorite `$EDITOR` and let txtcv handle the rest.
Finally, a CV workflow that makes sense for developers.

[txtcv] lets you manage your CV as code. Store your CV in JSON following the [JSON
Resume schema], put it in version control, and publish to txtcv with CLI or Github
Actions.

## Quick Start

### Web Interface

1. Sign in to [txtcv.com](https://txtcv.com) using your GitHub account
2. Create a new CV and copy/paste your JSON resume
3. Choose from multiple professional templates
4. Share your CV with a unique link

### CLI Tool

Install the CLI via Homebrew and manage your CV locally:

```bash
$ brew install txtcv/tap/txtcv
$ txtcv auth login
$ txtcv publish --id <cv-id> cv.json
```

### GitHub Actions

Automatically publish your CV on every push:

```yaml
- uses: txtcv/actions-publich@v1
  with:
    cv_id: your-cv-id
    cv_path: cv.json
    txtcv_auth_token: ${{ secrets.TXTCV_AUTH_TOKEN }}
```

[JSON Resume schema]: https://jsonresume.org
[txtcv]: https://txtcv.com
