# linen_cut

Version 1 · Release 1 · 23 June 2026

## What is this?

**linen_cut** is a free web app for planning how to cut a piece of linen into rectangles for art canvases.

You draw your linen on screen, place canvas sizes on it, and see each **cut size** (canvas plus overlap for stapling on stretcher bars). It helps you fit canvases onto a roll or length of fabric before you cut.

Linen is often bought in rolls a few metres long, typically about **2 m wide**. Default settings are **3 m × 2 m** linen; you can change both dimensions up to **10 m**.

**linen_cut is free to use.** There is no account, subscription, or payment. But you could buy me a coffee...

## Your data

Everything is stored **only in your browser** (local storage). One layout is saved automatically whenever you change something.

Stored data includes:

- Linen length and width
- Overlap size and unit (metres or inches)
- Toolbar checkbox settings
- Zoom and pan position
- All canvases (position, size, rotation)

Nothing is sent to a server. If you clear browser data for this site, or use a different browser or device, your layout will not be there. Use **Screenshot** to save a JPEG copy of the current view.

## On-screen layout

- **Linen** — pale grey/brown rectangle; size set in the app bar.
- **Canvas** — white rectangle; drag to move, corner handles to resize.
- **Grey border** — overlap allowance around each canvas (set by the Overlap box).
- **Labels** — show canvas size and cut size, e.g. `canvas = 25 cm × 35 cm; cut = 35 cm × 45 cm`.

Cut size = canvas size + twice the overlap on each axis.

Positions snap to **1 cm** in metres mode, or **0.5 inch** in inches mode. Minimum canvas size is **10 cm × 10 cm**.

The origin is the **bottom-left corner of the linen**. Canvases can overlap on screen; avoiding wasted fabric is up to you.

## Toolbar

| Control | What it does |
|--------|----------------|
| **Overlap** | Extra linen on each side for stapling (default 0.1 m, max 0.3 m). |
| **m / in** | Switch display units. |
| **Add canvas** | Adds a 0.2 m × 0.3 m canvas at the bottom-left (or next free slot). |
| **Zoom in / out** | Change on-screen scale only; real sizes stay the same. |
| **Center** | Reset pan so linen is centred. |
| **Screenshot** | Saves the current drawing area as a JPEG download. |
| **Help** | Opens this document. |
| **Delete all** | Removes every canvas (undo with Ctrl+Z). |

### Checkboxes

- **Pan viewport on empty drag** — On: dragging empty space pans the whole view. Off: dragging empty linen pans only the linen on screen.
- **Canvases follow linen** — Only when viewport pan is off. On: canvases move with the linen when you pan it. Off: canvases stay fixed on screen while the linen moves underneath.

## Mouse and touch

Click the drawing area first so keyboard shortcuts work there.

| Action | How |
|--------|-----|
| Select canvas | Click inside it. |
| Move canvas | Drag inside the white area. |
| Resize canvas | Drag a blue corner handle. |
| Rotate canvas | Double-click inside the canvas (swaps width and length). |
| Pan | Drag empty background (behaviour depends on checkboxes above). |
| Delete canvas | Select it, then **Backspace** or **Delete**. |

## Keyboard crib sheet

Shortcuts apply when the **drawing area** has focus (click it once). They do not fire while you are typing in a number box.

| Keys | Action |
|------|--------|
| **Ctrl+Z** | Undo last change (up to 10 steps). |
| **Ctrl+Y** | Redo. |
| **Ctrl+C** | Copy canvas under the cursor (or the selected canvas). |
| **Ctrl+V** | Paste copied canvas at the cursor. |
| **Backspace** / **Delete** | Delete selected canvas. |

## Tips

- Use **Center** after panning or zooming if you lose the linen.
- Copy and paste is handy for repeating the same canvas size in different places.
- Switch to inches if your stretchers are sized in imperial units; internal storage stays in metres.

---

*Questions or bugs? This is a personal planning tool — use your own judgement before cutting expensive fabric.*
