# preCICE Doxygen Publisher

This repository is used to publish the doxygen documentation of the repository `precice/precice`.

## Manually update

1. Log in
2. Go to [this page](https://github.com/precice/doxygen/actions?query=workflow%3A%22Update+the+preCICE+doxygen%22)
3. At the top of the results list should be box:  
   `This workflow has a workflow_dispatch event trigger.`  
   Click the `Run workflow` and then `Run workflow`.

## How it works

The `deploy` workflow clones the master and develop branch of `precice/precice` and builds the doxygen documentation.
It then combines both `master/` and `develop/` docs with the [landing page](index.html) and deploys it to the `ph-pages` branch.
The latter is then accessible via [precice.org/doxygen](https://www.precice.org/doxygen/).
