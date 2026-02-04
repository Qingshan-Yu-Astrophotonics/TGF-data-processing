GammaFlashSim Batch Run Notes
=============================

This folder stores runtime outputs generated from flash_batch.mac.

Key Parameters (from run/flash_batch.mac)
-----------------------------------------
- Source altitude: /tgf/sourceZ 900 m
- Beam half angle: /tgf/beamHalfAngle 15 deg
- Source spectrum:
  - /tgf/Ec   7.3 MeV
  - /tgf/Emin 0.2 MeV
  - /tgf/Emax 20 MeV
- Photons per event: /tgf/nPhotonsPerEvent 10000000
- Number of events: /run/beamOn 1

Timing / Burst Shape
--------------------
- /tgf/pulseWidth 200000 ns
- /tgf/useBurstProfile true
- /tgf/impulseFrac 0.01
- /tgf/tailTau 10000 ns
- /tgf/nBunches 1
- /tgf/bunchSpacing 0 ns

Time-resolved Output Settings
-----------------------------
- /tgf/output/timeMin 0 ns
- /tgf/output/timeMax 50000 ns
- /tgf/output/timeBins 10000
- Time bin width = (timeMax - timeMin) / timeBins = 5 ns

Geometry / Atmosphere
---------------------
- /tgf/geom/atmNLayers 10
- /tgf/geom/atmLayerThickness 1000 m
- Total atmosphere height = 10 km
- /tgf/geom/scoringPlaneZ 80 mm

Coastal atmosphere approximation:
- /tgf/geom/humidityVolFrac 0.025
- /tgf/geom/humidityTopZ 1 km
- /tgf/geom/aerosolPM25 20 (ug/m3)
- /tgf/geom/aerosolPM10 35 (ug/m3)
- /tgf/geom/aerosolTopZ 1 km

ROI Bias (importance sampling)
------------------------------
- /tgf/bias/enable true
- /tgf/bias/roiPlaneZ 0 m
- /tgf/bias/roiRadius 0.10 m
- /tgf/bias/verbose true

Digitizer / Trigger
-------------------
- /tgf/digi/sigma0 0.024 MeV
- /tgf/digi/triggerThreshold 0.2 MeV

Output files
------------
- Main output base name: /tgf/output/fileName tgf
- File type: /tgf/output/fileType root
- Additional CSV matrices may be generated:
  - tgf_srcE_t_matrix.csv
  - tgf_detE_t_matrix.csv

Recommended to record for reproducibility
-----------------------------------------
- Geant4 version and build type
- Number of threads used (MT settings)
- Commit hash / code revision
- Exact macro file used for the run
