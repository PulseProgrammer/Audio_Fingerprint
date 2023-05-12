# Audio_Fingerprint
Audio Fingerprinting and Identification through Spectral Peak Picking and Matching funnctions

This repository presents an audio identification algorithm based on spectral peak picking for the analysis of a set of database and query recordings. The algorithm generates audio fingerprints for each recording, allowing for efficient comparison and identification of audio content. The code has been tested and implemented using the GTZAN dataset and its query recordings.

## Background
Audio identification plays a crucial role in various domains, such as music recognition, content retrieval, digital forensics, and copyright enforcement. Fingerprinting is a key technique in audio identification, where relevant features, such as spectral peaks, are extracted from the audio signal to create a unique representation. Spectral peaks represent distinctive frequency components of the audio signal that correspond to its robust spectral content. These peaks are derived from the Fourier Transform of the audio signal, specifically the Short-Time Fourier Transform (STFT) in this implementation. Any spectral feature extraction algorithms can be used for building fingerprints, provided it is releavant with the quality of data we have and our end goal.  

## Goal
The goal of this algorithm is to identify the top 3 matches from the database fingerprints (database recordings) for each corresponding query fingerprint (query recording). The process involves calculating the fingerprints for each query audio file by performing STFT and applying the peak picking algorithm. These query fingerprints are then matched against the fingerprints of the database recordings.


## Results
The implementation evaluates the effectiveness of the algorithm in accurately identifying audio signals, using the GTZAN dataset and its query recordings as a test case. The report demonstrates the algorithm's ability to achieve accurate and efficient audio identification through the analysis of spectral peaks.

Please note that this algorithm serves as a starting point and can be further enhanced and customized based on specific requirements and datasets.

**Note:** This code was tested and implemented using the GTZAN dataset and its query recordings. The code is flexible enough to run on any dataset. Certain changes may have to be done depending on the preprocessing steps required on that new dataset. 
