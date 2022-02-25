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
UFS-RNR. To obtain the entire configuration archives, do:

~~~
user@host:$ git clone --recursive https://github.com/noaa-psd/UFS-RNR-configurations
~~~

# Configuration Archives

The directory tree for each UFS-RNR release configuration follows that
of the UFS-RNR workflow directory tree. For example, a given directory
tree for a single cycle of a 3DVAR weakly-coupled experiment would
have the following structure.

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

The configuration archive for the respective UFS-RNR releases follows
the same logic and contains the respective configuration (i.e., input
files, YAML files, etc.,) corresponding to the experiment type (e.g.,
coupled or uncoupled) and forecast type (e.g., cold-start or
warm-start).