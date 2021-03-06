
Overview
===========

This repository contains a series of Jupyter Notebooks that facilitate complete reproduction of all figures included in our study of Pnt and Yan expression during eye development in *Drosophila*. Refer to the [Jupyter documentation](https://jupyter-notebook.readthedocs.io/en/stable/) for an introduction to starting and running Jupyter Notebooks.



System Requirements
=========

 - Python 3.6+

Dependencies
------------

 - [Seaborn](https://seaborn.pydata.org/)
 - [Jupyter Notebook](http://jupyter.org/install)
 - [FlyEye Analysis](https://sebastianbernasek.github.io/flyeye/index.html): our package for analyzing FlyEye Silhouette data
 - [FlyEye Clones](https://sebastianbernasek.github.io/clones/index.html): our package for analyzing eye clones
 - [Binding](https://github.com/sebastianbernasek/binding): our package for modeling protein-DNA binding interactions



Data
=========

The data presented in our manuscript are available in our [data repository](https://github.com/sebastianbernasek/flyeye). The repository contains three types of data:

   1. **Microscopy:** Raw 3D image stacks in ``.tif`` format. Regularly spaced layers span the entire eye epithelium.

   2. **Measurements:** Segmented and annotated image stacks in ``.silhouette`` format. These files are generated by our *FlyEye Silhouette* software for macOS. The ``.silhouette`` container includes all measurement and annotation data, in addition to RGB images of each layer in ``.png`` format. These are not the original full-resolution microscope images, they have been smoothes and downsampled to reduce overall filesize.

   3. **Clone Microscopy:** Raw cross-sectional images of genetic clones in ``.tif`` format. A small collection of images depicting irregularly-spaced and non-overlapping layers are contained within each file.



Modules
=========

This repository includes a ``figures`` module comprised of several submodules for generating each type of figure in our manuscript:

* ``figures.images`` Rendered 2D images.

* ``figures.dynamics`` Protein expression time series.

* ``figures.scatter`` 2D joint distributions of protein expression levels.

* ``figures.comparison`` Box and Violin comparisons of expression levels.

* ``figures.spatial`` Correlation functions and spectrograms for detection of periodic spatial patterns.

* ``figures.phase`` Equilibrium binding occupancy phase diagrams and titration contours.



Notebooks
=========

We have included one notebook per primary figure that appears in the manuscript:

   1. ``Figure1.ipynb`` Pnt and Yan expression dynamics in multipotent cells.

   2. ``Figure2.ipynb`` Pnt and Yan expression dynamics in cells undergoing state transitions.

   3. ``Figure3.ipynb`` Equilibrium binding site occupancy by two competing transcription factors.

   4. ``Figure4.ipynb`` Effects of varying *pnt-GFP* and *yan* gene dosage.

   5. ``Figure5.ipynb`` Notch signaling effects on Pnt and Yan levels. Note that the images constructed in this notebook are based on the downsampled ``.png`` format images within each ``.silhouette`` file. The images presented in our manuscript were derived from the original full-resolution microscopy data.

   6. ``Figure6.ipynb`` RTK signaling effects on Pnt and Yan levels.

Each notebook is designed to walk a user through the generation of each subpanel comprising the primary figure and all of its supplements. We have explicitly named all subpanels in accordance with the corresponding figure numbers and panel letters that appear in our manuscript.

Note that we applied some minor formatting adjustments using Adobe Illustrator. Consequently, figures rendered via these notebooks may not be aesthetically identical to those presented in our manuscript.



Additional Questions
-------------

Please direct any questions related to the analysis covered by these notebooks to the [Amaral lab](https://amaral.northwestern.edu/).
