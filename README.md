# Gravitational-Wave-Analysis-and-Detection

# Dataset Description
 This dataset is taken from Kaggle G2Net Gravitational Wave Detection (https://www.kaggle.com/c/g2net-gravitational-wave-detection/overview)
 
 There are 560000 records in .npy format and each of them contains three samples from 3 different laboratory that spans for 2 seconds. The detectors
are sensitive to space time strain induced by passing gravitational waves but also, they are affected by many noises such as quantum sensing noise, seismic noise etc. Our job is to clean the noise from the records and extracting important features from it.

## Gravitational waves
 Gravitational waves are 'ripples' in space-time fabric caused by some of the most violent and energetic processes in the Universe such as black holes or neutron star collisions.
 
# Approach  
 A Tukey window with 0.15 s transition regions is applied and then whitened to ensure each frequency bin has equal significance by down-weighting frequencies where the noise is loud and then the data were bandpass filtered with band pass [35, 350]. Then the data is q transformed in order to produce the image.

# Note 
Download the g2net-gravitational-wave-detection from https://www.kaggle.com/c/g2net-gravitational-wave-detection/data, extract the zip folder and place it in the same place as this file. The directory should be like this.

|-->g2net-gravitational-wave-detectio---->(train\, test\, training_labels, sample_submission)

|--->plotting_the_data.ipynb

|--->Cleaning the data.ipynb

# Reference:
 1, https://github.com/scipy/scipy/blob/v1.7.1/scipy/cluster/vq.py#L85-L139
 2, A guide to LIGO-Virgo detector noise and extraction of transient gravitational-wave signals (https://arxiv.org/pdf/1908.11170.pdf)
 3, A tapering window for time-domain templates andsimulated signals in the detection of gravitational waves from coalescing compact binaries(https://arxiv.org/pdf/1003.2939.pdf)
 4, CONSTANT-Q TRANSFORM TOOLBOX FOR MUSIC PROCESSING (https://core.ac.uk/download/pdf/144846462.pdf)
