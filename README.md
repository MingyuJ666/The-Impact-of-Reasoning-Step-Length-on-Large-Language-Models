# The Impact of Reasoning Step Length on Large Language Models
![image](intro.png)

Created by [Mingyu Jin]()\*, Qinkai Yu\*, Dong Shu, Haiyan Zhao, Wenyue Hua, Yanda Meng†, Yongfeng Zhang†, Mengnan Du†
This repository contains PyTorch implementation of "The Impact of Reasoning Step Length on Large Language Models"

The paper has been accepted by ACL 2024 findings. 

[[arXiv]](https://arxiv.org/abs/2401.04925) https://arxiv.org/abs/2401.04925

[[ACL]](https://aclanthology.org/2024.findings-acl.108/) https://aclanthology.org/2024.findings-acl.108/

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
## Use demo 
### Relationship Between Steps and Accuracy
last_letter_1 represents adding one step to the demo

last_letter_2 represents adding two-step to the demo


.......and so on

```bash
python run_inference.py --dataset last_letter --demo_path demos/last_letter_1 --output_dir experiment/last_letters_1 #1 represent the number of add step
```

### Effect of Prompt with Wrong Answer
```bash
python run_inference.py --dataset last_letter --demo_path demos/last_letters_false --output_dir experiment/last_letters_false
```
## Create demo


## Citation 
If you find this codebase helpful, please consider to cite:
```
@inproceedings{jin2024impact,
  title={The Impact of Reasoning Step Length on Large Language Models},
  author={Jin, Mingyu and Yu, Qinkai and Shu, Dong and Zhao, Haiyan and Hua, Wenyue and Meng, Yanda and Zhang, Yongfeng and Du, Mengnan},
  booktitle={Findings of the Association for Computational Linguistics ACL 2024},
  pages={1830--1842},
  year={2024}
}

@inproceedings{jin-etal-2024-impact,
    title = "The Impact of Reasoning Step Length on Large Language Models",
    author = "Jin, Mingyu  and
      Yu, Qinkai  and
      Shu, Dong  and
      Zhao, Haiyan  and
      Hua, Wenyue  and
      Meng, Yanda  and
      Zhang, Yongfeng  and
      Du, Mengnan",
    booktitle = "Findings of the Association for Computational Linguistics ACL 2024",
    month = aug,
    year = "2024",
    address = "Bangkok, Thailand and virtual meeting",
    url = "https://aclanthology.org/2024.findings-acl.108",
    pages = "1830--1842",
}

@inproceedings{jin2024impact,
  title={The Impact of Reasoning Step Length on Large Language Models},
  author={Jin, Mingyu and Yu, Qinkai and Shu, Dong and Zhao, Haiyan and Hua, Wenyue and Meng, Yanda and Zhang, Yongfeng and Du, Mengnan},
  booktitle={ACL (Findings)},
  year={2024}
}


}
```
