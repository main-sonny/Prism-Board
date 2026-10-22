# Prism Whiteboard

A standalone HTML5 Canvas whiteboard with a glass-style interface. All HTML, CSS, and JavaScript are included in one file.

## Getting started

Open `prism-whiteboard.html` in a modern browser. No installation, build step, or server is required.

## Features

- Pen, highlighter, and whole-object eraser
- Rectangles, ellipses, lines, and arrows
- Text and editable sticky notes
- Image uploads, drag-and-drop, and image pasting
- Object selection, movement, resizing, duplication, and layering
- Undo and redo
- Zoom, pan, and fit-to-content
- Dot and line grids with optional snapping
- Custom colors, stroke widths, opacity, and background color
- Local browser autosave
- PNG, transparent PNG, and editable `.prism` exports
- Touch drawing and two-finger pinch zoom

## Files

| File | Purpose |
| --- | --- |
| `prism-whiteboard.html` | The complete application; this is the only file needed to run it. |
| `prism-check.js` | Temporary JavaScript extracted for a Node.js syntax check. Not required by the app and safe to delete. |
| `readme.me` | This guide. |

## Controls

| Action | Shortcut |
| --- | --- |
| Select | V |
| Pen | P or B |
| Highlighter | H |
| Object eraser | E |
| Rectangle | R |
| Ellipse | O |
| Line | L |
| Arrow | A |
| Text | T |
| Sticky note | N |
| Pan | Hold Space and drag |
| Zoom | Scroll or pinch |
| Fit content | Shift + 1 |
| Undo | Ctrl/Command + Z |
| Redo | Ctrl/Command + Shift + Z |
| Select all | Ctrl/Command + A |
| Duplicate | Ctrl/Command + D |
| Copy / paste | Ctrl/Command + C / V |
| Export editable board | Ctrl/Command + S |
| Open board or images | Ctrl/Command + O |
| Delete selected | Delete or Backspace |
| Cancel / deselect | Escape |

Shift-click objects to select multiple items, or drag empty space with the selection tool to box-select. Drag the bottom-right selection handle to resize. Double-click text or a sticky note to edit it.

Hold Shift while drawing to create squares, circles, or lines constrained to 45-degree increments. Image resizing preserves the aspect ratio.

## Saving and exporting

The app attempts to save your board in your browser's local storage. This is not cloud storage: saves are specific to the browser and may be unavailable in private browsing or when opening local files. Large images can exceed the storage quota.

For reliable backups, choose **Export board → Editable board**. Reopen the downloaded `.prism` file using the folder button or drag it onto the board. Opening a board replaces the current content; export your current board first if you want to keep it.

PNG exports include all objects, not just the visible area. The grid and selection controls are excluded. Choose **Transparent PNG** to omit the board background as well.

## Notes

- Use a recent version of Chrome, Edge, Firefox, or Safari.
- The eraser removes whole objects rather than individual pixels.
- There are no accounts, collaboration features, or backend services.
- Clearing browser data can delete locally saved work. Keep exported backups.
- Undo history is kept only for the current session.
