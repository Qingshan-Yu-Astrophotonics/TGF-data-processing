GammaFlashSim Batch Run Notes
=============================

Auto-generated from run/flash_batch.mac
Generated at: 2026-02-05 00:21:55

Key Parameters
--------------
/tgf/sourceZ 900 m
/tgf/beamHalfAngle 15 deg
/tgf/Ec 7.3 MeV
/tgf/Emin 0.2 MeV
/tgf/Emax 10 MeV
/tgf/nPhotonsPerEvent 10000000
/run/beamOn 1

Timing / Burst
--------------
/tgf/pulseWidth 200000 ns
/tgf/useBurstProfile true
/tgf/impulseFrac 0.01
/tgf/tailTau 10000 ns
/tgf/nBunches 1
/tgf/bunchSpacing 0 ns

Output
------
/tgf/output/fileName tgf
/tgf/output/fileType root
/tgf/output/timeMin 0 ns
/tgf/output/timeMax 10000 ns
/tgf/output/timeBins 1000

Geometry / Atmosphere
---------------------
/tgf/geom/atmNLayers 10
/tgf/geom/atmLayerThickness 1000 m
/tgf/geom/numArrays 1
/tgf/geom/scoringPlaneZ 80 mm
/tgf/geom/humidityVolFrac 0.025
/tgf/geom/humidityTopZ 1 km
/tgf/geom/aerosolPM25 20
/tgf/geom/aerosolPM10 35
/tgf/geom/aerosolTopZ 1 km

ROI / Bias
----------
/tgf/bias/enable true
/tgf/bias/roiPlaneZ 0 m
/tgf/bias/roiRadius 0.10 m
/tgf/bias/verbose true

Digitizer
---------
/tgf/digi/sigma0 0.024 MeV
/tgf/digi/triggerThreshold 0.2 MeV
