# grid-aeromag

This repository is a example on how to grid real aerogeophysical data using python. As an example, I'll be using the magnetometric survey "1113 - Projeto Aerogeofísico Sudeste do Mato Grosso" made by the Geological Survey of Brazil, or simply [CPRM](https://www.cprm.gov.br/en/), which is the acronym for the company's official name in Portuguese.

This data is quite big, in both size, area and number of data points. Because of that, it reflects a good real use case. All the code was done thinking on a real use, so any desktop PC should run this workflow without problems. The [notebooks](https://github.com/rmorel/grid-aeromag/tree/master/notebooks) have run time measurements for the most work intensive tasks. Either way, the heaviest tasks (file conversions) do not take more than 3-4 minutes. From data conversion to final interpolation, this workflow takes 7-10 minutes at most.

## Processing steps

1. [File format checking and geometry plot](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.1-rm-first-data-check.ipynb): This notebook previews the file format and create shapefiles with a light (simplified) version of the aeromagnétic survey geometry.

2. [Convert file format](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.2-rm-convert-data-format.ipynb): This notebook convert the decorrugated IGRF reduced magnetic anomaly flight and tie lines dataset to the NPY format for convenience.

3. [Check acquisiton geometry parameters](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.3-rm-acquisition-geometry-verification.ipynb): Basic checks of flight lines geometry.

4. [Data decimation](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.4-rm-data-decimation.ipynb): Decimate the data before gridding.

5. [Linear interpolation](https://github.com/rmorel/grid-aeromag/blob/master/notebooks/0.5-rm-linear-interpolation.ipynb): Interpolate the decimated data using linear interpolation.

## License information
See the file [LICENSE](https://github.com/rmorel/grid-aeromag/blob/master/LICENSE) for information on terms & conditions for usage.
