# micrIO:
An open-source <ins>micro</ins>fluidic <ins>I</ins>nput-<ins>O</ins>utput platform comprising a specialized *autosampler* and *fraction collector*. 
The Python package to control micrIO (and other devices such as *pressure manifolds*, *MFCS units*, and *syringe pumps*) is provided in the pip-installable `acqpack` repository.

This repository contains supplemental information for `Longwell, S.A.; Fordyce, P.M. Lab on a Chip (2019).` It details how to assemble micrIO, as well as the experiment/data analysis used to validate the platform. 

Large files (videos, images) are included in the repository as `git lfs` pointers.

![Alt Text](overview.gif)

## `assembly/`
- **`parts-list.xlsx`**: Start here. Details parts needed for each sub-assembly, example sourcing for commercial parts, and links to view/download custom parts (3D-printed/laser-cut).
- **`parts/`**: Contains `.stl` files for 3D-printed parts and `.pdf` files for laser-cut parts (formatted for a Universal Laser Systems cutter). For other file formats, see links within `parts-list`. 
- **`assembly.mp4`**: Walk-around of micrIO (to aid in assembly).


## `validation/`
- **`run/`**
    + **`config/`**: The `.yaml` config files, frame transformations, and platemaps.
    + **`run.ipynb`**: The notebook used to script/record production of spectrally encoded beads.
    + **`log/`**: Log files produced from the run. 
    + **`validation.mp4`**: Shows micrIO integrated into a setup to perform the validation experiment.
- **`analysis/`**
    + **`images/`**: Images of beads produced from the validation run. There are 4-channels (*brightfield*, *Dy: 572 nm*, *Eu: 620 nm*, *Sm: 650*).
    + **`bead_analysis.ipynb`**: Image analysis pipeline used to identify beads and generate size and channel intensity statistics.overview.gif
[overview.gif]: 
