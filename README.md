# EIC_CORE

!!!! Still in development. Binning and files may not be exact yet. !!!!


In each directory histograms are recorded in root files. Histograms are produced for three sets of energies: 5x100, 10x275 and 18x275 GeV (electron on proton). Each set of energies has generated (particle) and reconstructed (track) events for pions and kaons. Only particles where CORE is estimated to have 3 sigma pion/kaon separation (as defined by the rapidity, "eta"), are kept:

p < 2 GeV, -3.5 < eta < 3.5;
2 < p < 6, -1.65 < eta < 3.5;
6 < p < 50, 1.57 < eta < 3.5;

Binning was chosen to match the EIC Yellow Report. Bin edges defined below (so there are n-1 points):

float Q2_bins[12] = {1.0, 1.3335, 1.77828, 2.371373, 3.16227766, 4.2169657, 5.623415, 7.4989399, 10.0, 13.335216, 17.78280068, 23.7137302};

float x_bins[13] = {0.000398107, 0.000630957, 0.001, 0.00158489, 0.00251189, 0.00398107, 0.00630957, 0.01, 0.0158489, 0.0251189, 0.0398107, 0.0630957, 0.1};

float z_bins[14] = {0.0, 0.05, 0.1, 0.15, 0.2, 0.25, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0};

float PhT_bins[14] = {0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0, 1.5, 2.0, 4.0};

Histograms are for z or PhT and indexed by which Q2-x bin they occur in.
