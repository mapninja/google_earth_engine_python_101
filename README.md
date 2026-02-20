# Google Earth Engine Python 101

Short URL for this repo: [goto.stanford.edu/gee-python-101](https://goto.stanford.edu/gee-python-101)

Intro to Earth Engine Slides: [slides.com/staceymaples/gee101](https://slides.com/staceymaples/gee101)

JavaScript Editor Sample Scripts: [goo.gl/9f9NgB](https://goo.gl/9f9NgB)

This repository contains beginner-friendly lab and workshop notebooks for the Stanford Geospatial Center. The materials focus on getting started quickly with the Google Earth Engine Python API and use `geemap` [for inline visualization](https://geemap.org/).

## Audience

These notebooks assume little to no experience with spatial data or programming. Each notebook includes beginner-focused explanations, inline code comments, and concept checks.

## Getting started with Google Earth Engine

First, all users must have an active Google Earth Engine account, and the ability to create Google Cloud Projects, for use with Google Earth Engine.

If you are a Stanford User attending a workshop, you should already be added to the Stanford GEE Access Workgroup.

If you are not a Stanford affiliate, you can [request access to Google Earth Engine using your personal credentials](https://earthengine.google.com/).

## Logging in to Google Earth Engine and creating a new Project

1. First, go to [https://code.earthengine.google.com/](https://code.earthengine.google.com/) and log in using your Stanford credentials (or personal, if not a Stanford affiliate).

   ![](images/20260220_110253_image.png)
2. Click on your Profile Icon, in the top right of the Code Editor and select Register a new Cloud Project.

   ![](images/20260220_110446_image.png)
3. Give your new project a valid Project name:

   ![](images/20260220_110920_image.png)
4. Click on the Parent resource>Browse link, and Select "GEE Student Projects"

   ![](images/20260220_110944_image.png)
5. Click the Create button to mint your new project:

   ![](images/20260220_111042_image.png)
6. If you aren't taken to the COnfiguration Dashboard, you can click on the "Select Project" to make the new Project active, and begin the registration process:

   ![](images/20260220_111231_image.png)

You should now be in the Configuration Dashboard. Double-check that you are viewing the config for the Project you just created.

![](images/20260220_111545_image.png)

## Registering a new Google Cloud Project

Now, we have to register the Project we will use a non-commercial. This will provide us access to the GEE API, and generous compute quotas, without billing.

1. From the COnfiguration Dashboard for your Project, Click on the **See if you are eligible for non-commercial use**> **Get Started** button:

   ![](images/20260220_112130_image.png)
2. Complete the Registration Form with the appropraite answers for your use cases, then click on the Check Eligibility button to complete the form:

   ![](images/20260220_112335_image.png)
3. Since your Stanford GCP Project is not attached to a billing account, in the next step you should select "Community" which is the appropriate tier for Students and small research projects. If you need more capacity, you can contact UIT for access to GCP Projects with Billing Enabled (Stanford Facult PI and PTA, required).

   ![](images/20260220_112550_image.png)
4. Complete the remaining Registration steps and click the Register button to complete the process.

   ![](images/20260220_112722_image.png)

   ![](images/20260220_112807_image.png)
5. You should be presented with a pop-up that allows you to enable the Earth Engine API:

   ![](images/20260220_112855_image.png)

## Enable the Earth Engine API

1. Click on the Enable link in the pup-up window that results from your completion of the Registration process:

   ![](images/20260220_112941_image.png)

## Select your project in Earth ENgine

1. Return to the Code Editor and click on the Profile Icon to Select> **Choose a Cloud Project**

   ![](images/20260220_113116_image.png)![](images/20260220_113340_image.png)
2. Select your Project and click on the Select button.

![](images/20260220_113402_image.png)

3. Once you have selected your Project, you can test that all is working by simply running one of your scripts! In case you don't have one, you can use this one: [https://code.earthengine.google.com/f983a2d843739e23ffb77f336ad6d4fb](https://code.earthengine.google.com/f983a2d843739e23ffb77f336ad6d4fb)

## Switching to the Python API!

You can run these notebooks in either Google Colab or local Jupyter. The notebooks are written to support both.

### Option 1: Google Colab

1. Open a notebook in Colab.
2. Run the first code cell to install libraries.
3. When prompted, authenticate Earth Engine in the browser.

### Option 2: Local Jupyter

1. Create and activate a Python environment.
2. Start Jupyter Lab or Jupyter Notebook.
3. Run the first code cell to install libraries.
4. Authenticate Earth Engine when prompted.

## Notebook List

1. `notebooks/00_codeeditor_to_python_basic_syntax.ipynb` basic Python syntax primer. [https://colab.research.google.com/github/mapninja/google_earth_engine_python_101/blob/main/notebooks/00_codeeditor_to_python_basic_syntax.ipynb](https://colab.research.google.com/github/mapninja/google_earth_engine_python_101/blob/main/notebooks/00_codeeditor_to_python_basic_syntax.ipynb)
2. `notebooks/01_authentication_and_libraries.ipynb` Earth Engine authentication and core libraries. [https://colab.research.google.com/github/mapninja/google_earth_engine_python_101/blob/main/notebooks/01_authentication_and_libraries.ipynb](https://colab.research.google.com/github/mapninja/google_earth_engine_python_101/blob/main/notebooks/01_authentication_and_libraries.ipynb)
   </a>
3. `notebooks/02_image_collections_bands_and_pixels.ipynb` image collections, bands, and pixels. [https://github.com/mapninja/google_earth_engine_python_101/blob/main/notebooks/02_image_collections_bands_and_pixels.ipynb](https://github.com/mapninja/google_earth_engine_python_101/blob/main/notebooks/02_image_collections_bands_and_pixels.ipynb)
4. `notebooks/03_multispectral_imagery_visualizations.ipynb` true color, false color, and NDVI. [https://github.com/mapninja/google_earth_engine_python_101/blob/main/notebooks/03_multispectral_imagery_visualizations.ipynb](https://github.com/mapninja/google_earth_engine_python_101/blob/main/notebooks/03_multispectral_imagery_visualizations.ipynb)
5. `notebooks/10_largest_fire_today_workflow copy.ipynb` find the largest active fire using NASA FIRMS. [https://colab.research.google.com/github/mapninja/google_earth_engine_python_101/blob/main/notebooks/10_largest_fire_today_workflow%20copy.ipynb](https://colab.research.google.com/github/mapninja/google_earth_engine_python_101/blob/main/notebooks/10_largest_fire_today_workflow%20copy.ipynb)

## Notes

1. Some notebooks download or export outputs to the `notebooks/output` folder.
2. PlanetScope data requires a Planet API key and valid account access.

![](images/20260220_130558_image.png)
