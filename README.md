#  LibriSpeech 100h ASR Training with k2/icefall
This project demonstrates training an **Automatic Speech Recognition (ASR)** system using the **LibriSpeech 100-hour subset**, implemented with the [k2](https://github.com/k2-fsa/k2) and [icefall](https://github.com/k2-fsa/icefall) frameworks.

##  Dataset

- **LibriSpeech (train-clean-100)** from [OpenSLR](http://www.openslr.org/12/)
- Total: ~100 hours of clean, read English speech
- Sample rate: 16 kHz, mono

##  Setup and Environment

- Framework: [Icefall](https://github.com/k2-fsa/icefall)
- Libraries: PyTorch, K2, Lhotse, torchaudio
- Python: 3.8+

##  Data Preparation

I used the official **k2 LibriSpeech recipe** located in:
icefall/egs/librispeech/ASR
To prepare the dataset:



