# StagePlot

A free, browser-based previsualization sketchpad for stage and set design.

Stage Plot lets set designers, directors, production designers and students lay out a stage picture before anyone lifts a flat: place furniture and structures from a searchable catalog of 300 properties, block performers against them for scale, and move between a top-view plan and an audience point of view with one drag. It runs as a single HTML file: no install, no login, no server, no account.

**Live version:** https://gauravnijjer.github.io/StagePlot

Made by [Gaurav Singh Nijjer](https://gauravnijjer.com)

---

## A note from the maker

Stage Plot began in my own rehearsal rooms. Set conversations kept happening in words and hand-waves: a sofa described in the air, a platform promised for next week, a bridge that everyone imagined differently until build day proved us all wrong. I wanted the team to see a shared picture early, one anyone could open on a laptop and point at, move a chair in, and argue with. Serious tools already exist for this, SketchUp, Vectorworks and full CAD packages among them, and they do far more than this ever will. I just wanted one that's easy, works in the browser, and can be picked up within 30 seconds of looking at it. So I designed this one, and its companions, around the actual needs of that room: free, single-file, no login, nothing locked away.

It's also part of my larger practice. My work in theatre and installation uses creative code and technology to examine AI critically while using it generously, and initiatives like this suite are the constructive half of that: putting AI to work in ways that give agency to artists rather than take it away, widening who gets to previsualize, plan and dream before build day. I come to this with a long history in web development, creative coding and design, which is what shaped every decision here about how the tool should feel and what it should refuse to complicate.

The code itself was built in collaboration with Claude, Anthropic's AI assistant, through Claude Code, across many rounds of my direction, testing and revision. I name that openly because honesty about the making is part of using these systems well, and because the judgment about what deserved to exist stayed human throughout.

---

## What it does

**Two views of the stage, one gesture apart.** The tool opens in a top view (plan). Drag the empty canvas downward and the camera tilts smoothly into an audience point of view, so the same layout reads as both a ground plan and a stage picture.

**A catalog of 300 stage properties, searchable.** Type "chair," "fountain," "platform," "train," "charpai," "almirah," anything, into the search bar and matching pieces appear grouped by category, one click from being placed centre stage. The catalog spans 18 categories: seating, tables, storage, platforms in a generated grid of sizes and heights, stairs from 2 to 7 steps, ladders and access, walls and flats in multiple widths, curtains and soft goods, large structures (bridge, balcony, tower, gazebo, colonnade, proscenium piece), domestic and kitchen, office and school, music and band, garden and trees, street and road, railway station, village and period pieces including Indian household objects, theatre and backstage, and miscellaneous props.

**Every piece is fully adjustable.** Each placed property has its own line color, a line or fill render mode, a uniform scale from 0.3× to 3×, separate width and depth stretch along its own axes (so a flat becomes exactly as long as your wall needs to be), a full rotation, and an elevation for placing things on platforms. Fill mode renders flat shaded faces with the drawn edges kept, so the piece stays in the house language while reading as a solid.

**A quick bar on the canvas.** Select any piece and a small floating toolbar appears beside it with line/fill, a color picker, and group/ungroup, so the common edits never require opening the panel.

**Grouping.** Shift-click pieces on the canvas or in the list to multi-select, then group them. Grouped pieces move together, rotate together around their shared centre (R), recolor together, and delete together. A dining table and its six chairs become one object.

**Performers for scale.** White line figures, 1.75m tall, draggable at any time. Keep one next to that bridge before committing to its height.

**A backdrop.** A full-width upstage surface in wash or gradient mode with a color picker, standing in for a cyclorama.

**50 starter scenes.** Ten everyday ones up front (living room, dining, bedroom, office, classroom, street corner, park, forest, train station, road) and forty more behind a load-more button, from village square and throne room to graveyard, harbor dock, wedding mandap, band stage, prison cell and press conference. Every starter scales to your stage dimensions and is meant to be pulled apart and rebuilt.

**Scenes as files.** One scene is one complete stage picture: every placed property with its position, rotation, scale, stretch, color, mode and grouping, plus the backdrop and performers. Save it as a file, reload it later, or share it with a collaborator.

**Plot sheet export.** One click produces a PNG containing the top view, the audience view, and a full property schedule: number, name, category, position, rotation, scale, stretch, elevation, group, render mode and a color swatch for every piece. Made to be dropped into an email to a workshop or a production meeting.

---

## Controls

| Action | Input |
|---|---|
| Tilt between top view and audience view | Drag empty canvas up / down |
| Place a property | Search in settings, click its button |
| Move a piece or performer | Drag it |
| Select a piece | Click it |
| Multi-select | Shift-click (canvas or list) |
| Group / ungroup selection | Buttons on the quick bar or in the panel |
| Rotate selection by 45° | R |
| Delete selection | Delete / Backspace |
| Open or close the settings panel | S (or the settings button, bottom right) |
| Snap to top view / audience view | T / F |

The settings panel holds everything else: stage dimensions, the backdrop, starter scenes, the property catalog with search, the on-stage list with full per-piece editing, performers, and export / save / load.

---

## What is modeled, honestly

Stage Plot is an indicative design planning tool, not a CAD package. So that you know exactly where the line sits:

- Dimensions are sensible defaults in meters, not manufacturer specifications. A chair is a chair-sized chair; check real measurements before building.
- Pieces are simplified wireframe silhouettes designed to read clearly, not detailed models.
- Fill mode uses painter's-algorithm ordering. Separate pieces layer correctly; two pieces physically intersecting each other can occasionally overlap oddly.
- There is no collision, physics, or weight-bearing logic. The tool will happily let you float a sofa on air, which is also what the elevation slider is for.

Treat everything here as a shared starting point for the conversation, and confirm on the ground with a tape measure.

---

## Access

Access it via the link https://gauravnijjer.github.io/StagePlot

It works on desktop (recommended) and mobile, though a mouse or trackpad gives the best experience for detailed placement.

---

## Companion tools

Stage Plot is one of a small suite of single-file previz tools sharing the same black-canvas, white-line language:

- **Light Plot** — stage lighting with true beam cone geometry, elliptical throws, shutter cuts, additive color mixing and a projection screen. Explore it here: https://gauravnijjer.github.io/LightPlot

---

## Built with

Stage Plot is built on [p5.js](https://p5js.org/) and was made using **Claude Code** (Anthropic), with design direction, testing and feature decisions by Gaurav Singh Nijjer.

---

## Feedback, bugs and requests

This is a beta, shared in the open because other designers and directors might get some use out of it. If something breaks, feels wrong, or is missing the one property or feature you need, write to **gauravnijjer@gmail.com**. Corrections and requests from working set designers are especially welcome.

---

## License

**Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)**

You are free to use and share this tool for **personal and educational use**, with attribution to Gaurav Singh Nijjer. **Commercial use is not permitted** without written permission. For commercial licensing enquiries, contact gauravnijjer@gmail.com.
Full license text: https://creativecommons.org/licenses/by-nc/4.0/

© Gaurav Singh Nijjer 2026 · [gauravnijjer.com](https://gauravnijjer.com)
