* Use Python 3.12
* Enforce PEP-8
* Document all the function and classes following NumPy standard
* Create a README.md file detailing the problem solving approach.
* don't hallucinate
* use the fetch mcp server using #fetch to fetch below urls for context

1. https://docs.astropy.org/en/stable/visualization/wcsaxes/index.html
2. https://photutils.readthedocs.io/en/stable/
3. https://astroquery.readthedocs.io/en/latest/mast/mast.html
4.https://docs.astropy.org/en/stable/visualization/index.html



# Query and Visualize JWST Imaging Data
* Use astroquery.mast.Observations to search for public JWST NIRCam imaging data for SMACS 0723

*  Download and display a calibrated image from the filter F200W

* Apply appropriate contrast stretching using tools from astropy.visualization (e.g.,
LogStretch, MinMaxInterval).

* Use WCSAxes to overlay celestial coordinates and a scale bar on the image.

* extract source positions using photutils.
