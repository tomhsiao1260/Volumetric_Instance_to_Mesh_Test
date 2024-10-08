## Introduction

Generate `.obj` mesh from a given `.nrrd` mask. The source is from [here](https://github.com/JamesDarby345/Volumetric_Instance_to_Mesh).

## Install

`pip install -r requirements.txt`

## Download

Create a folder called `data` in root directory and put the corresponding `mask.nrrd` and `volume.nrrd` with the following structure.

```
.
└── data
    └── 10624_02304_02432
        ├── 10624_02304_02432_mask.nrrd
        └── 10624_02304_02432_volume.nrrd
```

## Run

Turn a given mask into 1 voxel thickness (`fb_avg_mask_thinned.nrrd`).

`python fb_avg_3d_instance_to_midline_volume.py`

Once finished, generate the `.obj` with the following command.

`python midline_to_obj.py`