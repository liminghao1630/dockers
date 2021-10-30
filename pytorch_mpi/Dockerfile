FROM pytorch/pytorch:1.10.0-cuda11.3-cudnn8-devel
RUN apt-get update -y && \
    apt-get install -y --no-install-recommends git curl gcc g++ && \
    apt-get install -y --no-install-recommends libopenmpi-dev openmpi-bin openmpi-common openmpi-doc  && \    
    rm -rf /var/lib/apt/lists/*

# RUN apt-get update -y && \
#     apt-get install -y --no-install-recommends libnccl2=2.9.6-1+cuda11.3 libnccl-dev=2.9.6-1+cuda11.3