# TransFusion

[Paper](https://arxiv.org/abs/2305.13582): Better Low-resource Entity Recognition Through Translation and Annotation Fusion

<img src="https://raw.githubusercontent.com/edchengg/transfusion/main/asset/trans_gif.gif" width="250" height="150">

## Data
[TransFusion Data](https://drive.google.com/drive/folders/1dNPLlvgA_wQ72uVhw5gL30a60aIySkl-?usp=share_link)

## Code
Train transfusion on masakhaner with mdebertav3 (code/).
```bash
bash train_masakha_ner_mdeberta.sh
```

## EasyProject Data Generation
Translation data can be found in the [Google Drive](https://drive.google.com/drive/folders/1hGdHfs4eoOR7Ve9Y_tCUu-p0xRmzXf6J?usp=sharing). 
Run the following code to project labels from translation data in 'conll_nllb_3B_ft.pkl':

```
python decode_marker_conll.py
```


## Funding Acknowledgment
This material is based in part on research sponsored by IARPA via the BETTER program (2019-19051600004).
