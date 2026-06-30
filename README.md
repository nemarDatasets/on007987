[![DOI](https://img.shields.io/badge/DOI-10.82901%2Fnemar.on007987-blue)](https://doi.org/10.82901/nemar.on007987)

This dataset contains raw EEG recordings in resting state from healthy participants with no current psychiatric or neurological diagnosis, recorded at the Universidad Autónoma de Madrid, inside a Faraday cage. 

No preprocessing was applied prior to data sharing, only conversion to bids from .bdf format (.bdf files are also available upon request). 


- Dataset organization:

All EEG recordings were acquired during a single recording session lasting approximately 20 minutes. Participants completed four consecutive 5-minute runs: two eyes-open (EO) runs and two eyes-closed (EC) runs. Conditions alternated throughout the session, and participants were randomly assigned to one of two acquisition sequences: EO run-1 → EC run-1 → EO run-2 → EC run-2, or EC run-1 → EO run-1 → EC run-2 → EO run-2.

In the BIDS structure, recordings are organized into two session folders for each participant: "ses-OA" (Ojos Abiertos: eyes open) and "ses-OC" (Ojos Cerrados: eyes closed). These session labels are used only to separate recording conditions and do not indicate different visits or recording days.

Example:

sub-05/
├── ses-OA/
│ └── eeg/
│   ├── ...run-1...
│   └── ...run-2...
└── ses-OC/
  └── eeg/
    ├── ...run-1...
    └── ...run-2...

Note that file names also use Spanish abbreviations: OA = Ojos Abiertos (eyes open) and OC = Ojos Cerrados (eyes closed).

- Recording system: 

Biosemi ActiveTwo 128 channels.
1024 Hz sampling rate (except for subj 19, 20, 31, 33, 37, 38, 39, 40, 41, 42, 47 with 2048 Hz).

Note that the power line frequency in Spain is 50 Hz (and harmonics).

Dim light (120-150 lux). 

Participants were instructed to sit still and avoid muscle tension.

Black fixation point over white wall for OA condition. 

