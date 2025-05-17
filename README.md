#  LibriSpeech 100h ASR Training with K2/Icefall
This project demonstrates training an **Automatic Speech Recognition (ASR)** system using the **LibriSpeech 100-hour subset**, implemented with the [K2](https://github.com/k2-fsa/k2) and [Icefall](https://github.com/k2-fsa/icefall) frameworks.

##  Dataset

- **LibriSpeech (train-clean-100)** from [OpenSLR](http://www.openslr.org/12/)
- Total: ~100 hours of clean, read English speech
- Sample rate: 16 kHz, mono

##  Setup and Environment

- Framework: [Icefall](https://github.com/k2-fsa/icefall)
- Libraries: PyTorch, K2, Lhotse, torchaudio
- Python: 3.8+
- CUDA (for GPU training)

##  Data Preparation

I used the official **K2 LibriSpeech recipe** located in:
icefall/egs/librispeech/ASR
To prepare the dataset:


```bash
cd icefall/egs/librispeech/ASR
./prepare.sh  --stage 0 --stop-stage 0```
Then I completed the rest of the stages sequentially to fully prepare the data.

This handles:
 Downloading train-clean-100
 Creating manifests using Lhotse
 Preparing lexicon and language models
 Generating features (e.g., fbank)
 Constructing FSAs for training
