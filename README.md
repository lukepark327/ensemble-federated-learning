# ensemble-federated-learning
Decentralized Federated Learning based-on Ensemble Paradigm

---

# Environment

## System

```
$ nvidia-smi
Sat Jan  9 11:54:14 2021
+-----------------------------------------------------------------------------+
| NVIDIA-SMI 450.57       Driver Version: 450.57       CUDA Version: 11.0     |
|-------------------------------+----------------------+----------------------+
| GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
| Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
|                               |                      |               MIG M. |
|===============================+======================+======================|
|   0  GeForce RTX 208...  Off  | 00000000:09:00.0 Off |                  N/A |
|  0%   47C    P8     8W / 250W |      6MiB /  7982MiB |      0%      Default |
|                               |                      |                  N/A |
+-------------------------------+----------------------+----------------------+
|   1  GeForce RTX 208...  Off  | 00000000:41:00.0 Off |                  N/A |
|  0%   46C    P8    14W / 250W |     19MiB /  7979MiB |      0%      Default |
|                               |                      |                  N/A |
+-------------------------------+----------------------+----------------------+

+-----------------------------------------------------------------------------+
| Processes:                                                                  |
|  GPU   GI   CI        PID   Type   Process name                  GPU Memory |
|        ID   ID                                                   Usage      |
|=============================================================================|
+-----------------------------------------------------------------------------+
```

## Setup

Using [pytorch docker](https://hub.docker.com/r/pytorch/pytorch/tags?page=1&ordering=last_updated) @ `pytorch:1.7.0-cuda11.0-cudnn8-devel` and nvidia-docker.

```
$ docker pull pytorch/pytorch:1.7.0-cuda11.0-cudnn8-devel
$ nvidia-docker run -i -t --name pytorch -v <HOMEPATH>:/workspace pytorch/pytorch:1.7.0-cuda11.0-cudnn8-devel /bin/bash
```
