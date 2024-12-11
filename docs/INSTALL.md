# Installation

### Requirements
All the codes are tested in the following environment:
* Linux (tested on Great Lakes Redhat 8.8)
* Python 3.6+
* PyTorch 1.1 or higher (tested on PyTorch 1.1, 1,3, 1,5~1.10)
* CUDA 9.0 or higher (PyTorch 1.3+ needs CUDA 9.2+)
* [`spconv v2.x`](https://github.com/traveller59/spconv)


### Install `pcdet v0.5`
Install latest `spconv v2.x` with pip, see the official documents of [spconv](https://github.com/traveller59/spconv).


Install pcdet library and its dependent libraries by running the following command:
```shell
python setup.py develop
```
