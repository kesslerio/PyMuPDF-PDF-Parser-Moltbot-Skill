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
