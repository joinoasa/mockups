# OASA mockups

Rough 3D concept mockups of nodes on the [OASA tech tree](https://joinoasa.org/techtree/). Each one runs in the browser: rotate it, explode it and tap a part to see what it does and which nodes it belongs to.

**View them:** <https://joinoasa.github.io/mockups/>

| Folder | Node | What it shows |
|---|---|---|
| [`site/`](site/) | T-SITE1–3, G-10, T-DOCK2, T-SAFE1, T-LEARN1 | A whole landscaping job, start to finish (start here) |
| [`rcom5/`](rcom5/) | R-COM5 | Open SDR radio core and its versions |
| [`g10/`](g10/) | G-10 | Open tracked platform, robot types and quick-attach tools |
| [`g2/`](g2/) | G-2 | Legged dog and spider for extreme terrain ([IDEA #117](https://github.com/joinoasa/ideas/issues/117)) |
| [`t-site1/`](t-site1/) | T-SITE1 | Survey drone airframes, sensors and a survey mission |
| [`t-dock/`](t-dock/) | T-DOCK1–3 | Drone docks: field, battery swap, mobile hive and buoy |
| [`t-node2/`](t-node2/) | T-NODE1–2 | Mesh node kits and a mesh view with best-path routing |
| [`s-3/`](s-3/) | S-3 | Solar boat and the water robots built on it (S-1, S-4, S-5, S-6, U-4) |
| [`u-5/`](u-5/) | U-1–U-7 | Underwater robots and a reef scene |
| [`l-5/`](l-5/) | L-4–L-7 | Blimps: tethered, solar, wildfire watch, disaster relay and mothership |

These are block-level concepts for discussion. Shapes and sizes are guesses, not designs.

## Adding a mockup

1. Copy an existing folder (for example `g10/`) to a new folder named after the node, in lower case (`t-node2/`).
2. Edit `index.html`. Each part is defined once with a name, a short description, the node IDs it belongs to and where it moves in the exploded view.
3. Add a card for it to the top-level `index.html` and a row to the table above.
4. Open a pull request.

Each page is one self-contained HTML file. It uses [three.js](https://threejs.org/) r128 from `lib/` and no build step. To try a page locally, run `python3 -m http.server` in the repo folder and open <http://localhost:8000/>.

When the team picks a CAD tool, real CAD files for a node go in that node's folder next to its mockup.

## License

- **Code:** [Apache-2.0](LICENSE).
- **Content** (descriptions and models): [CC BY-SA 4.0](LICENSE-content).
- `lib/three.min.js` is three.js, [MIT](lib/three.LICENSE).
