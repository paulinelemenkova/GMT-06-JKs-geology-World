# GMT Geology World — Global Geological Features Map

GMT (Generic Mapping Tools) shell scripts that draw a world map of major geological and tectonic features on an equal-area global projection. The scripts overlay hotspots, plate-margin structures, magmatic provinces and volcanoes on a coastline base, with a full legend. They have been used to generate global geological map figures in the author's geoscientific and cartographic publications.

## What the scripts map

- Hotspots (psxy)
- Mid-ocean ridges, transform faults and subduction trenches, drawn with directional front symbols (psxy -Sf)
- Ophiolites (psxy)
- Volcanoes (psxy)
- Large Igneous Provinces (LIPs) as filled polygons plus point locations (psxy)
- Coastlines, grid, scale bar, legend and GMT logo (pscoast, psbasemap, pslegend, logo)

Two variants are provided using the Eckert equal-area pseudocylindrical projection (Eckert VI / Eckert IV), centred on the Pacific at 180 degrees.

## Data sources

Global tectonic and geological vector datasets bundled with / used by GMT and community sources: hotspots, ridge / transform / trench lines, ophiolites, volcanoes, and the LIPs (Large Igneous Provinces) compilations. Coastlines from GSHHG via GMT.

## Files

- GMT-06-script-JKs-geology-World.sh: Eckert VI (JKs) variant
- GMT-06-script-JW-geology-World.sh: alternative projection variant

## Requirements

- GMT 6.x (Generic Mapping Tools): https://www.generic-mapping-tools.org
- A POSIX shell (bash/sh)
- The geological vector data files (hotspots, ridges, trenches, transforms, ophiolites, volcanoes, LIPs) available locally

## Usage

Place the required geological vector files in the working directory, then run:

    bash GMT-06-script-JKs-geology-World.sh

The script writes a PostScript file and converts it to a raster image (JPG/PNG) via psconvert.

## Author and citation

Polina Lemenkova
ORCID: https://orcid.org/0000-0002-5759-1089

These scripts support figures in the author's geoscientific and cartographic papers; please cite the specific article a given figure appears in. The full publication list is available via the ORCID record above.

## License

See the LICENSE file in this repository.
