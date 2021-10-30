FROM hangbo/pytorch:1.8.0-superbench

RUN apt-get update -y && \
    apt-get install -y --no-install-recommends git curl gcc g++ && \
    apt-get install -y --no-install-recommends libopenmpi-dev openmpi-bin openmpi-common openmpi-doc && \    
    rm -rf /var/lib/apt/lists/*

RUN pip install -U pip && pip install natsort tensorboard tensorboardX nltk h5py numpy pybind11 fastwer sentencepiece && \
    pip install -v --no-cache-dir --global-option="--cpp_ext" --global-option="--cuda_ext" 'git+https://github.com/NVIDIA/apex.git'    