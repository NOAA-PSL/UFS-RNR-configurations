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
system which can be found here. To obtain the UFS-RNR configuration
archive for a specific UFS-RNR release, do:

~~~
user@host:$ git clone --branch release/ufsrnr.v### https://github.com/noaa-psd/UFS-RNR-configurations
~~~

where `release/ufsrnr.v###` is the respective UFS-RNR release against
which to compare. Note that the latest UFS-RNR `develop` branch
configuration will be that contained in the `develop` branch of this
repository.

# Configuration Archives

The archives are paritioned according to the forecast model resolution
and UFS forecast configuration (e.g., `coupled` or `uncoupled`). For
example, a coupled UFS-RNR experiment of cubed-sphere resolution C96
and using 127 unstaggered vertical levels would be denoted as
`C96L127/coupled`. The archive is then further partitioned according to
the UFS forecast type (i.e., `cold-start` or `warm-start`). All
cold-start dates for the respective configuration examples are
relative to 0000 UTC 01 January 2016 while the warm-start dates are
relative to 0600 UTC 01 January 2016. Each component of the UFS-RNR
contains the respective configuration files used to the respective
release baseline experiments. This includes the input files, the YAML
files (where relevant), and other necessary input files required by
the various UFS-RNR system applications.

# UFS-RNR Application Branches and Tags

The following table specifies the respective applications and the
corresponding tags/hashes valid for the UFS-RNR v2.0 configurations.



<div align="center">

| Application | <div align="center">[GSI](https://github.com/jswhit/GSI)</div> | <div align="center">[UFS](https://github.com/ufs-community/ufs-weather-model)</div> | <div align="center">[UFS-RNR](https://github.com/noaa-psd/UFS-RNR)</div> | <div align="center">[SOCA-science](https://github.com/JCSDA-internal/soca-science)</div> |
| :-------------: | :-----------: | | :-------------: | :-----------: | | :-------------: |
| Tag | `750de32` | `b26a896` | `06747e5` | `9dce8a7` |

</div>