# Joint action and pose estimation
## Action recognition using pose estimation

#### Aim of this project is to automatically recognize human actions based on analysis of the body landmarks using pose estimation.

1. Implementation of CNN based Pose Estimation model

2. Implementation of NN based Action Recognition model

3. Action Recognition in videos

4. Testing your model on the evaluation dataset
 ## Requirements
 
 ```bash
pip install --upgrade --no-cache gdown
pip install -U scikit-learn
pip install matplotlib
pip install numpy
pip install pandas
pip install tensorflow
pip install keras
pip install imageio-ffmpeg
```
## Download the dataset
```bash
wget --load-cookies /tmp/cookies.txt "https://docs.google.com/uc?export=download&confirm=$(wget --quiet --save-cookies /tmp/cookies.txt --keep-session-cookies --no-check-certificate 'https://docs.google.com/uc?export=download&id=FILEID' -O- | sed -rn 's/.*confirm=([0-9A-Za-z_]+).*/\1\n/p')&id=12FQpzkwwf53hhvWUsffLWTqgtZDcAOXJ" -O Data.zip && rm -rf /tmp/cookies.txt
```
## Unzip the dataset
```bash
unzip -qq Data.zip
rm Data.zip
```

Data
```bash
$ tree
Data
├── Action_Dataset
│   ├── Waving.mp4
│   ├── action_joints.csv
│   └── images
└── Pose_Dataset
    ├── test
    ├── test_joints_coords.csv
    ├── train
    └── train_joints_coords.csv

5 directories, 4 files
```


### Conclusion
This project successfully constructed a Pose Estimation model based on Convolutional Neural Networks (CNN) and an Action Recognition model based on Neural Networks (NN). After that, the Action Recognition model was combined with the Pose Estimation model to detect actions in films using pose joints predicted by CNN. The project report contains a detailed.ipynb file including the code as well as descriptions of the models' architecture, data preparation, and assessment measures. The model was evaluated on an assessment dataset, and the results show that the models are capable of reliably detecting human actions in films.
