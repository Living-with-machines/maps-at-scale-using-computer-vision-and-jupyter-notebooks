# Working with maps at scale using Computer Vision and Jupyter notebooks

Author: Daniel van Strien <a itemprop="sameAs" content="https://orcid.rg/0000-0003-1684-6556" href="https://orcid.org/0000-0003-1684-6556" target="orcid.widget" rel="me noopener noreferrer" style="vertical-align:top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon">https://orcid.org/0000-0003-1684-6556</a>

> Credit: *This project, funded by the UK Research and Innovation (UKRI) Strategic Priority Fund, is a multidisciplinary collaboration delivered by the Arts and Humanities Research Council (AHRC), with The Alan Turing Institute, the British Library and the Universities of Cambridge, East Anglia, Exeter, and Queen Mary University of London.*

Originally delivered as part of [Digital Humanities and Digital Archives](https://web.archive.org/web/20201103155204/https://www.nlib.ee/en/node/8579) workshop at the National Library of Estonia.

## tl;dr 

This workshop/notebook aims to cover a few main things:
- 📒 how notebooks can be particularly useful for working with digitised collections at scale
- 👀 give a brief sense of what is possible using computer vision with image collections 
- 🤖 give some ideas for how existing GLAM infastucture (in this case IIIF) can support new machine learning based approaches 

The above use maps as an example, but most of the workshop is not specific to maps. 


## Contents 
### 01_finding_maps.ipynb
Is the main notebook which covers the above topics using data drawn from the [Newspaper Navigator dataset](news-navigator.labs.loc.gov/), in particular images from the Newspaper Navigator dataset predicted as 'maps'. The model trained in the notebook is trained on a dataset; [Images from Newspaper Navigator predicted as maps, with human corrected labels](https://zenodo.org/record/4156510)


### appendix_finding_maps_inference_demo.ipynb 
An appendix notebook which is used to generate an example JSON dataset of predicted labels for 10,000 images from the Newspaper Navigator dataset of images predicted as maps.  
