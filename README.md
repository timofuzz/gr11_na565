[pypi-ver-102]: https://img.shields.io/pypi/v/spconv-cu102
[pypi-url-102]: https://pypi.org/project/spconv-cu102/
[pypi-download-102]: https://img.shields.io/pypi/dm/spconv-cu102

# This is the repo for Group 11 final project

Download trained models and outputs are here:
https://drive.google.com/drive/folders/1QRNqA9w0oqielCvK3jleMs6Sw4Hi1bgx?usp=sharing

The algorithms were trained and test on the Great Lakes cluster with the following Anaconda environment: Python 3.9, Cuda 10.2, with installed requirements.txt. 

Once the environment is set up, install spconv (https://github.com/traveller59/spconv):

| CUDA 10.2 | [![PyPI Version][pypi-ver-102]][pypi-url-102] | ```pip install spconv-cu102```| [![pypi monthly download][pypi-download-102]][pypi-url-102]| 

Once these steps are complete, install the setup.py file via
```python
python setup.py develop
```
Set up the KITTI data in the following matter

```
Parent Folder
├── data
│   ├── kitti
│   │   │── ImageSets
│   │   │── training
│   │   │   ├──calib & velodyne & label_2 & image_2 & depth_2
│   │   │── testing
│   │   │   ├──calib & velodyne & image_2
├── pcdet
├── tools
```

## Training & Testing


### Test and evaluate the pretrained models
* Test with a pretrained model: 
```shell script
python test.py --cfg_file ${CONFIG_FILE} --batch_size ${BATCH_SIZE} --ckpt ${CKPT}
```

### Train a model

Train with a single GPU:
```shell script
python train.py --cfg_file ${CONFIG_FILE}
```
