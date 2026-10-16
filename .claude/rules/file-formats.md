# Reading and writing PDF, Word, and other formats

Team members run Claude Code on their own Windows laptops, and the tools
installed differ from machine to machine. Check what's available before
relying on it, and fall back gracefully.

## Reading

- **PDF:** use the Read tool directly. For long PDFs, read a page range
  (up to 20 pages at a time), starting with the table of contents to find
  the right pages.
- **Word (.docx):** try, in order: `pandoc "file.docx" -t plain`; Python
  with `python-docx`; or treat the .docx as a zip and pull the text out of
  `word/document.xml`. If none of those work, ask the person to save a PDF
  copy.
- **Audio (.m4a):** you can't listen to recordings. Use the matching
  transcript PDF instead.
- **EPUB:** use the per-chapter PDFs in
  `Course Files/Readings/Mastering the TOGAF Standard - Segmented/`
  instead of the .epub.

## Writing

- **Markdown** always works and is easiest to review and re-edit later.
- **Word or PDF:** use whatever is installed (pandoc, Python with
  `python-docx` or `reportlab`). If nothing suitable is available, say so,
  offer Markdown instead, or ask whether they'd like to install a tool.
  Don't build Word files by hand from raw XML unless the person agrees.
- After writing a Word or PDF file, reopen it and check the text came out
  right, including headings, tables, and special characters.
