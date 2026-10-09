# Hubness Code

In the real world, many projects end up being only partially completed. In projects where a subset of a set of need to be selected, this creates challenging resilience problem: given that not all of the planned set will be constructed, which should you build and in what order to maintain the greatest functionality. To solve this callenge, we developed the hubness metic. For more detailed infromation on please consult the corresponding paper:

This repository contains the code used to generate the examples shown in this paper.

## Requirements and Installation

This project uses conda environments to manage dependencies. This environment can be created using the command:

``` conda env create --name hubness_code --file=env.yml ```

## Project Point of Contact

If you have any questions about either running this project or the project in general, feel free to contact Kelsey Stoddard at:
```kelsey.s.stodard@gmail.com```

## Project Structure
###

```
├── README.md          <- The top-level README for developers using this project (this file).
│
├── env.yml            <- Conda environment file.
│
├── fuel_breaks
│   ├── data           <- Input data: Saved fire graph and optimization results
│   ├── figures        <- Output figures: Paper plots
│   └── fuel_breaks_paper_plots.ipynb   <- Jupyter notebook used to generate output paper plots 
|
├── motivating_example
│   ├── figures        <- Output figures: Paper plots
│   └── motivating_example.ipynb   <- Jupyter notebook used to generate motivating example and plots
|
├── network_separation
│   ├── data           <- Intermediate data: Saved fire graph and optimization results output from internet_disruption
│   ├── figures        <- Output figures: Paper plots
│   ├── internet_disruption.ipynb      <- Jupyter notebook used to make internet graph and perform optimization
│   └── hubness_paper_pictures.ipynb   <- Jupyter notebook used to generate output paper plots 
|
└── zero-e_refueling_ca
    ├── data           <- Input data: CA optimization results
    ├── figures        <- Output figures: Paper plots
    └── hubness_paper_generator.ipynb   <- Jupyter notebook used to generate output paper plots 

(structure based on http://drivendata.github.io/cookiecutter-data-science/)