# TTS-for-the-hearing-impaired
### STATEMENT
This repository contains all codes I used for my master's thesis: Transfer Learning to Quickly Adapt a Text-to-Speech System for the Hearing Impaired

This repository is a collaborative work with my supervisor, Dr. Josef Schlittenlacher

### BRANCH CONTENTS TABLE
1. Inference
<br />(1) Inference mult: Used for Inference. Users need to manually create a test list of audio and mel (.wav and .wav.pt) based on their own directory.
2. MOS
<br />(1) Calculate MOS: Calculates the MOS based on the raw data from Prolific (https://www.prolific.co/)
<br />(2) MOS evaluation: Conducts data wrangling, descriptives and ANOVA on the MOS.
3. STOI
<br /> (1) Combined HI: Does the same job as STOI HI, but with Experiment I, Experiment IIa and IIb (i.e. standard audiogram and patient audiogram vocoders)
<br /> (2) Compute STOI: Compute STOI from the test speech and original speech  
<br /> (3) STOI HI: Reads cleaned STOI data from the patient-audiogram condition. Performs basic data wrangling and visualization before ANOVA.  
<br /> (4) STOI demo: Generates heatmaps and waveforms to demonstrate the rationale of STOI.
<br /> (5) STOI standard_audiograms: Does the same job as STOI HI, but with the standard-audiogram vocoders.
4. Training
<br /> (1) Train config: configurations for transfer learning (need a fully-trained WaveGLow (630k iterations) before adaptation)
<br /> (2) Train HI: Training the vocoders according to a certain config file. This is the main training file.

### Others
<be /> (1) Some other MATLAB codes I used in this thesis, such as inverse amplification, were modified based on codes owned by Josef Schlittenlacher and were not open source, thus I didn't post them here. If required, go to https://arxiv.org/abs/2012.02174 or https://github.com/js2251.
<be /> (2) The codes were not well-structured basically because of the follow-up (ExpIIb) test we included during our experiment and I made some other attempts or changes during processing the data. However, the files contain all the essential scripts. One may selectively refer to part of these codes.

### Acknowledgement 
<be /> I would like to thank my supervisor, Dr. Josef Schlittenlacher (https://www.schlittenlacher.com/), for all his help and suggestions during my master's program. 
