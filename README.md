# HMR Code Modified for Photo Wake Up Implementation

Photo Wake Up project: https://grail.cs.washington.edu/projects/wakeup/
Chung-Yi Weng, Brian Curless, Ira Kemelmacher-Shlizerman

Original HMR (End-to-end Recovery of Human Shape and Pose) GitHub: https://github.com/akanazawa/hmr
Angjoo Kanazawa, Michael J. Black, David W. Jacobs, Jitendra Malik
CVPR 2018

The following requirements are from the original HMR project: https://github.com/akanazawa/hmr

### Requirements
- Python 2.7
- [TensorFlow](https://www.tensorflow.org/) tested on version 1.3

### Installation

#### Setup virtualenv
```
virtualenv venv_hmr
source venv_hmr/bin/activate
pip install -U pip
deactivate
source venv_hmr/bin/activate
pip install -r requirements.txt
```
#### Install TensorFlow
With GPU:
```
pip install tensorflow-gpu==1.3.0
```
Without GPU:
```
pip install tensorflow==1.3.0
```

### Demo

1. Download the pre-trained models
```
wget https://people.eecs.berkeley.edu/~kanazawa/cachedir/hmr/models.tar.gz && tar -xf models.tar.gz
```

2. Run the demo
```
python PhotoWakeUpHMR/PhotoWakeUp.py -img_path data/coco1.png
```

Many thanks to the original authors contributions!!
