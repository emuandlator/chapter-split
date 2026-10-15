# Chapter Split

A single web page that cuts a long PDF into one file per chapter. Everything runs in your browser, so the PDF never leaves your computer.

## Installation

There's nothing to install. Pick one:

- Use it online at https://emuandlator.github.io/chapter-split (once GitHub Pages is turned on for this repo).
- Download it: click the green Code button on this page, choose Download ZIP, unzip it, and double-click `index.html`. It opens in your web browser.

Either way it needs an internet connection the first time the page loads, to pull in the PDF libraries it uses.

## How to use it

Open the page in Chrome, Edge or Firefox, drop in a PDF, and pick how to find the chapters:

- Built-in bookmarks: uses the PDF's own table of contents. Usually the cleanest option for textbooks.
- Headings on the page: scans the top of each page for lines starting with "Chapter", "Part", "Appendix" and so on. You can change the words it looks for.
- Every so many pages: cuts at a fixed interval, for documents with no structure.
- Type the starting pages: one line per chapter, page number first, then the title (`13 Cardiac Physiology`).

The chapter list is editable, so you can fix titles and starting pages before splitting. Download the chapters one at a time or all together as a .zip.

## Limits

- Bookmarks, internal links and form fields don't carry over to the split files.
- Copy-protected (encrypted) PDFs can't be split. Printing to a new PDF first usually gets around this.
- The heading search needs real text on the page, so it won't find anything in a scan without OCR.
- The page loads pdf.js, pdf-lib and JSZip from cdnjs, so it needs an internet connection to start.
