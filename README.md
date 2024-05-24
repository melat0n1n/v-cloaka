The modified source code of V-Cloak.
Original code is taken from here: https://github.com/V-Cloak/V-Cloak

# Code structure

```shell
.
|-- Datasets
|-- ECAPA
|   |-- classifier.ckpt
|   |-- embedding_model.ckpt
|   |-- hyperparams.yaml
|   |-- label_encoder.ckpt
|   |-- mean_var_norm_emb.ckpt
|-- XVECTOR
|   |-- classifier.ckpt
|   |-- embedding_model.ckpt
|   |-- hyperparams.yaml
|   |-- label_encoder.ckpt
|   `-- mean_var_norm_emb.ckpt
|-- deepspeech4loss_original.py
|-- deepspeech4loss.py
|-- ecapa_tdnn_test.py
|-- masker.py
|-- model
|   |-- conv.py
|   |-- crop.py
|   |-- resample.py
|   |-- utils.py
|   |-- waveunet4val.py
|   `-- waveunet.py
|-- new_pytorch_deep_speech_original.py
|-- new_pytorch_deep_speech.py
|-- requirements.txt
|-- train.py
|-- trainingDataset.py
`-- validation.py
```

- Datasets
	+ README.md
	+ Put the training set here, e.g., voxceleb1.
- ECAPA
	+ README.md
	+ Download the ECAPA-TDNN here.
- deepspeech4loss.py
	+ Compute the ASR loss (CTC, GPG).
- ecapa_tdnn_test.py
	+ tools of ECAPA-TDNN
- masker.py
	+ Compute the psychoacoustic-based loss.
- model
	+ The anonymizer of V-Cloak.
- new_pytorch_deep_speech.py
	+ A modified DeepSpeech model to allow torch.DataParallel.
- train.py
	+ Train the anonymizer.
- trainingDataset.py
	+ Data preparation
- validation.py
	+ Generate anonymized audios.
- requirements.txt
- test.wav
