# Word to PDF Converter

A fully self-contained, single-file HTML tool that converts `.docx` Word documents to PDF — entirely in your browser. No internet connection required after download, no server, no data upload.

---

## Features

- Drag & drop or click to browse for `.docx` files
- Live document preview before converting
- Supports headings, paragraphs, lists, and tables
- Page size options: A4, Letter (US), Legal
- Orientation: Portrait or Landscape
- Custom output filename
- 100% offline — your file never leaves your device

---

## How to Use

1. **Download** the `index.html` file
2. **Open** it directly in any browser (double-click the file, or drag it into your browser)
3. **Drop or select** your `.docx` file
4. **Preview** your document in the panel below
5. **Choose** page size, orientation, and output filename (optional)
6. **Click** "Convert to PDF" — the PDF downloads automatically

> ⚠️ Do NOT use it inside the Claude.ai preview panel — open it as a local file for it to work correctly.

---

## Browser Compatibility

| Browser | Supported |
|---------|-----------|
| Chrome  | ✅ Yes |
| Brave   | ✅ Yes (open as local file) |
| Firefox | ✅ Yes |
| Edge    | ✅ Yes |
| Safari  | ✅ Yes |

---

## Limitations

- Only `.docx` files are supported (not `.doc`, `.odt`, or `.rtf`)
- Images inside the Word document are not embedded in the PDF
- Complex formatting (multi-column layouts, text boxes) may be simplified
- Very large documents may take a few seconds to process

---

## How It Works

All processing happens locally using two bundled libraries:

- **mammoth.js** — parses the `.docx` file and extracts structured content (headings, paragraphs, lists, tables)
- **jsPDF** — renders the extracted content directly into a PDF file

Because both libraries are inlined inside the HTML file, no internet connection is needed at runtime.

---

## File Structure

```
word-to-pdf.html   ← the entire app (HTML + CSS + JS + libraries, all in one file)
README.md          ← this file
```

---

## Privacy

- No data is sent to any server
- No analytics or tracking
- The file works fully offline once downloaded

---

## Credits

Built with [mammoth.js](https://github.com/mwilliamson/mammoth.js) and [jsPDF](https://github.com/parallax/jsPDF).
