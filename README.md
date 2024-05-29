The modified source code of V-Cloak.
Original code is taken from here: https://github.com/V-Cloak/V-Cloak
Weights after training (43 epoch ~ 43h on A100) are located at [Google Drive](https://drive.google.com/file/d/18a9uxaoJKU6JEB_SFGv7YFLnOGp865Oo/view?usp=drive_link)

## Project structure

```shell
|--Pics
|--Samples
|--V-Cloak
|  |-- Datasets
|  |-- ECAPA
|  |   |-- classifier.ckpt
|  |   |-- embedding_model.ckpt
|  |   |-- hyperparams.yaml
|  |   |-- label_encoder.ckpt
|  |   |-- mean_var_norm_emb.ckpt
|  |-- XVECTOR
|  |   |-- classifier.ckpt
|  |   |-- embedding_model.ckpt
|  |   |-- hyperparams.yaml
|  |   |-- label_encoder.ckpt
|  |   `-- mean_var_norm_emb.ckpt
|  |-- model_checkpoint_GPU
|  |   `-- _VCloak_CheckPoint_newest
|  |-- deepspeech4loss_original.py
|  |-- deepspeech4loss.py
|  |-- ecapa_tdnn_test.py
|  |-- masker.py
|  |-- model
|  |   |-- conv.py
|  |   |-- crop.py
|  |   |-- resample.py
|  |   |-- utils.py
|  |   |-- waveunet4val.py
|  |   `-- waveunet.py
|  |-- new_pytorch_deep_speech_original.py
|  |-- new_pytorch_deep_speech.py
|  |-- requirements.txt
|  |-- train.py
|  |-- trainingDataset.py
|  `-- validation.py
|--Graphs.ipynb
|--RIR.ipynb
`--VCloak_test.ipynb
```


## Results
- Detailed results and comparisons can be found in the `Graphs.ipynb` notebook.

Below are the barplots illustrating the model performance comparisions: 

1. **ASR model performance on anonimized data**

<p align="center"><img src="pics/Picture_2.png" width="600">

2. **Speaker verification task by model**

<p align="center"><img src="pics/Picture_1.png" width="600">
