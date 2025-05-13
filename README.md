# ants-docker

A Dockerfile for **ANTs 2.3.1** (Conda-based) with:

* **HCP Pipelines** cloned at `/opt/HCPpipelines`
* **MNI152 templates** downloaded into `/atlas`

---

## Build

```bash
docker build -t brainlife/ants-docker:2.3.1 .
```

---

## Run (Docker)

```bash
docker run --rm -it \
  brainlife/ants-docker:2.3.1 \
  <your_command>
```

---

## Run (Singularity)

### From your local Docker image

```bash
singularity build ants-2.3.1.sif \
  docker-daemon://brainlife/ants-docker:2.3.1

singularity exec \
  --bind $(pwd):/workspace \
  ants-2.3.1.sif \
  <your_command>
```

### Directly from Docker Hub

```bash
singularity exec \
  docker://brainlife/ants-docker:2.3.1 \
  <your_command>
```

---

## Contents

* **ANTs 2.3.1** installed in a Conda env named `ants-2.3.1`
* **HCP Pipelines** repo: `/opt/HCPpipelines`
* **MNI152** templates unpacked under `/atlas`
