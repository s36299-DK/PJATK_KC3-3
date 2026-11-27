# Modules Plan — Mediterranean Italian House
**Course:** PJATK KC3-3  |  **Team:** Davyd Kulikov (s36299), Lukasz Pochwatko
**Grid tool:** Blender snapping (scale = 0.25 m cells in viewport) / UE5 snapping list

## 1. Modular grid
Base sizes are rounded from real Italian house proportions to the UE5 snapping values (0.01, 0.05, 0.1, 0.5, 1, 5, 10, 50 m):

| Element | Real-world (typ.) | Kit value | Grid |
|---|---|---|---|
| Floor height | 2.4 - 2.8 m | **2.5 m** | 5 x 0.5 m |
| Facade module width | 2.2 - 3.0 m | **2.5 m** | 5 x 0.5 m |
| Wall thickness | 0.30 - 0.40 m | **0.30 m** | 3 x 0.1 m |
| Window | 0.8 x 1.1 m | **0.9 x 1.2 m** (sill 0.9 m) | x 0.1 m |
| Arched window | 0.9 x 1.4 m | **0.9 x 1.4 m**, arch r = 0.45 m | x 0.05 m |
| Door | 0.95 x 2.05 m | **1.0 x 2.1 m** | x 0.1 m |
| Portal | 1.5 x 2.6 m | **1.6 x 2.7 m** | x 0.1 m |
| Stair step | 0.16 R x 0.28 D | **0.15 R x 0.30 D**, width 1.25 m | x 0.05 m |
| Roof pitch | 25 - 35 deg | **30 deg**, gable h = 1.25 m | 2.5 m base |
| Railing height | 0.85 - 1.0 m | **0.9 m**, bar spacing 0.12 m | x 0.01/0.1 m |
| Boundary wall | 0.5 - 0.8 m | **0.5 m** | 1 x 0.5 m |
| Chimney | 0.4 x 0.4 x 1.4 m | **0.5 x 0.5 x 1.5 m** | x 0.1 m |
| Balcony slab | 1.2 x 0.55 m | **1.25 x 0.6 x 0.15 m** | x 0.05 m |

**Primary modular grid: 2.5 m x 2.5 m** (one floor x one bay). **Detail grid: 0.1 m** (all openings, trims, bars).
Blender: set snap increment to 0.05 m (grid scale 0.25 in the viewport corner for visual check, increment 0.05 for precision).

## 2. Module list (14 modules)
| # | Module | Size | Key materials |
|---|---|---|---|
| 01 | Wall — Plain | 2.5 x 2.5 x 0.3 m | stucco (4 color variants) |
| 02 | Wall — Window + Shutters | 2.5 x 2.5 x 0.3 m, win 0.9 x 1.2 m | stucco, stone lintel, wood shutters, glass |
| 03 | Wall — Window + Flower Box | as 02 + box 0.9 x 0.3 x 0.25 m | + terracotta box, plants |
| 04 | Wall — Arched Window | 2.5 x 2.5 x 0.3 m, open 0.9 x 1.4 m | stucco, wood, glass |
| 05 | Wall — Corner | 2.5 x 2.5 m L, trim 0.3 m | stucco, stone trim + plinth |
| 06 | Door — Arched Stone Portal | portal 1.6 x 2.7 m, door 1.0 x 2.1 m | stone, wood, step |
| 07 | Roof — Gable End Wall | base 2.5 m, h 1.25 m | stucco, terracotta trim |
| 08 | Roof — Tile Slope | 2.5 x 2.5 m, 30 deg | terracotta coppi, ridge |
| 09 | Roof — Chimney | 0.5 x 0.5 x 1.5 m | brick/terracotta, stone cap |
| 10 | Balcony — Iron Railing | slab 1.25 x 0.6 x 0.15 m, rail 0.9 m | stone slab, iron (balustrade variant) |
| 11 | Stairs — Flight + Parapet | 10 steps 1.25 x 0.30 x 0.15 m | stone, green iron (variant) |
| 12 | Wall — Low Boundary | 2.5 x 0.5 x 0.3 m + posts | stone, stucco |
| 13 | Props — Urn + Plants | urn 0.35 dia x 0.45 h | terracotta, green |
| 14 | Rooftop — Terrace | 2.5 x 2.5 m, rail 0.9 m | stone slab, iron, wood |

## 3. Shared materials (set up once, reuse across modules)
- **Stucco plaster** — 4 variants: cream, ochre, pink-terracotta, pale blue (rough plaster, refs: References/Materials/rough-plaster.jpg, limestone-background-in-Aspra.jpg)
- **Terracotta** — roof coppi, flower boxes, urns, chimneys (warm orange-brown, slightly rough)
- **Stone (limestone)** — plinths, portal, steps, caps, corner trim (light beige-gray, blocky)
- **Wood (painted)** — shutters, doors, table/chairs: white, sage green, sky blue (weathered paint)
- **Iron (black/dark green)** — railings, drainpipe (thin, slightly rough)
- **Glass** — windows (simple translucent)

## 4. Per-module reference boards
Each folder `Mxx_<name>/` contains:
- `refboard.drawio` — reference board (open in https://app.diagrams.net, free; add the blockout screenshot into the dashed box, then File > Export as > PNG/PDF and save next to it)
- `description.md` — module description, dimensions, materials, what to model from each reference
Red circles on the reference images mark the elements that will be modeled.

## 5. Work division (equal workload, 7 modules each)
See `Work_division.txt`.

## 6. Next steps
1. TA accepts this plan (adjustments if needed).
2. Both members model the BLOCKOUT of their 7 modules (simple gray boxes, correct grid + silhouette).
3. Screenshot every blockout, insert into the module's refboard.drawio, export boards.
4. Update this folder with the exports; one team member submits the folder URL + work-division document.
