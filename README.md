# ants-docker

This repository contains a Dockerfile for ANTs 2.3.1 (Conda-based), plus:
- HCP Pipelines clone
- MNI152 template download

Build with:
```bash
docker build -t brainlife/ants-docker:2.3.1 .
```

Run with:
```bash
docker run --rm -it brainlife/ants-docker:2.3.1 <your_command>
```
Or with Singularity with:
```bash
singularity exec -e docker://brainlife/ants:2.3.1 <your_command>
```
