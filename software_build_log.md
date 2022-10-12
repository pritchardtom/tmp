# Software Install Log

| Software       | Version | Date Installed | Available as Module | Availability | Notes                                                       |
|:--------------:|:-------:|:--------------:|:-------------------:|:------------:|:------------------------------------------------------------|
| `Matlab`       | 2022a   | 03/05/2022     | Yes                 | Sunbird      |                                                             |
| `GNU GCC`      | 11.3.0  | 13/06/2022     | Yes                 | Hawk/Sunbird |                                                             |
| `GNU GCC`      | 12.1.0  | 14/06/2022     | Yes                 | Hawk/Sunbird |                                                             |
| `openMPI`      | 3.1.5   | 20/06/2022     | Yes                 | Hawk/Sunbird | Recompile job for GCC 12.  Still need to do `AVX2` version. |
| `GSL`          | 2.6     | 20/06/2022     | Yes                 | Hawk/Sunbird | Recompile job for GCC 12.  Still need to do for GCC 11      |
| `CellProfiler` | 4.2.1   | 21/06/2022     | Yes (22/06/2022)    | Sunbird      | Singularity container.                                      |
| `Eigen`        | 3.4.0   | 21/06/2022     | Yes                 | Hawk/Sunbird |                                                             |
| `FFTW`         | 3.3.10  | 21/06/2022     | Not yet             | Sunbird      | Local install for JJ Lenz.  Will provide system ones soon.  |
| `GMP`          | 6.2.1   | 21/06/2022     | Not yet             | Sunbird      | Local install for JJ Lenz.  Will provide system ones soon.  |
| `MPFR`         | 4.1.0   | 21/06/2022     | Not yet             | Sunbird      | Local install for JJ Lenz.  Will provide system ones soon.  |
| `Boost`        | 1.79.0  | 22/06/2022     | Not yet             | Sunbird      | Local install for JJ Lenz.  Will provide system ones soon.  |
| `Go`           | 1.18.3  | 23/06/2022     | Yes                 | Hawk/Sunbird | Dependecy for `Apptainer`.                                  |
| `Apptainer`    | 1.0.3   | 23/06/2022     | Yes                 | Sunbird      |                                                             |
| `CMake`        | 3.24.2  | 25/09/2022     | Yes                 | Sunbird      |                                                             |
| `OpenMPI`      | 4.1.1   | 26/09/2022     | Yes                 | Hawk/Sunbird | rsync from Hawk (GNU 9 only) bur needed for dependency.     |
| `ORCA`         | 5.0.3   | 26/09/2022     | Yes                 | Sunbird      | ACLs set                                                    |
| `Mamba`        | 4.14.0.0| 26/09/2022     | Yes                 | Sunbird      |                                                             |
| `Udunits`      | 2.2.28  | 30/09/2022     | No                  | Sunbird      | Installed as dependency.  Module tested but removed until needed. |
| `SQLite`       | 3390400 | 30/09/2022     | Yes                 | Sunbird      |                                                                   |
| `Proj`         | 9.1.0   | 30/09/2022     | Yes                 | Sunbird      | GNU only - Intel being annoying                                   |
| `Geos`         | 3.11.0  | 30/09/2022     | Yes                 | Sunbird      | GNU only - Intel being annoying                                   |
