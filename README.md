# Digital-Assyriology
Tools and Examples for Computational Text Analysis for Assyriologists.

This repository offers Jupyter Notebooks for scraping data from the [Open Richly Annotated Cuneiform Corpus](http://oracc.org) and the [Electronic Text Corpus of Sumerian Literature](http://etcsl.orinst.ox.ac.uk/), as well as Notebooks that provide examples for the kind of analyses that the data make possible. You may download the entire fileset as a ZIP file with the green button (Clone or download). In order to run the Notebooks you need to install [Anaconda](https://www.continuum.io/downloads) for Python 3.5 (this includes Python as well as a host of other tools). You may adjust the Notebooks or re-use the code for other purposes without restriction.

Currently, three Notebooks are available, plus a set of files scraped from ETCSL.

## Scraping ORACC

The process of scraping dating from ORACC works in two steps: 1. downloading the HTML files to your local computer and 2. scraping the data from the local HTML files.

The Notebook `Save Oracc HTML files.ipynb` needs a list of text identification numbers that you wish to download. This list should be placed in the directory `Input`. This directory already contains a few example lists. The list of text IDs should be made with a text editor such as TextEdit (or, if you prefer a program like Word, use the Save As function to create a Plain Text file). The list of text IDs gives the ORACC project abbreviation plus the text's P, Q, or X number (consisting of a capital P, Q, or X plus six digits). You find these numbers in the left pane of any ORACC text page:

dcclt/Q000039
rinap/rinap1/Q003421
saao/saa01/P313876

etc.

The HTML pages will be stored in the directory `HTML` on your computer.

The Notebook `Scrape Oracc.ipynb` will use the same list of text ID numbers to scrape the raw HTML files and create output in the directory `Output` on your computer. 

## Scraping ETCSL

The scraped ETCSL files are available in the directory `ETCSL/cleaned`. If you wish to scrape the ETCSL files yourself (for instance because you need another output format) you may request the original XML files at the [Oxford Text Archive](http://ota.ox.ac.uk/desc/2518). You may then use the Notebooks `Scrape-etcsl-XML.ipynb` to scrape the XML files and `ETCSL-to EPSD2.ipynb` to adjust the lemmatization to Epsd2 standards.

The scraped ETCSL files essentially draw directly from the data on the online ETCSL site. The following header, copied from the Oxford Text Archive, equally applies to the files available here.

> The Electronic Text Corpus of Sumerian Literature. Revised edition.

> Editor	
> Cunningham, Graham (ed.); Ebeling, Jarle (ed.); Black, Jeremy (deceased) (ed.); Flückiger-Hawker, Esther (ed.); Robson, Eleanor (ed.); Taylor, Jon (ed.); Zólyomi, Gábor (ed.)

> Availability	
> Use of this resource is restricted in some manner. Usually this means that it is available for non-commercial use only with prior permission of the depositor and on condition that this header is included in its entirety with any copy distributed.
