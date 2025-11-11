## AI coding guide for this repo (Earth Engine + geemap)

This repository is an educational, notebook-first walkthrough of Google Earth Engine (GEE) in Python using geemap. It contains Jupyter notebooks under `notebooks/` and no package, build, or test system.

### Big picture
- Structure: numbered notebooks in `notebooks/` (e.g., `00_...` to `03_...`) that build from authentication to imagery visualization.
- Goal: teach core GEE Python workflows; each notebook is a self-contained lesson rather than a library.
- Runtime: Jupyter kernels only. There’s no CLI, API server, or scripts to run.

### What to edit / generate
- Add or improve content inside the existing notebooks rather than creating new modules.
- Keep examples minimal and runnable top-to-bottom within a single notebook.
- Prefer adding new lessons as new numbered notebooks (e.g., `04_<short-topic>.ipynb`).

### Environment and dependencies (assumed for this project)
- Python with Jupyter, plus Earth Engine and geemap:
  - pip packages: `earthengine-api`, `geemap`, `jupyter`
- Authentication is expected to happen inside a notebook (typical pattern below). If terminal auth is desired, it’s optional.

### Common patterns to use in notebooks
- Imports (keep consistent across notebooks):
  - `import ee`
  - `import geemap as geemap`
- Auth/init when needed:
  - `ee.Authenticate()` (first-time); then `ee.Initialize()`
- Map workflow with geemap:
  - `m = geemap.Map()`
  - `m.addLayer(image, vis_params, 'Layer name')`
  - `m`
- Example vis params for multispectral RGB:
  - `{ 'bands': ['B4', 'B3', 'B2'], 'min': 0, 'max': 3000 }` (Sentinel-2 or Landsat variants as applicable)

### Conventions in this repo
- File naming: two-digit prefix to indicate order (e.g., `01_authentication_and_libraries.ipynb`).
- Keep cells short; prefer one concept per cell with a markdown explanation preceding code.
- Use clear layer names in `addLayer` and show the map object as the last statement of the cell.

### External services and data
- Primary data source is Google Earth Engine assets and collections (no local data management in this repo).
- Expect remote computation latency; prefer lightweight previews (thumbnails, simple composites) over heavy exports.

### Debugging and gotchas
- If `ee.Initialize()` fails, re-run `ee.Authenticate()` in the same kernel/session and retry.
- Notebook state matters—restart the kernel before re-running a lesson end-to-end.
- Visualizations failing silently? Check band names and scales match the chosen collection.

### What’s currently known vs inferred
- The repository contains placeholder notebooks (no cells at time of writing). Patterns above are inferred from notebook names and typical GEE+geemap usage.
- When content is added, keep to these patterns for consistency. If the repo adopts different imports or flows, update this guide.

### Examples tied to files
- `01_authentication_and_libraries.ipynb`: demonstrate `ee.Authenticate()`, `ee.Initialize()`, and creating a `geemap.Map()`.
- `02_image_collections_bands_and_pixels.ipynb`: load an ImageCollection and select bands before display.
- `03_multispectral_imagery_visualizations.ipynb`: apply RGB/natural color visualization and add to the map.

---
Feedback welcome: if any of the conventions above don’t match the intended approach, point to a canonical example and I’ll update this guide.
