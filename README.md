# Working with maps at scale using Computer Vision and Jupyter notebooks
 

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4244363.svg)](https://doi.org/10.5281/zenodo.4244363)

Author: Daniel van Strien <a itemprop="sameAs" content="https://orcid.rg/0000-0003-1684-6556" href="https://orcid.org/0000-0003-1684-6556" target="orcid.widget" rel="me noopener noreferrer" style="vertical-align:top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon">https://orcid.org/0000-0003-1684-6556</a>

> Credit: *This project, funded by the UK Research and Innovation (UKRI) Strategic Priority Fund, is a multidisciplinary collaboration delivered by the Arts and Humanities Research Council (AHRC), with The Alan Turing Institute, the British Library and the Universities of Cambridge, East Anglia, Exeter, and Queen Mary University of London.*

Originally delivered as part of [Digital Humanities and Digital Archives](https://web.archive.org/web/20201103155204/https://www.nlib.ee/en/node/8579) workshop at the National Library of Estonia. This notebook is intended to work as a 'stand alone' resource but doesn't cover all the topics in depth. It is instead intended as an overview of a range of topics. 

## tl;dr 

This workshop/notebook aims to cover a few main things:
- 📒 show how [Jupyter notebooks](https://jupyter.org/) can be particularly useful for working with digitised collections at scale
- 👀 give a brief sense of what is possible using computer vision with image collections 
- 🤖 give some ideas for how existing GLAM infrastructure (in this case [IIIF](iiif.io/)) can support new machine learning-based approaches 

The above use maps as an example, but most of the workshop is not specific to maps. 

The notebooks make use of the delightful [Newspaper Navigator dataset](https://news-navigator.labs.loc.gov/) from the Library of Congress: 
> ["Chronicling America is a product of the National Digital Newspaper Program, a partnership between the Library of Congress and the National Endowment for the Humanities to digitize historic newspapers. Over 16 million pages of historic American newspapers have been digitized for Chronicling America to date, complete with high-resolution images and machine-readable METS/ALTO OCR. Of considerable interest to Chronicling America users is a semantified corpus, complete with extracted visual content and headlines. To accomplish this, we introduce a visual content recognition model trained on bounding box annotations of photographs, illustrations, maps, comics, and editorial cartoons collected as part of the Library of Congress's Beyond Words crowdsourcing initiative..."](https://arxiv.org/abs/2005.01583)


## Contents 
### 01_finding_maps.ipynb

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Living-with-machines/maps-at-scale-using-computer-vision-and-jupyter-notebooks/blob/main/01_finding_maps.ipynb)

This notebooks uses a sample of images drawn from the [Newspaper Navigator dataset](news-navigator.labs.loc.gov/), in particular images from the Newspaper Navigator dataset predicted as 'maps'. It turns out that machine learning isn't perfect! In this notebook we look at some potential approaches to:
- 'cleaning' up this dataset 
- using [ipywidgets](https://ipywidgets.readthedocs.io/en/stable/) as a middle ground between developing 'full' [GUIs](https://en.wikipedia.org/wiki/Graphical_user_interface) and 'code only' sharing of methods
- traning a computer vision model 
- a couple of potential approches for working with images at scale
- brief discussion of working with probable labels. 

The model trained in the notebook is trained on a dataset; [Images from Newspaper Navigator predicted as maps, with human corrected labels](https://zenodo.org/record/4156510)


### appendix_finding_maps_inference_demo.ipynb 
An appendix notebook which is used to generate an example JSON dataset of predicted labels for 10,000 images from the Newspaper Navigator dataset of images predicted as maps.  
