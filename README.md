# In-Betweens Art Gallery Archive — Portable Static Export

This is a self-contained browser-only export. Its images, videos, PDFs, fonts,
scripts, stylesheets, and tools use relative paths, so the folder can be hosted
at a domain root or inside a subdirectory.

## Test Locally

Do not double-click `index.html`. Start a small local web server from the folder
instead.

On macOS or Linux:

```sh
python3 -m http.server 8080
```

On Windows:

```powershell
py -m http.server 8080
```

Then open <http://localhost:8080>.

## Upload to a Server

Extract the ZIP and upload its contents to either:

- a domain or subdomain root, such as `https://archive.example.org/`; or
- a subdirectory, such as `https://example.org/art-gallery/`.

The server should serve `index.html` as its default document and use standard
MIME types for HTML, CSS, JavaScript, WebP/JPEG images, MP4 video, PDF, and
WOFF2 fonts.

The included `.nojekyll` file keeps GitHub Pages from filtering the `_next`
directory. `SOURCE-COMMIT.txt` records the source revision used for this export.
