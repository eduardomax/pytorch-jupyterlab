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
docker run --name pytorch-jupyterlab --ipc=host --gpus all -p 8888:8888 -e JUPYTER_TOKEN={DEFINE_YOUR_PASSWORD} -v {YOUR_CURRENT_PROJECT_FOLDER}:/tmp -w /tmp -it pytorch-jupyter
```
#
```
docker start pytorch-jupyterlab
```

Then, you can access via url: http://localhost:8888/

# Jupyterlab
The current port using is 8888.

