# duplex_bead_model
Data extraction and example files for coarse-grained DNA/RNA folding model

# Requirements
* The newest version of [oxDNA_analysis_tools](https://github.com/sulcgroup/oxdna_analysis_tools) (you need to clone from github and run `python -m pip install .`).
* numpy

# Usage
Set the directory of the structure you would like to coarse-grain in the `dirname` variable of `get_viz.ipynb` and then run all cells

This will generate a couple different visualization/simulation options.  First is an xyz file that contains the centers of mass for the individual domains.
These files are terrible for visualization (and require a hacked version of oxView anyway) but might be useful for model generation.
The second file is a regular oxDNA file with just the median base pair in each helix (rounded down on the lower indexed strand in the oxDNA file in the case of even-length strands). 
This also comes with some oxView instructions for generating pretty images overlaying this file on the original mean structure.
<p float="center">
  <img src="/ico/beads.png" width="45%" />
  <img src="/ico/overlay.png" width="45%" /> 
</p>
