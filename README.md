## Text classification algorithm for the Reuters 21578 dataset

### To install all dependencies on ubuntu 16.04 run:

(Before you ask me how to install on your os. You can always start a docker container using 'docker run -it ubuntu:16.04 /bin/bash' and copy and run the scripts in there.)

sudo apt-get update

sudo apt-get install python3 python3-dev python3-pip python3-h5py build-essential

sudo pip3 install pip --upgrade

sudo pip3 install keras sklearn nltk gensim numpy https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-0.10.0-cp35-cp35m-linux_x86_64.whl --upgrade

### 1. Run the doc2vec training script to generate the doc2vec model
python3 reuters-doc2vec-train.py

### 2. Run the classifier training script to generate the classifier model
python3 reuters-classifier-train.py

### 3. Run the prediction script to view the predicted labels and the original labels
python3 reuters-predict.py