##  Official Implementation of [GLMKD-WSSS] / 论文代码官方实现

This repository contains the official implementation of the paper:

**[GLMKD: Joint Global and Local Mutual Knowledge Distillation for Weakly Supervised Lesion Segmentation in Histopathology Images]**

[Authors: Hangbei Cheng, Yongfei Wu, etc.]  [作者：成航北，刘雪宇，吴永飞等]

Currently under review at [[Expert Systems with Applications](https://www.sciencedirect.com/journal/expert-systems-with-applications)].

If our work is accepted, we plan to publicly release the code in a timely manner after the paper is published.

---

## *The overall framework* / 主体框架

To segment the lesion from WSI image with image-level label, we propose a novel weakly supervised segmentation solution that combines global and local mutual knowledge distillation (dubbed GLMKD). The overall framework of our proposed approach is illustrated in Fig. 2, GLMKD adheres to the two-stage paradigm of WSSS, which consists of three components: global learning, multi-scale local learning, and mutual knowledge distillation segmentation.
![image](https://github.com/user-attachments/assets/f3d1da31-566d-47af-8822-0e2ff9dbccce)



## Highlights / 亮点

- A novel weakly-supervised segmentation framework is proposed to enhance lesion delineation in digital pathology images by integrating global and local information.
- This study is the first to combine global supervisory information and multi-scale MIL via dual-stream knowledge distillation in a WSSS framework.
-  A multi-scale multi-instance learning model (MMIL) is designed to capture subtle variations in lesions across different scales.
- A shape transfer loss function is introduced to facilitate effective information exchange between global and local contexts during the dual-flow mutual knowledge distillation (MKD) segmentation phase.

---

## Code Overview / 代码概览

### Repository Structure / 仓库结构

```
├── data/                 # 示例数据集或数据加载脚本
├── models/               # 模型定义
├── experiments/          # 实验脚本
├── utils/                # 工具函数
├── results/              # 结果或检查点
├── requirements.txt      # Python 依赖
└── README.md             # 本文件
```

### Requirements / 环境要求

安装依赖环境：

```bash
pip install -r requirements.txt
```

### Datasets / 数据集

The experiments were conducted on two publicly available datasets, Camelyon16 and

DigestPath 2019, as well as a proprietary Glomerular lesion dataset.

---

## Getting Started / 快速开始

1. Clone the repository（克隆代码仓库）：

   ```bash
   git clone  https://github.com/chenghangbei0702/GLMKD-WSSS.git
   cd main
   ```

2. Install dependencies（安装依赖）:

   ```bash
   pip install -r requirements.txt
   ```

3. train（训练模型）:

   ```bash
   python train.py
   ```

---

## **Acknowledgment/项目支持**

The authors sincerely thank the editors and reviewers for their valuable and constructive advice on the revision of the manuscript. This work was supported by National Natural Science Foundation of China under Grant No. 61901292, The Natural Science Foundation of Shanxi Province, China under Grant No. 202303021211082.

## Citation / 引用

如果您觉得该工作有帮助，请引用：

```bibtex
@inproceedings{GLMKD,
  title={GLMKD: Joint Global and Local Mutual Knowledge Distillation for Weakly Supervised Lesion Segmentation in Histopathology Images},
  author={Hangbei Cheng, Xueyu Liu, Jun Zhang, Xiaorong Dong, Xuetao Ma, Yansong Zhang, Hao Meng, Xing Chen, Guanghui Yue, Yidi Lia,∗, Yongfei Wu∗},
  year={2025}
}
```

---

## License / 许可

本项目基于 [License Name] 许可协议发布。详细信息请参阅 `LICENSE` 文件。

---

## Contact / 联系方式

如有问题或反馈，请联系 [chenghangbei0702@163.com或 GitHub 主页]。
