# Options Selected:
* OpenVino
* Rest API

MultiModalClassifier
This is a project repo for multi-modal deep learning classifier with popular models from Tensorflow and Pytorch. The goal of these baseline models is to provide a template to build on and can be a starting point for any new ideas, applications. If you want to learn basics of ML and DL, please refer this repo: https://github.com/lkk688/DeepDataMiningLearning.

Package setup
Install this project in development mode

(venv38) MyRepo/MultiModalClassifier$ python setup.py develop
After the installation, the package "MultimodalClassifier==0.0.1" is installed in your virtual environment. You can check the import

>>> import TFClassifier
>>> import TFClassifier.Datasetutil
>>> import TFClassifier.Datasetutil.Visutil

If you went to uninstall the package, perform the following step

(venv38) lkk@cmpeengr276-All-Series:~/Developer/MyRepo/MultiModalClassifier$ python setup.py develop --uninstall
Code organization
DatasetTools: common tools and code scripts for processing datasets
TFClassifier: Tensorflow-based classifier
myTFDistributedTrainerv2.py: main training code
myTFInference.py: main inference code
exportTFlite.py: convert form TF model to TFlite
TorchClassifier: Pytorch-based classifier
myTorchTrainer.py: Pytorch main training code
myTorchEvaluator.py: Pytorch model evaluation code

#Procedure:

Dataset: ASIRRA(animal species image recognition) dataset includes 25,000 images

