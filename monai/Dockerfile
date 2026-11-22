FROM pytorch/pytorch:2.5.1-cuda12.4-cudnn9-runtime

RUN pip install --no-cache-dir \
    monai nibabel pydicom SimpleITK scikit-image \
    pandas einops tqdm matplotlib tensorboard jupyterlab

WORKDIR /workspace
EXPOSE 8888
CMD ["jupyter", "lab", "--ip=0.0.0.0", "--no-browser", "--allow-root"]
