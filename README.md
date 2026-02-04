# USMD-and-UDLM

##  Overview

USMD-and-UDLM is a maritime small-object dataset designed for unmanned surface vessel (USV) perception tasks, such as maritime patrol, marine governance, and autonomous navigation.

The dataset consists of two complementary parts:

- **USMD**: a large-scale dataset constructed by filtering and re-labeling multiple publicly available maritime datasets.
- **UDLM**: a real-world dataset collected and annotated by a self-built unmanned surface vessel (USV) platform in Dalian Bay.

The two datasets share consistent category definitions and annotation rules, enabling joint model training and real-world generalization evaluation.

Contact: Ning Huang, Email:funny1201@foxmail.com;  Changdong Yu, Email: ycd@dlmu.edu.cn;
---

![pdf](combined_analysis.pdf)

## Dataset Description

### USMD (The Small Maritime Dataset for USV)

The **USMD** dataset is a large-scale dataset obtained by filtering and re-labeling multiple publicly available maritime datasets.  
All images are strictly selected from the **USV perspective**, ensuring that the vast majority of objects occupy less than **1% of the image area**, which conforms to the definition of maritime small objects.

- Data split: training / validation / test = **7 : 2 : 1**
- Usage: model training and performance evaluation
- Object categories:
  - Passenger ship  
  - Freighter  
  - Yacht  
  - Assault boat  
  - Canoe  
  - Fisher  
  - Others  

---

### UDLM (The Small Maritime Dataset for USV collected in DaLian)

The **UDLM** dataset is a small-scale dataset collected and annotated in real marine environments using a self-built unmanned surface vessel (USV) platform.

- Collection area: Dalian Bay and surrounding waters
- Image resolution: 1920 × 1080
- Weather conditions: clear, cloudy, and foggy
- Supplementary data: a small number of publicly available online maritime images
- Usage: evaluation of **model generalization ability** and **engineering applicability**
- Object categories: consistent with USMD

USMD and UDLM can be used respectively for model training and real-world generalization testing.

---

# Download Datasets

Download link: [Baidu]( https://pan.baidu.com/s/1kZNsOI1ZZ6QZKpJuZDa_9Q?pwd=7sr9) Password: 7sr9

## 🗂 Description of the File Structure

```text
USMD-and-UDLM/
├── USMD/
│   ├── images/
│   │   ├── train/
│   │   ├── val/
│   │   └── test/
│   └── labels/
│       ├── train/
│       ├── val/
│       └── test/
├── UDLM/
│   ├── images/
│   └── labels/
├── combined_analysis.pdf
├── README.md
└── LICENSE
