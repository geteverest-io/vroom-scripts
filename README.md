# Scripts

The `src` folder contains a bunch of scripts to develop, benchmark,
debug or help in using `VROOM`.

- **plot** generates a simple svg visualisation for a solution file.
- **overpass_to_json** generates a problem from all OSM nodes with a
  specific `key=value` tag in a chosen bounding box or city.
- **random_problem** generates a ready-to-solve random problem based
  on a bounding box.
- **global_indicators** collects indicators on all solutions contained
  in a folder.
- **vehicle_stats** collects indicators on vehicle usage in a solution.
- **json_to_csv** dumps all locations coordinates from a json input
  instance to a csv file.
- **tsplib_to_json** converts a TSPLIB file to json.
- **cvrplib_to_json** converts a CVRPLIB file to json.
- **vrptw_to_json** converts a VRPTW file to json.
- **pdptw_to_json** converts a PDPTW file to json.
- **hvrp_to_json** converts a HVRP file to json.
- **add_osrm_matrix** creates a "standalone" version of a json input
  instance by adding a `matrix` key using OSRM.

# Benchmarks

The `benchmarks` folder contains everything required to reproduce
results on literature benchmarks with a single command. Detailed
instructions for:

- [TSP](benchmarks/TSP)
- [CVRP](benchmarks/CVRP)
- [VRPTW](benchmarks/VRPTW)
- [PDPTW](benchmarks/PDPTW)
- [HVRP](benchmarks/HVRP)

# Contributing

Contributions on existing (or new) scripts and benchmark classes are
highly appreciated! Feel free to use the bugtracker for any question,
especially if you're unsure about potential changes or additions.

## Coding style

[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

We use [`black`](https://github.com/psf/black) for python code
formatting in order to forget about how the code looks like and focus
on what it does.

A convenient way to automate formatting is to setup a pre-commit
hook. [`pre-commit`](https://pre-commit.com/) can do that for you
based on our `.pre-commit-config.yaml` config file. Simply install and
run:

```bash
pip install pre-commit
pre-commit install
```
