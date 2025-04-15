# Dry-Soil-Detection
Dry soil refers to soil that has a low moisture content—meaning it lacks sufficient water in its pores to support healthy plant growth or maintain its structure.

# Dry Soil Detection using Sentinel-2 Data

🛰️ Sentinel-2 Overview
Sentinel-2 is part of the European Space Agency’s Copernicus program. It provides high-resolution optical imagery with a 5-day revisit cycle, useful for land surface monitoring, including vegetation, water bodies, and soil conditions.

Spatial Resolution: 10m to 60m depending on band

Revisit Frequency: ~5 days

Bands Used in Dry Soil Analysis:

B2 (Blue, 490 nm – 10m)

B4 (Red, 665 nm – 10m)

B5 (SWIR1, 705 nm – 20m)

# In your code, you used bands B2, B4, and B5 to compute dry soil areas.

# Dry Soil Detection Logic

The detection is based on the spectral behavior of dry soil:

Dry soil tends to reflect more strongly in the SWIR band (B5).

It also shApplied Condition:ows moderate reflectance in the red and blue wavelengths.


# Applied Condition:
js
Copy
Edit
swir1 > blue && red > 0.05
This implies:

Soil is relatively dry if its SWIR reflectance is greater than blue reflectance.

The red band threshold ensures that vegetated or saturated surfaces are excluded.

# Why Sentinel-2 for Dry Soil Monitoring?

High temporal resolution (5 days): Allows for near real-time monitoring.

High spatial resolution (10m–20m): Ideal for capturing small-scale soil moisture variations.

Multispectral capabilities: Covers key bands for soil and vegetation differentiation.

# Time Series Analysis

Tracking the mean dry soil index over time helps:

Monitor drought patterns.

Support agricultural planning and irrigation management.

Understand land surface response to rainfall or seasonal changes.


# Applications

Agricultural drought monitoring

Land degradation assessment

Soil moisture pattern mapping

Irrigation management support

Would you like a visual infographic or slide version of this summary? I can also help you write a report or presentation based on it.


# Refarances PDF 
https://www.researchgate.net/profile/Jianhua-Zhang-35/publication/234836983_Root_Signals_and_the_Regulation_of_Growth_and_Development_of_Plants_in_Drying_Soil/links/59379228aca272ede1cb3cb5/Root-Signals-and-the-Regulation-of-Growth-and-Development-of-Plants-in-Drying-Soil.pdf?__cf_chl_tk=UG7jpOzXRB1bQb66u3ZUiTJDNeRn4mmQIx1oAdjWIqI-1744688597-1.0.1.1-iG4j9y83YLZJMv122nt_s5WBkMMGd0P7VWiS5gzRKwk

# Contact

For questions, suggestions, or collaborations:

📧 tejaskchavan22@gmail.com +91 7378423157
