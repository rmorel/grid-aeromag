# grid-aeromag
Gridding of brazilian aeromagnetometric data with Python

## Processing steps

1. [File format checking and geometry plot](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.1-rm-first-data-check.ipynb): This notebook previews the file format and create shapefiles with a light (simplified) version of the aeromagnétic survey geometry.

2. [Convert file format](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.2-rm-convert-data-format.ipynb): This notebook convert the decorrugated IGRF reduced magnetic anomaly flight and tie lines dataset to the NPY format for convenience.

3. [Check acquisiton geometry parameters](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.3-rm-acquisition-geometry-verification.ipynb): Basic checks of flight lines geometry.

4. [Data decimation](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.4-rm-data-decimation.ipynb): Decimate the data before gridding.

5. [Linear interpolation](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.5-rm-linear-interpolation.ipynb): Interpolate the decimated data using linear interpolation.

## License information
See the file [LICENSE](https://github.com/rmorel/grid-aeromag/blob/master/LICENSE) for information on terms & conditions for usage.
