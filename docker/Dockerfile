FROM ubuntu:20.04

WORKDIR /code

ARG DEBIAN_FRONTEND=noninteractive


RUN apt-get update && apt-get install -y \
	git \
	vim \
	python3 \
	python-is-python3 \
	python3-pip

#RUN pip install cudatoolkit=10.2
RUN pip install torch==1.6.0 torchvision==0.7.0
RUN pip install scipy scikit-image matplotlib opencv-python
RUN pip install tensorboard tensorboardX
RUN pip install tqdm path.py

#apt-get install nvidia-cuda-toolkit
#git clone https://github.com/NVIDIA/apex
#cd apex


ARG DEBIAN_FRONTEND=dialog

WORKDIR leastereo

