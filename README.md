# Phase-field Serpentinization #

This repository contains supplementary [*TerraFERMA*](http://terraferma.github.io) model files to accompany the paper

>Evans, O., Spiegelman, M., Kelemen, P.B.,
*Exploring Feedbacks in a Model of Reaction-Driven Cracking*, submitted to JGR-Solid Earth

### Contents ###
This repository contains the following directories:

* **models:** Directories containing input files for describing and running the models used in this manuscript.
* **meshes:** gmsh input files used in the models

### Running the Models ###

* **Install TerraFERMA:** To view and run these models will require building and installing the open source code [*TerraFERMA*](http://terraferma.github.io).

* **Running Models:** If the software is installed successfully the models can be run from within each subdirectory using

```
$ tfsimulationharness --test <filename>.shml
```

where `<filename>.shml` is the name of the *simulation harness* file that controls parameter sweeps and parallelization options. Models are described (boundary/initial conditions, timesteppers, weak forms, solvers etc.) in the *TerraFERMA* markup language files with suffix `.tfml`.

* **Viewing Input files:**  both `.tfml` and `.shml` files can be viewed and changed using the `diamond` GUI with

```
$ diamond <filename>.tfml
```
