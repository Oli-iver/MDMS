# MDMS
"Multi-Domain Multi-Scale Diffusion Model for Low-Light Image Enhancement"

## Demo
#### 1. Download pretrained model

Download Pretrained MDMS: [Baidu NetDisk](https://pan.baidu.com/s/1J8rrUW8K0Cw2L94sgMI-vQ).

Put the downloaded model in `datasets/scratch/LLIE/ckpts`.



#### 2. Inference
```
# in {path_to_this_repo}/,
$ python eval_diffusion.py
```
Put the test input in `datasets/scratch/LLIE/data/lowlight/test/input`.

Output results will be saved in `results/images/lowlight/lowlight`.

## Evaluation
```
# in {path_to_this_repo}/,
$ python evaluation.py
```

## Results
All results and models listed in our paper are available in [Baidu Netdisk](https://pan.baidu.com/s/1O8hOVflnLGLSLP07nXp_sg?pwd=zftu) or [Google Drive](https://pan.baidu.com/s/1O8hOVflnLGLSLP07nXp_sg?pwd=zftu).

* Note that the provided model is trained on the LOLv1 training set, but generalizes well on other datasets. 

### 1. Test results on LOLv1 test set.
![All text](https://github.com/Oli-iver/MDMS/blob/main/figs/v1.png)

### 2. Generalization results on LOLv2 syn and real test sets.
![All text](https://github.com/Oli-iver/MDMS/blob/main/figs/vis.png)

### 3. Generalization results on other unpaired datasets.
![All text](https://github.com/Oli-iver/MDMS/blob/main/figs/unpaired.png)

## Training
```
# in {path_to_this_repo}/,
$ python train_diffusion.py
```
Detailed training instructions will be updated soon.

