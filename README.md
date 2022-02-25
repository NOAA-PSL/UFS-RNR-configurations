# Disclaimer

The United States Department of Commerce (DOC) GitHub project code is
provided on an "as is" basis and the user assumes responsibility for
its use. DOC has relinquished control of the information and no longer
has responsibility to protect the integrity, confidentiality, or
availability of the information. Any claims against the Department of
Commerce stemming from the use of its GitHub project will be governed
by all applicable Federal law. Any reference to specific commercial
products, processes, or services by service mark, trademark,
manufacturer, or otherwise, does not constitute or imply their
endorsement, recommendation or favoring by the Department of
Commerce. The Department of Commerce seal and logo, or the seal and
logo of a DOC bureau, shall not be used in any manner to imply
endorsement of any commercial product or activity by DOC or the United
States Government.

# Cloning

This repository contains configurations for each release of the
Unified Forecast System (UFS) Reanalysis and Reforecasting (RNR)
system which can be found [here](https://github.com/noaa-psd/UFS-RNR).
To obtain the entire UFS-RNR configuration archive, do:

~~~
user@host:$ git clone --recursive https://github.com/noaa-psd/UFS-RNR-configurations
~~~

# Configuration Archives

The directory tree for each respective UFS-RNR release configurations
follows that of the UFS-RNR workflow directory tree. For example, a
given directory tree for a single cycle of a 3DVAR weakly-coupled
UFS-RNR experiment would have the following structure.

~~~
├── forecast
│   └── cntrl
│       ├── history
│       ├── INPUT
│       ├── INPUT_NODA
│       ├── MOM6_OUTPUT
│       ├── RESTART
├── gsi
│   └── 3dvar
├── jedi
│   ├── soca
│   │   └── 3dvar
~~~

The configuration archives for the respective UFS-RNR releases follows
this similar logic. The archives are paritioned according to the
forecast model resolution and UFS forecast configuration (e.g.,
`coupled` or `uncoupled`). For example, a coupled UFS-RNR experiment
of cubed-sphere resolution C96 and using 64 unstaggered vertical
levels would be denoted as `C96L64/coupled`. The archive is then
further partitioned according to the UFS forecast type (i.e.,
`cold-start` or `warm-start`). All cold-start dates for the respective
configuration examples are relative to 0000 UTC 01 January 2016 while
the warm-start dates are relative to 0600 UTC 01 January 2016. Each
component of the UFS-RNR contains the respective configurtion files
used to the respective release baseline experiments. This includes the
input files, the YAML files (where relevant), and other necessary
input files required by the various UFS-RNR system applications.