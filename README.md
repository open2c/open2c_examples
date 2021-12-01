# examples

Following the old adage that an example is worth a thousand docstrings, we created a set of notebooks that cover many typical Hi-C analyses using the open2c code ecosystem. For users who are new to Hi-C analysis, we recommend going through example notebooks in the following order:
- [viz.ipynb](https://github.com/open2c/open2c_examples/viz.ipynb): how to load and visualize Hi-C data stored in coolers.
- [contacts_vs_distance.ipynb](https://github.com/open2c/open2c_examples/contacts_vs_distance.ipynb): how to calculate contact frequency as a function of genomic distance-- the most prominent feature in Hi-C maps
- [insulation_and_boundaries.ipynb](https://github.com/open2c/open2c_examples/insulation_and_boundaries.ipynb): how to extract insulation profiles and call boundaries using insulation profile minima.
- [pileup_CTCF.ipynb](https://github.com/open2c/open2c_examples/pileup_CTCF.ipynb): how to create avearge maps around genomic features like CTCF.
- [compartments_and_saddles.ipynb](https://github.com/open2c/open2c_examples/compartments_and_saddles.ipynb): how to extract eigenvectors and create saddleplots reflecting A/B compartments.

Note that these notebooks currently focus on mammalian interphase Hi-C analysis, but are readily extendible to other organisms and cellular contexts.


# Installation

Clone ope2c_exampnles on your computer using `git clone` command, and checkout the recent version:
```sh
git clone https://github.com/open2c/open2c_examples
git checkout cooltools-0.5.0
```
Then navigate to the `open2c_examples` directory and use `environment.yml` file to create a conda environment `open2c` with the software packages required to run these notebooks:
```sh
cd open2c_examples
conda env create -f environment.yml
```
Activate the environment and launch jupyter:
```sh
conda activate open2c
jupyter lab

```

