<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/brand/brainlife-mark-on-dark.svg">
    <img src=".github/brand/brainlife-mark-on-light.svg" alt="brainlife.io" width="140">
  </picture>
</p>

<h1 align="center">ants-docker</h1>

<p align="center">
  ANTs 2.3.1 with the HCP Pipelines and MNI templates, in one container.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-maintained-blue.svg" alt="Status: maintained">
  <a href="https://brainlife.io"><img src="https://img.shields.io/badge/brainlife.io-site-3b9fd0.svg" alt="brainlife.io"></a>
  <a href="https://brainlife.io/docs"><img src="https://img.shields.io/badge/Docs-brainlife.io%2Fdocs-005981.svg" alt="Documentation"></a>
  <a href="https://doi.org/10.1038/s41592-024-02237-2"><img src="https://img.shields.io/badge/DOI-10.1038%2Fs41592--024--02237--2-e57536.svg" alt="Nature Methods paper"></a>
</p>

## 🧠 At a glance

| | |
|---|---|
| 🐳 **Image** | `brainlife/ants-docker:2.3.1` |
| 📦 **Contents** | ANTs 2.3.1 (Conda) · HCP Pipelines in `/opt/HCPpipelines` · MNI152 templates in `/atlas` |
| 🕰️ **Last change** | 2025-05-13 |

## 🚀 Build and run

```bash
docker build -t brainlife/ants-docker:2.3.1 .
docker run --rm -it brainlife/ants-docker:2.3.1 antsRegistration --version
```

## 🔗 Related

[dockerfiles](https://github.com/brainlife/dockerfiles) (other shared images, including `ants/`) · [abcd-spec](https://github.com/brainlife/abcd-spec)

## 📚 Citing

If you use brainlife.io in your work, please cite:

> Hayashi S, Caron BA, Heinsfeld AS, et al. brainlife.io: a decentralized and open-source cloud platform to support neuroscience research. *Nature Methods* 21:809–813 (2024). [doi:10.1038/s41592-024-02237-2](https://doi.org/10.1038/s41592-024-02237-2)

## 🤝 Contributing

Issues and pull requests are welcome in this repository. For help using brainlife.io, see the [documentation](https://brainlife.io/docs).

## ⚖️ License

This repository does not include a license file yet.

<p align="center"><sub>brainlife.io · Brain data across scales. One place to analyze, share and publish it. · The University of Texas at Austin</sub></p>
