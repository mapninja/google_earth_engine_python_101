# Google Earth Engine @ Stanford
## Getting Started with GEE and Google Cloud Platform

---

## What is Google Earth Engine?

Google Earth Engine is a cloud-based geospatial analysis platform that provides instant access to petabytes of satellite imagery and geospatial datasets. Instead of downloading massive files to your computer, Earth Engine lets you analyze global-scale imagery directly on Google's servers—a capability essential for modern environmental research, climate science, agriculture monitoring, and disaster response. Explore the available [datasets in the Earth Engine catalog](https://developers.google.com/earth-engine/datasets/).

### Why Earth Engine Matters for Stanford Researchers

- **No hardware investment required** — all computation happens in the cloud
- **Access to decades of satellite imagery** — [Landsat, Sentinel, MODIS, and hundreds of other datasets](https://developers.google.com/earth-engine/datasets/)
- **Programming flexibility** — use JavaScript in the [Code Editor](https://code.earthengine.google.com/) or Python in your own workflows
- **Real-time processing** — analyze changes at regional and global scales instantly

---

## Getting Access to Earth Engine at Stanford

### Step 1: Join the GIS Users Workgroup

Contact the [Stanford Geospatial Center](https://library.stanford.edu/libraries/stanford-geospatial-center) to request membership in the **GIS Users Workgroup**. This gives you:
- Access to the Stanford Geospatial Center at Branner Library
- Network storage (R: drive on SGC lab machines)
- Earth Engine access via the browser-based [Code Editor](https://code.earthengine.google.com/)
- Eligibility for GCP project creation

**Contact:** stanford-geospatial@stanford.edu

### Step 2: Create Your Google Cloud Project

Once you're added to our GCP workgroup for student access, you'll gain two immediate benefits: increased quotas and improved performance. Most importantly, you'll get access to the Python API, which requires a GCP project for authentication.

To set up your project, follow these steps:

**Sign in with fresh permissions:**
First, sign out of your Google account completely, clear your browser cache, and sign back in. This ensures you have access to the new GCP project creation permissions.

**Create your project:**
When you access the Cloud Project menu in the [Earth Engine Code Editor](https://code.earthengine.google.com/), you'll be prompted with a "Create Project" dialog. Create a new project and select the `gee_student` folder as the location for your project.

**Complete the setup:**
You'll then see two prompts you must complete:
1. Confirm non-commercial use
2. Enable the Earth Engine API

Both steps have clear on-screen instructions. This entire process takes approximately 15 minutes and requires no billing information (Earth Engine is free for research and educational use).

Note: Your project is restricted to Earth Engine API use only. You won't be able to enable other Google APIs that require billing, but that's by design to keep the service freely available for student research.

### Step 3: Verify Your Setup

After you complete onboarding, test your Earth Engine Python API access with this verification notebook from Google:

[Earth Engine Python API Setup Verification](https://colab.research.google.com/github/google/earthengine-community/blob/master/guides/linked/ee-api-colab-setup.ipynb)

When you run this notebook in Google Colaboratory, replace the `project_folder` parameter in the second code block with your new project name. This notebook confirms that your API permissions are set up correctly and your Python API access is working.

If you encounter any issues during onboarding or when running the verification notebook, please contact the Stanford Geospatial Center with a screenshot if possible. Your feedback helps us improve the documentation and process.

---

## Your First Steps with Earth Engine

### Learning Resources

**SGC Workshops & Training**
- Attend live workshops: "Google Earth Engine: An Introduction for Complete Beginners"
- Access self-paced learning modules at Stanford Geospatial Center
- Visit [Stanford Geospatial Center Events](https://events.stanford.edu/department/stanford_geospatial_center) for upcoming sessions

**Official Documentation**
- [Google Earth Engine Home](https://earthengine.google.com/) – Main Earth Engine page
- [Earth Engine User Guide](https://developers.google.com/earth-engine)
- [Earth Engine API Tutorials](https://developers.google.com/earth-engine/tutorials)
- [Earth Engine Python API Documentation](https://developers.google.com/earth-engine/apidocs)

**Recent Innovations**
- [AlphaEarth Embeddings](https://developers.google.com/earth-engine/datasets/catalog/GOOGLE_SATELLITE_EMBEDDING_V1_ANNUAL) – Google's new satellite embedding dataset enabling advanced machine learning applications with satellite imagery

**Community Resources**
- [Awesome Google Earth Engine](https://awesome.geemap.org/) — curated resource list
- [GEE Community Catalog](https://gee-community-catalog.org/) — community-contributed datasets and scripts
- [Cloud-Based Remote Sensing with GEE: Fundamentals and Applications](https://www.eefabook.org/) — free, comprehensive textbook

### Getting Help

The Stanford Geospatial Center provides:
- Technical support and troubleshooting
- Office hours and walk-in consultations at Branner Library
- Email support at gis@stanford.edu
- Community forums and discussion groups

---

## FAQ

**Q: Do I need to pay for Earth Engine?**  
A: No. Google Earth Engine is free for research and educational purposes. Your Stanford affiliation qualifies you automatically.

**Q: Can I use Earth Engine in my class?**  
A: Yes! Contact the Stanford Geospatial Center to discuss curriculum integration and student onboarding.

**Q: Do I really need to set up a GCP project?**  
A: Yes. A GCP project is now required for all Earth Engine use—both the [Code Editor](https://code.earthengine.google.com/) and the Python API. Creating a GCP project unlocks several key benefits. You'll get increased quotas for larger analyses, improved performance and faster processing times, access to the Python API (essential for automation and integration with other tools), and the current version of Earth Engine rather than the legacy interface.

**Q: Can I access Earth Engine from home?**  
A: Yes. Once your GCP project is set up, you can access Earth Engine from anywhere with an internet connection—both the [Code Editor](https://code.earthengine.google.com/) and the Python API.

**Q: What data can I use?**  
A: Earth Engine hosts hundreds of public [datasets available in the Earth Engine catalog](https://developers.google.com/earth-engine/datasets/), including:
- Landsat (free US Geological Survey satellite imagery, 1972–present)
- Sentinel-1 & -2 (free European Space Agency satellites)
- MODIS (NASA daily global imagery)
- Google's high-resolution basemap
- Climate, weather, and environmental datasets

---

## Next Steps

1. **Reach out to SGC:** Email gis@stanford.edu to request GIS Users Workgroup access
2. **Complete GCP setup** when you receive the invitation
3. **Test your access** using the verification notebook
4. **Attend a workshop** or explore the learning resources above
5. **Connect with the community** at SGC events and forums

---

## Contact & Resources

**[Stanford Geospatial Center](https://library.stanford.edu/libraries/stanford-geospatial-center)**  
Branner Library, Stanford University  
Email: stanford-geospatial@stanford.edu  
Web: [gis.stanford.edu](https://gis.stanford.edu)

**[Stanford Libraries Research Data Services](https://library.stanford.edu/libraries/research-data-services)**  
Web: [library.stanford.edu/research](https://library.stanford.edu/research)

**[Stanford Doerr School of Sustainability](https://sustainability.stanford.edu/)**  
Web: [sustainability.stanford.edu](https://sustainability.stanford.edu/)

**[University Information Technology (UIT)](https://uit.stanford.edu/)**  
Web: [uit.stanford.edu](https://uit.stanford.edu)

---

## Upcoming Events

Visit [Stanford Geospatial Center Events](https://events.stanford.edu/department/stanford_geospatial_center) for:
- Earth Engine workshops and seminars
- Geospatial analysis training
- Community meetups and networking events
- Advanced technique courses

