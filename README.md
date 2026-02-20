# Google Earth Engine Python 101

This repository contains beginner-friendly lab and workshop notebooks for the Stanford Geospatial Center. The materials focus on Google Earth Engine with the Python API and use `geemap` for inline visualization.

## Audience
These notebooks assume little to no experience with spatial data or programming. Each notebook includes beginner-focused explanations, inline code comments, and concept checks.

## Running the Notebooks
You can run these notebooks in either Google Colab or local Jupyter. The notebooks are written to support both.

### Option 1: Google Colab
1. Open a notebook in Colab.
2. Run the first code cell to install libraries.
3. When prompted, authenticate Earth Engine in the browser.
4. For Planet API notebooks, add `PL_API_KEY` in Colab Secrets and enable notebook access.

### Option 2: Local Jupyter
1. Create and activate a Python environment.
2. Start Jupyter Lab or Jupyter Notebook.
3. Run the first code cell to install libraries.
4. Authenticate Earth Engine when prompted.
5. For Planet API notebooks, create a `.env` file with your key:

```bash
PL_API_KEY="PASTE_YOUR_PLANET_API_KEY_HERE"
```

Use `.env.example` as a template and keep `.env` out of version control.

## Notebook List
1. `notebooks/00_codeeditor_to_python_basic_syntax.ipynb` basic Python syntax primer.
2. `notebooks/01_authentication_and_libraries.ipynb` Earth Engine authentication and core libraries.
3. `notebooks/02_image_collections_bands_and_pixels.ipynb` image collections, bands, and pixels.
4. `notebooks/03_multispectral_imagery_visualizations.ipynb` true color, false color, and NDVI.
5. `notebooks/10_largest_fire_today_workflow copy.ipynb` find the largest active fire using NASA FIRMS.
6. `notebooks/11_order_planetscope_of_largest_fire.ipynb` order PlanetScope imagery for the largest fire.

## Notes
1. Some notebooks download or export outputs to the `notebooks/output` folder.
2. PlanetScope data requires a Planet API key and valid account access.
