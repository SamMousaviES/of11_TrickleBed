# Trickle Bed Modeling Using OpenFOAM 11

This GitHub repository hosts simulation cases for the modeling of trickle bed reactors using OpenFOAM 11, which is a widely recognized open-source platform for computational fluid dynamics (CFD). The aim of this project is to explore various scenarios and incorporate enhancements into the simulation of trickle beds, making full use of the extensive functionalities and customizations that OpenFOAM 11 offers.

The organization of the cases is meticulous, with each folder name indicating the specific nature and developmental stage of the simulation case. This structured setup ensures transparency and ease of navigation through different stages of the project development.

## Getting Started

Begin by installing OpenFOAM, and then proceed to download the specific simulation case that fits your project needs.

### Prerequisites

The following tools and software are required to build, test, and execute the simulations:
- [OpenFoam 11](https://openfoam.org/version/11/)

## Running the Tests

To execute the cases, use the provided `Allrun` script within each case folder. Run the following commands based on your processor configuration:
./Allrun
- For single processor simulations:
foamRun

- For multi-processor simulations (default is set to use 20 processes):
mpirun -np 20 foamRun -parallel

## Versioning

The versions of the cases are structured to guide the user from basic to advanced implementations:

bedV00_original: Adapted from the OpenFOAM 11 tutorial, this serves as the baseline case.
bedV01ErgunRealSizeBed: Utilizes built-in Ergun drag formulations with precisely defined geometries to match real dimensions.
bedV02MomentumSource_NoSources: A template-like case designed for the incorporation of source terms.
bedV03MomentumSource: Features explicitly defined source terms using the fvModels file, ideal for further development and integration of complex physical phenomena.

## Authors

  - **Sam Mousavi**
    [PurpleBooth](https://github.com/SamMousaviES)


