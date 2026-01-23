# PyMuPDF Notes

- Fast local parsing via PyMuPDF (`fitz`).
- Less robust than specialized PDF parsers; table extraction is minimal.
- `page.get_text("markdown")` gives quick Markdown output.
- `page.get_text("text")` provides plain text for JSON.
- Image extraction uses `page.get_images(full=True)` and `Pixmap`.

Install:
```bash
pip install pymupdf
```

Nix note (if import fails with libstdc++ missing):
```bash
# Example: pick a gcc lib path from /nix/store/*gcc*/lib
export LD_LIBRARY_PATH=/nix/store/xc0ga87wdclrx54qjaryahkkmkmqi9qz-gcc-15.2.0-lib/lib
```
