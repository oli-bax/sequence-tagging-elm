# Sequence Tagging with Extreme Learning Machines

This repo contains implementation of a bunch of extreme learning machine algorithms for sequence tagging tasks. All have been implemented in plain Python with help from [chickenbestlover](https://github.com/chickenbestlover/Online-Recurrent-Extreme-Learning-Machine).

This repo contains implementations of ORELM, NFOSELM, NAOSELM, FOSELM.

### Running

- `git clone https://github.com/E-Renshaw/sequence-tagging-elm`
- Download the CONLL-2003 dataset
- `python run.py -a [ORELM|NFOSELM|NAOSELM|FOSELM] -d path/to/dataset`

### Results

Here are some initial results on the CONLL-2003 NER task.

| Algorithm | F1 score |
|---|---|
| GloVe + Bi-LSTM + CRF (baseline) | [91.62](https://github.com/mxhofer/Named-Entity-Recognition-BidirectionalLSTM-CNN-CoNLL) |
| GloVe + ORELM | 84.21 |
| GloVe + NAOSELM | 82.22 |
| GloVe + NFOSELM | 81.49 |
| GloVe + FOSELM | 77.53 |
