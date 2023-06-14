# EarthByte Model

This model is imported from the *EarthByte* model,
that is the default model included in [GPlates](https://www.gplates.org/).
The original model can be downloaded
from the [EarthByte page](https://www.earthbyte.org/gplates-2-3-software-and-data-sets/).

## Time frame

The rotations are defined from 400 million years
(up to 410 for the plate motion model)
to today,
in time stages of 5 million years.

## Pixelation

The model is available in three resolutions:
e360 (360 pixels in the equatorial ring),
e180,
and e120.

## File descriptions

All the files are prefixed as `earthbyte-*`
usually followed by the pixelation resolution,
the size of time step,
and the kind of file.

### Pixelated features

It is based on the continental polygons
from the original EarthByte model,
extended with the volcanic provinces from Johansson et al. (2018).
It is stored in the file `earthbyte-pixels-xxx.tab`
in which `xxx` is used to indicate the resolution.

### Plate motion model

The plate motion model
(or rotation model)
was the model compiled by the EarthByte group,
and the main references are:
Torsvik et al. (2019),
Young et al. (2019),
Müller et al. (2019),
Cao et al. (2022).
See that papers for additional references of the different rotations.

The model is stored in the file `earthbyte-motion-xxx-5.tab`,
in which `xxx` is the pixel resolution,
and 5 is the time resolution (in million years).

### Paleolandscape

The 'ocean plateau' layers are just the tectonic features
pixelated at each time.
Other layers were prepared from the paleogeography model
of Cao et al. (2017),
that can be found at [EarthByte page](https://www.earthbyte.org/gplates-2-3-software-and-data-sets/).
Layers at present time are derived
from [NaturalEarth](https://www.naturalearthdata.com/)
and [NaturalEarth III](https://www.shadedrelief.com/natural3/index.html).
The landscape model uses the following convention:

Key | Environment
--- | -----------
  1 | oceanic plateaus
  2 | continental shelf
  3 | lowlands
  4 | highlands
  5 | ice sheets

The model is stored in the file `earthbyte-landscape-cao-xxx-5.tab`,
in which `xxx` is the pixel resolution,
and 5 is the time resolution (in million years).

A color key,
which is compatible with color-blindness,
and can be used with `plates timepix map` command
is stored in the file `earthbyte-landscape-cao-key.tab`.

## Citation and data license

This model is the direct process of the
Cao et al. (2017),
Torsvik et al. (2019),
Young et al. (2019),
Müller et al. (2019),
and Cao et al. (2022) models.
As such,
the original publications should be cited when the model is used.
Relevant papers are given in this file
and provided as bibTeX.

It is not required to cite this repository,
but if you do not include the model in the supplementary material
of your publication,
it might be a good idea to link this repository
and help others to replicate or re-use your analysis.

## References

Cao, W. et al.
(2017)
Improving global paleogeography since the late Paleozoic using paleobiology.
Biogeosciences, 14, 5425-5439.
DOI: [10.5194/bg-14-5425-2017](https://doi.org/10.5194/bg-14-5425-2017).

Cao, X. et al.
(2022).
A deforming plate tectonic model of the South China Block since the Jurassic.
Gondwana Research, 102, 3-16.
DOI: [10.1016/j.gr.2020.11.010](https://doi.org/10.1016/j.gr.2020.11.010).

Johansson, L., Zahirovic, S., & Müller, R. D.
(2018).
The interplay between the eruption and weathering of large igneous provinces and the deep‐time carbon cycle.
Geophysical Research Letters, 45, 5380-5389.
DOI: [10.1029/2017GL076691](https://doi.org/10.1029/2017GL076691).

Müller, R. D. et al.
(2019).
A global plate model including lithospheric deformation along major rifts and orogens since the Triassic.
Tectonics, 38, 1884-1907.
DOI: [10.1029/2018TC005462](https://doi.org/10.1029/2018TC005462).

Torsvik, T. H. et al.
(2019).
Pacific‐Panthalassic reconstructions: Overview, errata and the way forward.
Geochemistry, Geophysics, Geosystems, 20, 3659-3689.
DOI: [10.1029/2019GC008402](https://doi.org/10.1029/2019GC008402).

Young, A. et al.
(2019).
Global kinematics of tectonic plates and subduction zones since the late Paleozoic Era. Geoscience Frontiers, 10, 989-1013.
DOI: [10.1016/j.gsf.2018.05.011](https://doi.org/10.1016/j.gsf.2018.05.011).
