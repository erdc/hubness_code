# Hubness Code

In the real world, many projects end up being only partially completed. In projects where a subset of a set of need to be selected, this creates challenging resilience problem: given that not all of the planned set will be constructed, which should you build and in what order to maintain the greatest functionality. To solve this callenge, we developed the hubness metic. For more detailed infromation on please consult the corresponding paper:

This repository contains code used to generate the examples shown in this paper.

## Requirements and Installation

This project uses conda environments to manage dependencies. This environment can be created using the command:

``` conda env create --name hubness_code --file=env.yml ```

## Additional Project Resources and Files

The data files for the project are too big to push via github so they are can be found in the project googledrive. Additionally, documents including project presentations, task lists and saved documents resources (such as saved papers) will all be located it this folder as well. These resources can be found at:

https://drive.google.com/drive/folders/1ZsvbWJA5_4pgqf9oQ1ZK2Bdjq9Msw1Ve?usp=sharing

## Project Point of Contact

If you have any questions about either running this project or the project in general, feel free to contact Kelsey Stoddard at:
```kelsey.s.stodard@gmail.com```

## Project Structure
###

```
├── README.md          <- The top-level README for developers using this project (this file).
│
├── data
│   ├── raw*           <- A local cache of data loaded directly from a raw data source
│   │   ├── maxar*     <- Raw data downloaded from MAXAR.
│   │   │   ├── carmel*         <- MAXAR data from the Carmel River fires.
│   │   │   │   ├── post_swir*     <- Post-event swir images
│   │   │   │   ├── post_visible*  <- Post-event visibe light images.
│   │   │   │   └── pre_visible*   <- Pre-event visible light images.
│   │   │   └── santa_rosa*     <- MAXAR data from the Santa Rosa fires.
│   │   ├── drone*     <- Raw drone data. (currently unused)
│   │   └── sentinal2* <- Raw Sentinal2 data. (currently unused)
│   ├── formatted*     <- Output data that has been processed by code and tools in this project
│   └── supplemental   <- Extra data files expected by processing or visualization code
│
├── notebooks          <- Jupyter notebooks
│   ├── analysis       <- Notebooks used to explore data before a consise analysis question or explore results
│   │   └── base_env.txt    <- Conda environment file with the requirements to run analysis notebooks
│   ├── gdal           <- Notebooks and code that requires gdal to perform geospatial transformations
│   │   └── gdal_env.txt    <- Conda environment file with the requirements to run gdal notebooks
│   └── archive        <- OBE which we wanted save but are no longer in use. Name analysis_* or gdal_* for env
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   ├── plots          <- Generated graphics and figures to be used in reporting 
│   └── model_parameters  <- Model generation and test performance results
│
├── models             <- Saved generated models and model generation reports (currently empty)
│
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   └── img_transform  <- Code to perform geospatial transforms on images.

```

`* Asterisk` indicates a directory's contents is gitignored.

(structure based on http://drivendata.github.io/cookiecutter-data-science/)