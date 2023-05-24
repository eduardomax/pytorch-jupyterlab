# pytorch-jupyterlab
For my personal use.
The idea is to have a docker image with:
- pytorch 1.12.1
- cuda11.3
- cudnn8
- devel
- jupyterlab

# Docker build
```
docker build -t pytorch-jupyterlab:lastest .
```

# Run
```
docker start pytorch-jupyterlab
```

Then, you can access via url: http://localhost:8888/

# Jupyterlab
The current port using is 8888.

