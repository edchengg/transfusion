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

- We use [nllb-200-3.3B-easyproject](https://huggingface.co/ychenNLP/nllb-200-3.3B-easyproject) translation model that is fine-tuned to preserve special markers during translation on 5 high-resource languages (Germany, Spanish, Dutch, Chinese, Arabic). The fine-tuning data is automatically constructed (see details in Section 4.1 in [EasyProject](https://arxiv.org/abs/2211.15613)). You can access fine-tuning data and training script at [EasyProject Github](https://github.com/edchengg/easyproject/tree/main/mt_training).

## Funding Acknowledgment
This material is based in part on research sponsored by IARPA via the BETTER program (2019-19051600004).
