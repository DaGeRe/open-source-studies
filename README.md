This repository contains the data of analysis of open source repositories with Peass.

Each folder could either be results of a project or results of a specific configuration of a project (e.g. range of commits or measurement configuration). It should contain the following subfolders:
- `results/` with the regression test selection results
- `measurement-results/` with the measurement data (measurementsFull-folder) and `changes.json` and `statistics.json`
- `rca-results/` with the root cause analysis data (`treeMeasurementResults`-folder and `run-rca-$project.sh`)
- `run-$project.sh`, which contains the execution script for the measurement

When this structure is used, metadata of the measurement can be obtained by executing `./analyzeRTS.sh` (list of folders that should be analyzed should be defined in the file).
