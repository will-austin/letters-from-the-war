# Letters from the War

A digital archive preserving wartime correspondence from World War II. This project displays scanned handwritten letters alongside their transcriptions, creating a personal window into history.

## Project Structure

```
letters-from-the-war/
├── index.html              # Main gallery/landing page
├── css/
│   ├── style.css           # Core styles and gallery layout
│   └── letter.css          # Individual letter page styles
├── letters/
│   ├── letter-001.html     # Individual letter pages
│   ├── letter-002.html
│   └── letter-003.html
├── images/
│   ├── scans/              # High-resolution letter scans
│   └── photos/             # Portrait and other photos
└── README.md
```

## Adding New Letters

1. **Scan the letter** at high DPI (300+ recommended)
2. **Create the HTML file** by copying an existing letter template from `/letters/`
3. **Update the metadata** at the top (date, location, topics, etc.)
4. **Replace the placeholder** with your scanned image
5. **Update the transcription** with the OCR text
6. **Add the letter card** to `index.html` in the gallery grid
7. **Update navigation links** in adjacent letter pages

## Adding Images

### Letter Scans
Place high-resolution scans in `/images/scans/` and update the letter HTML:

```html
<img src="../images/scans/letter-001.jpg" alt="Letter dated March 15, 1943">
```

### Portrait Photo
Place the portrait in `/images/photos/` and update `index.html`:

```html
<img src="images/photos/grandfather-portrait.jpg" alt="Portrait">
```

## Design Notes

- **Fonts**: Special Elite (typewriter), Playfair Display (headings), Source Serif 4 (body)
- **Colors**: Olive drab military palette with aged paper tones
- **Theme**: WW2-era correspondence aesthetic

## Hosting

This is a static site designed to be hosted as a subdirectory of willaustin.net.

---

*Austin Family Archive — Preserving History, One Letter at a Time*
