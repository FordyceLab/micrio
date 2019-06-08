[Simple Project Download via OSF \[2 GB\]](https://osf.io/86wf5/?view_only=c3bfd653adfa457480bd9e34eeaa98bf) (click: Google Drive > Download as zip)

# micrIO:
An open-source <ins>micro</ins>fluidic <ins>I</ins>nput-<ins>O</ins>utput platform comprising a specialized *autosampler* and *fraction collector*. 

This repository contains supplemental information for [`S.A. Longwell and P.M. Fordyce (under review)`](https://www.biorxiv.org/content/10.1101/655324v1). It details how to assemble micrIO, as well as the experiment/data analysis used to validate the platform. 

The Python software to control micrIO (and other devices such as *pressure manifolds*, *MFCS units*, and *syringe pumps*) is available as our pip-installable [`acqpack`](https://pypi.org/project/acqpack/) package (documentation [here](https://acqpack.readthedocs.io/en/latest/)).

Large files (videos, images) are included in the repository via git-lfs, which must be installed to have these files clone properly. Downloading the `.zip` from here will not include working versions of these files. (See [OSF: Google Drive](https://osf.io/86wf5/?view_only=c3bfd653adfa457480bd9e34eeaa98bf) mirror for easy viewing / downloading of these files).

[Full CAD Link](https://a360.co/2IcW9vt)

[![micrIO CAD](overview.gif)](https://a360.co/2IcW9vt)

## [`assembly/`](https://github.com/FordyceLab/micrio/tree/master/assembly)
- [**`parts-list.gsheet`**](https://docs.google.com/spreadsheets/d/17_JYHVy769XvpJGD3QiEPhoSL2Djqnr2_NVfNIwoY9A/edit?usp=sharing) Start here. Details parts needed for each sub-assembly, example sourcing for commercial parts, and links to view/download custom parts (3D-printed/laser-cut).
- [**`parts/`**](https://github.com/FordyceLab/micrio/tree/master/assembly/parts) Contains `.stl` files for 3D-printed parts and `.pdf` files for laser-cut parts (formatted for a Universal Laser Systems cutter). For other file formats, see links within `parts-list.gsheet`. 
- [**`assembly.mp4`**](https://osf.io/6a3vq/?view_only=c3bfd653adfa457480bd9e34eeaa98bf) Walk-around of micrIO (to aid in assembly).


## [`validation/`](https://github.com/FordyceLab/micrio/tree/master/validation)
- [**`run/`**](https://github.com/FordyceLab/micrio/tree/master/validation/run)
    + [**`config/`**](https://github.com/FordyceLab/micrio/tree/master/validation/run/config) The `.yaml` config files, frame transformations, and platemaps.
    + [**`run.ipynb`**](https://github.com/FordyceLab/micrio/blob/master/validation/run/run.ipynb) The notebook used to script/record production of spectrally encoded beads.
    + [**`log/`**](https://github.com/FordyceLab/micrio/tree/master/validation/run/log) Log files produced from the run. 
    + [**`validation.mp4`**](https://osf.io/ydbtc/?view_only=c3bfd653adfa457480bd9e34eeaa98bf) Shows micrIO integrated into a setup to perform the validation experiment.
- [**`analysis/`**](https://github.com/FordyceLab/micrio/tree/master/validation/analysis)
    + **`images/`** Images of beads produced from the validation run. There are 10 channels, 4 of which were used in the manuscript's analysis (*brightfield*, *Dy: 572 nm*, *Eu: 620 nm*, *Sm: 650*).
    + [**`bead_analysis.ipynb`**](https://github.com/FordyceLab/micrio/blob/master/validation/analysis/bead_analysis.ipynb) Image analysis pipeline used to identify beads and generate size and channel intensity figures and statistics.
    
