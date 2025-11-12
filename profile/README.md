# txtcv

**A developer-oriented CV builder for software engineers.**

[txtcv] makes it simple to maintain and manage your professional resume using a workflow
designed specifically for developers. Keep your CV in a JSON file following the [JSON
Resume Schema](https://jsonresume.org/), and let txtcv handle the rest.

---

## 🚀 Quick Start

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

[txtcv]: https://txtcv.com
