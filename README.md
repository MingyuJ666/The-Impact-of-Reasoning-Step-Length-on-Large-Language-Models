# The Impact of Reasoning Step Length on Large Language Models

Created by [Mingyu Jin]()\*, [Qinkai Yu]()\*, [Dong Shu],[Haiyan Zhao],[Wenyue Hua],[Yanda Meng]†,[Yongfeng Zhang]†,[Mengnan Du]†
This repository contains PyTorch implementation of "The Impact of Reasoning Step Length on Large Language Models"

[intro.png]

[[arXiv]](https://arxiv.org/abs/2401.04925)

## Installation
Make sure you have Python>=3.8 installed on your machine.

```bash
pip install torch==1.8.2+cu111 torchtext==0.9.2 -f https://download.pytorch.org/whl/lts/1.8/torch_lts.html
pip install -r requirements.txt
```
## Datasets 
Download the datasets from the following:
```
https://github.com/kojima-takeshi188/zero_shot_cot/tree/main/dataset
https://github.com/kojima-takeshi188/zero_shot_cot/tree/main/log
```
## Run inference
```bash
python run_inference.py --dataset multiarith --demo_path demos/multiarith --output_dir experiment/multiarith
```
## Create demo


## Citation 
If you find this codebase helpful, please consider to cite:
```
@article{jin2024impact,
  title={The Impact of Reasoning Step Length on Large Language Models},
  author={Jin, Mingyu and Yu, Qinkai and Zhao, Haiyan and Hua, Wenyue and Meng, Yanda and Zhang, Yongfeng and Du, Mengnan and others},
  journal={arXiv preprint arXiv:2401.04925},
  year={2024}
}
```
