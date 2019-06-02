# Interim data files

This folder contains interim data files created by this project.

1. MAGIGRF.npy: decorrugated IGRF reduced magnetic field anomaly in NPY format. Converted from the original dataset by running [notebooks/0.2-rm-convert-data-format.ipynb](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.2-rm-convert-data-format.ipynb).

2. MAGIGRF_DECIMATED_150x150m.npy: Decimated IGRF reduced magnetic field anomaly in NPY format. Decimation was done using means on 150 x 150 meter cells, x and y coordinates are at the center of each cell. Created by running [notebooks/0.4-rm-data-decimation.ipynb](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.4-rm-data-decimation.ipynb).
