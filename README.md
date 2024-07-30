## EEG source estimate with atlas labeling

I tried to estimate the activity of the sources of the contingent negative variation. 
I used an LCMV beamformer (linearly constrained minimum variance) implemented in MNE Python. 
I have quite long epochs (3 s). Empirically, the best quality was achieved when calculating the date covariance for the entire epoch, the noise covariance on the baseline and then cutting out the area of interest.

To associate activity with specific structures, the coordinates of the most active vertices were compared with the coordinates of the AAL atlas


