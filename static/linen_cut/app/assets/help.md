# linen_cut

Version 1.1 · 26 June 2026

## What is this?

**linen_cut** is a free web app for planning how to cut a piece of linen into rectangles for art canvases.

You draw your linen on screen, place canvas sizes on it, and see each **cut size** (canvas plus overlap for stapling on stretcher bars). It helps you fit canvases onto a roll or length of fabric before you cut.

Linen is often bought in rolls a few metres long, typically about **2 m wide**. Default settings are **3 m × 2 m** linen; you can change both dimensions up to **10 m**.

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

- **Linen** — pale grey/brown rectangle; size set in the app bar (desktop) or toolbar (narrow screens).
- **Canvas** — white rectangle; drag to move, corner handles to resize when selected.
- **Grey border** — overlap allowance around each canvas (set by the Overlap box).
- **Labels** — show canvas size and cut size, e.g. `canvas = 25 x 35; cut = 35 x 45` (units follow the m/in toggle).

Cut size = canvas size + twice the overlap on each axis.

Positions snap to **1 cm** in metres mode, or **0.5 inch** in inches mode. Minimum canvas size is **10 cm × 10 cm**.

The origin is the **bottom-left corner of the linen**. Canvases can overlap on screen; avoiding wasted fabric is up to you.

## Toolbar

| Control | What it does |
|--------|----------------|
| **Overlap** | Extra linen on each side for stapling (default 0.1 m, max 0.3 m). |
| **m / in** | Switch display units. |
| **Add canvas** | Adds a canvas. **First canvas:** 70 × 70 cm, centred on the linen. **Later canvases:** placed about half a canvas width from the **selected** canvas (or **last edited** if none selected); size from that same canvas, else default **0.2 m × 0.3 m** at the bottom-left. |
| **Rotate** (↺) | Swaps the selected canvas width and length. Disabled until a canvas is selected. |
| **Align left** | Moves other canvases whose left edge is within **30 cm** of the selected canvas’s left edge so they line up with it. |
| **Align top** | Same for **top** edges (within 30 cm). |
| **Delete** (red bin) | Removes the selected canvas. Disabled until a canvas is selected. Undo with Ctrl+Z. |
| **Zoom in / out** | Change on-screen scale only; real sizes stay the same. |
| **Center** | Reset pan so linen is centred. |
| **Screenshot** | Saves the current drawing area as a JPEG download. |
| **Help** | Opens this document. |
| **Delete all** | Removes every canvas (undo with Ctrl+Z). |
| **Separate** | Spreads **all** overlapping canvases apart. Each pair ends up with about **5 cm** between the white canvas faces (not the grey cut margin). Canvases may move **outside** the linen. Disabled until there are at least two canvases. Undo with Ctrl+Z. |

### Checkboxes

- **Pan viewport on empty drag** — On: dragging empty space pans the whole view. Off: dragging empty linen pans only the linen on screen.
- **Canvases follow linen** — Only when viewport pan is off. On: canvases move with the linen when you pan it. Off: canvases stay fixed on screen while the linen moves underneath.

## Mouse and touch

Click or tap the drawing area first so keyboard shortcuts work there (desktop).

| Action | Desktop | Phone / narrow screen |
|--------|---------|------------------------|
| Select canvas | Click inside it. | Tap or long-press inside it. |
| Move canvas | Drag inside the white area. | Drag inside the white area. |
| Resize canvas | Drag a blue corner handle (selected canvas). | Drag a blue corner handle (selected canvas). |
| Rotate canvas | Double-click inside the canvas, or **Rotate** (↺) in the toolbar. | Select the canvas, then tap **Rotate** (↺) in the toolbar. |
| Pan | Drag empty background (behaviour depends on checkboxes above). | Same. |
| Delete canvas | Select it, then **Delete** (red bin) in the toolbar, or **Backspace** / **Delete**. | Select it, then the red **Delete** bin in the toolbar, or keyboard if available. |
| Separate overlapping canvases | **Separate** in the toolbar (after **Delete all**). | **Separate** icon in the icon row, or **Separate canvases** in **⋮** (More). |

On narrow screens the toolbar uses **icon buttons** only; tap **⋮** (More) for **Separate canvases**, Screenshot, Help, Delete all, and the pan checkboxes.

Linen length, width, overlap, and units appear in the compact toolbar. Dimensions use **metres** by default; tick the **in** checkbox in the icon row to switch to inches. Use the **⇄** button next to the linen size boxes to swap length and width.

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
- **Add canvas** repeats the size of the canvas you have selected, or the last one you moved, resized, or rotated — handy for placing several of the same size.
- On a phone, **Rotate** (↺) is the easiest way to turn a canvas — select it first, then tap the button.
- Copy and paste is handy for repeating the same canvas size in different places.
- **Separate** is useful when canvases have been stacked on top of each other — it pushes them apart with roughly **5 cm** between each pair. The result is approximate (positions snap to the grid) and canvases can end up off the linen; drag them back or use **Align left** / **Align top** if needed.
- Switch to inches if your stretchers are sized in imperial units; internal storage stays in metres.

---

*Questions or bugs? This is a personal planning tool — use your own judgement before cutting expensive fabric.*
