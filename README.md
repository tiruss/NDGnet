# PMNet: Coarse to Fine: Progressive and Multi-Task Learning for Salient Object Detection

Pytorch implementation of "Coarse to Fine: Progressive and Multi-Task Learning for Salient Object Detection"

<img src="Figure/overall_net.png">

### Qualitative Evaluation

<img src="Figure/qualitative.png">

<img src="Figure/inside.png">

<img src="Figure/multi_ablation.png">

### Quantative Evaluation

<img src="Figure/table.PNG">

<img src="Figure/fm_pr.png">

## Getting Started
### Installation

- Clone this repository
```
git clone https://github.com/tiruss/PMNet.git
```

- You can install all the dependencies by 
```
pip install -r requirements.txt
```

### Download datasets

- Download training datasets [[DUTS-TR]](http://saliencydetection.net/duts/download/DUTS-TR.zip) from the link 

- Download [[HKU-IS]](https://sites.google.com/site/ligb86/hkuis) for test from the link 

- Other datasets can download from the link [[sal_eval_toolbox]](https://github.com/ArcherFMY/sal_eval_toolbox) Thank you for the awesome evaluation toolbox!

### Run experiments from pretrained weight

- Download pretrained weight from the link. [[Google Drive]](https://drive.google.com/open?id=11PQySPgimyZ011FOjmxGBOGcyti1Z0rH) [[Baidu Drive]]() Baidu drive will be updated soon.

- If you want CRF for postprocessing, download [PyCRF](https://pypi.org/project/pydensecrf/) from the link.

- Pre-computed saliency maps can download from the link. [[Google Drive]](https://drive.google.com/open?id=1im9vBnMN5zLXH-NwHzsosltYyKfyRsyz) [[Baidu Drive]]() Baidu drive will be updated soon.

### Train from scratch

- DUTS-TR is our traning set for pair comparison

- Run 

```
python Train.py --img_dir [DUTS-TR img dir] --gt_dir [DUTS-TR label dir] --epoch --batch_size --gpus --down_scale
```
