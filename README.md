# Predicting libraries for labeled peptides

Peptides are made identifiable in LC-MS/MS due to their predictable characteristics (e.g. retention time, ion-mobility, MS1 precursor m/z, and MS2 fragment m/z's). While these characteristics are largely predictable with high accuracy for label-free peptides due to overwhelming experimental and analytical work spanning decades, there is need for a stream-lined workflow to predict these characteristics for labeled peptides (e.g. mTRAQ or TMT) to improve identifications. 

Here, empirical ion-mobility (IM) and MS2-spectral data from mTRAQ-labeled peptides were used to build deep learning models to predict these characteristics; the goal was to increase the number of identifications, and thus proteomic coverage.

Results:

**Ion-mobility predictions**: ~2% increase in precursor identifications and ~5% increase in protein identifications.

**MS2-fragment-spectra** (work in progress): ~5% fewer precursor & protein identifications than DIA-NN's base-line predictions, which has already been optimized for mTRAQ by other means during work related to plexDIA (https://www.nature.com/articles/s41587-022-01389-w). Note: this current implementation works well, albeit perhaps not as well as DIA-NN's fragment spectra prediction. However, the benefit of this work-flow is that it will extend easily to other novel labels (not just mTRAQ), whereas DIA-NN cannot without outside training such as this.




Spectral library used for training Ion Mobility of mTRAQ peptides can be downloaded here: https://drive.google.com/file/d/1ldCjhKOhRpPfrEc7GQNaHztP_nwlrj1g/view
