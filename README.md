# Letters from the War

A digital archive preserving wartime correspondence from World War II. This project displays scanned handwritten letters from CPL Chester Shiver to his mother, Mrs. Mae Shiver, alongside their transcriptions.

## Project Structure

```
letters-from-the-war/
├── index.html                    # Main gallery/landing page
├── css/
│   ├── style.css                 # Core styles and gallery layout
│   └── letter.css                # Individual letter page styles
├── letters/
│   └── letter-001.html           # Individual letter pages
├── images/
│   ├── scans/
│   │   └── 100444/               # Letter folder (format: MMDDYY)
│   │       ├── 100444_1.png      # Page 1 scan
│   │       ├── 100444_2.png      # Page 2 scan
│   │       ├── 100444.docx       # OCR transcription
│   │       └── Handwritten_*.png # Original scan composite
│   └── photos/                   # Portrait and other photos
└── README.md
```

## Letter Folder Naming Convention

Letter folders use the format `MMDDYY` (e.g., `100444` = October 4, 1944):
- `100444_1.png`, `100444_2.png` - Individual page scans
- `100444.docx` - OCR transcription from Microsoft Word
- `Handwritten_*.png` - Original full scan

## Adding New Letters

1. **Create the folder** in `/images/scans/` using the date format `MMDDYY`
2. **Add page scans** as `MMDDYY_1.png`, `MMDDYY_2.png`, etc.
3. **Add the OCR file** as `MMDDYY.docx`
4. **Create the HTML file** by copying `/letters/letter-001.html`
5. **Update the letter HTML**:
   - Change the date, location, and metadata
   - Update the `pages` array in the JavaScript with the correct image paths
   - Replace the transcription text
6. **Add the letter card** to `index.html` in the gallery grid
7. **Update navigation links** in adjacent letter pages

## Design Features

- **Cinematic WW2 Aesthetic**: Deep olive drab palette with gold accents
- **Typewriter Typography**: "Special Elite" font for authentic correspondence feel
- **Film Grain Effect**: Subtle animated grain overlay for vintage atmosphere
- **Multi-page Support**: Navigate between letter pages with prev/next buttons
- **Lightbox Viewer**: Click to view full-resolution scans
- **Keyboard Navigation**: Arrow keys work in lightbox mode
- **Responsive Design**: Works on mobile devices

## Fonts Used

- **Cinzel**: Elegant serif for titles and headings
- **Special Elite**: Typewriter font for letter text and UI elements
- **Crimson Text**: Readable serif for body copy

## Development

To preview locally:
```bash
cd letters-from-the-war
python3 -m http.server 8080
# Visit http://localhost:8080
```

## Historical Context

Chester Shiver served in Europe during World War II. The letters in this archive were written from locations including Neckargartach, near Heilbronn, Germany, to his mother Mae Shiver in Bluff Springs, Florida.

---

*Austin Family Archive — Preserving History, One Letter at a Time*
