# Radi Ajjaji

Numerical Weather Prediction | Data Assimilation | HPC | AI Weather Models

I work on research and development around atmospheric modelling,
numerical weather prediction, data assimilation, high-performance
computing, and AI-based weather forecasting.

## Featured Research & Development

### Operational MPAS-Atmosphere 8.0 System

I developed and operationally integrated a dust-enabled
MPAS-Atmosphere 8.0 forecasting system together with its complete
HPC, conversion and post-processing workflow.

Major developments include:

- substantial redevelopment of the MPAS dust capability for the
  MPAS 8.0 code structure;
- native handling of the dust erodibility field (`erod`) in
  `init_atmosphere`;
- operational GOCART dust and aerosol configuration;
- native MPAS-to-WRF global remapping using an extended `metgrid`;
- generalized support for native MPAS atmospheric fields;
- Parallel-NetCDF support in `metgrid` through `io_form = 11`
  and `IO_PNETCDF`;
- an extended UPP 4.1 workflow for processing the resulting global
  WRF-format fields;
- global GRIB production for GrADS, NCL and downstream operational
  processing;
- GeoJSON, polygon, isoband and MBTiles generation for operational
  visualization.

The global interoperability chain is:

    Native MPAS forecast
            |
            v
    MPAS-aware modified metgrid
            |
            | Parallel-NetCDF / io_form=11
            v
    Global WRF lat/lon representation
            |
            v
    Extended UPP 4.1
            |
            v
    Global GRIB / operational products

[View the operational MPAS system](https://github.com/radiajjaji/mpas-operational)

### MPAS-JEDI Native-MPAS B-Matrix Workflows

I successfully developed and operationally integrated
MPAS-JEDI/SABER background-error covariance workflows derived
directly from native MPAS-Atmosphere forecast data.

The methodology has been implemented at:

- **12 km** — successfully generated and operationally used;
- **24 km** — successfully generated;
- **30 km** — successfully generated.

The workflows include:

- VBAL;
- HDIAGS;
- NICAS;
- BUMP localization.

The covariance-training data originate from native MPAS forecasts,
without requiring conversion from another numerical weather
prediction model.

[View the MPAS-JEDI tools and B-matrix workflows](https://github.com/radiajjaji/mpas-jedi-tools)

## Research & Development

### MPAS / MPAS-JEDI
- MPAS model workflows and utilities
- MPAS-JEDI data assimilation
- SABER / BUMP / NICAS
- Mesh conversion and remapping
- State conversion and diagnostics

### WRF / WRFDA
- Operational WRF workflows
- WRFDA and FGAT
- HPC optimization
- Parallel I/O and domain decomposition
- Forecast post-processing utilities

### GSI
- GSI data assimilation workflows
- Observation processing
- Diagnostic tools
- Radiance assimilation utilities

### AI Weather Models
- ECMWF AIFS
- GraphCast
- PanguWeather
- NeuralGCM
- AI model integration and evaluation

### High-Performance Computing
- HPE Cray systems
- MPI and Slurm
- Parallel I/O
- Numerical model performance optimization
- Large-scale operational forecasting workflows

## Current Focus

My current development work focuses primarily on MPAS,
MPAS-JEDI, data assimilation, high-performance numerical weather
prediction, and the integration of AI weather models into
operational forecasting environments.

## Professional Profile

[LinkedIn](https://www.linkedin.com/in/radi-ajjaji-10008071)
