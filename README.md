# `kerchunk` GOES-16/17 Tutorial: Faster Cloud Data Access

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lsterzinger/kerchunk-medium-tutorial/HEAD?labpath=tutorial.ipynb)

## Overview

This repository provides a hands-on tutorial demonstrating the power of [kerchunk](https://github.com/fsspec/kerchunk) for accelerating access to GOES-16/17 NetCDF4 datasets hosted on AWS S3.

By creating lightweight index files (`kerchunk` references), we can treat collections of NetCDF files as a single, virtual Zarr dataset, enabling significantly faster and more scalable data analysis workflows with tools like Xarray.

This tutorial accompanies a blog post on Medium (link forthcoming) that delves deeper into the concepts.

## The Tutorial Notebook (`tutorial.ipynb`)

The main content is within the `tutorial.ipynb` Jupyter Notebook. It covers:

1.  Setting up the required Python environment.
2.  Generating `kerchunk` index files for sample GOES-16 data.
3.  Using `fsspec` and `xarray` to open the virtual dataset from the generated index.
4.  Demonstrating the performance benefits.