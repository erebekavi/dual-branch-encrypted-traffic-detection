# Dual-Branch Multimodal Deep Learning for Encrypted Traffic & Zero-Day Detection

**Research Paper:** *Dual-Branch Multimodal Deep Learning Framework for Encrypted Traffic Analysis and Zero-Day Anomaly Detection in Next-Generation Networks*

## Overview

This repository contains research on a dual-branch multimodal deep learning framework for encrypted traffic analysis and zero-day anomaly detection without requiring traffic decryption.

The framework combines two complementary representations of network traffic:

- **Temporal Branch** — captures packet-level dynamics such as inter-arrival times and burst sizes using 1D CNNs.
- **Statistical Branch** — analyzes global flow characteristics using an MLP.
- **Feature Fusion** — combines temporal and statistical representations.
- **Focal Loss** — addresses class imbalance and emphasizes difficult samples.
- **SHAP Explainability** — provides interpretable insights into model predictions.

## Research Objectives

- Analyze encrypted network traffic without decrypting payloads.
- Capture temporal and statistical traffic characteristics.
- Combine multiple traffic representations through multimodal learning.
- Investigate detection of previously unseen or zero-day attack patterns.
- Address class imbalance using focal loss.
- Improve model interpretability using SHAP.
- Explore practical use for network security monitoring.

## Proposed Architecture

```text
                    Encrypted Network Traffic
                              |
              +---------------+---------------+
              |                               |
              v                               v
       Temporal Branch                Statistical Branch
              |                               |
       Packet Dynamics                 Flow Statistics
              |                               |
            1D CNN                           MLP
              |                               |
              +---------------+---------------+
                              |
                              v
                       Feature Fusion
                              |
                              v
                       Deep Classifier
                              |
                              v
                      Anomaly Detection
                              |
                              v
                     SHAP Explainability
```

## Methodology

1. Encrypted traffic collection
2. Packet and flow preprocessing
3. Temporal feature extraction
4. Statistical feature extraction
5. Temporal representation learning using 1D CNN
6. Statistical representation learning using MLP
7. Feature fusion
8. Focal-loss-based optimization
9. Anomaly classification
10. SHAP-based explainability
11. Performance evaluation

## Datasets

The research considers publicly available network traffic datasets, including:

- **CICIDS2019**
- **USTC-TFC2016**

These datasets are considered for evaluating encrypted traffic analysis and anomaly detection scenarios.

## Evaluation Metrics

Potential evaluation metrics include:

- Accuracy
- Precision
- Recall
- Macro F1-score
- Per-class F1-score
- Confusion Matrix
- False Positive Rate
- Detection Rate
- Inference Latency
- AUROC
- AUPRC

## Zero-Day Evaluation

A rigorous zero-day evaluation should separate known attack patterns used during training from previously unseen attack categories used during testing.

```text
Known Traffic / Attacks
          |
       Training
          |
        Model
          |
Previously Unseen Attack
          |
       Evaluation
```

## Experimental Design

The proposed framework can be compared against:

- Traditional machine-learning approaches
- Temporal-only models
- Statistical-only models
- The proposed dual-branch architecture

Ablation studies can evaluate the contribution of individual components:

```text
Statistical Branch Only
          |
Temporal Branch Only
          |
Temporal + Statistical
          |
Temporal + Statistical + Fusion
          |
Full Model + SHAP
```

## Target Environments

The framework is designed with modern encrypted networking environments in mind, including:

- Enterprise networks
- 5G networks
- IoT environments
- Cloud infrastructure
- Edge computing
- TLS 1.3
- HTTP/3 and QUIC

## Repository Structure

```text
dual-branch-encrypted-traffic-detection/
|
+-- paper/
|   +-- research-paper.pdf
|
+-- figures/
|   +-- architecture.png
|
+-- README.md
+-- CITATION.cff
+-- LICENSE
+-- .gitignore
```

Additional directories such as `src/`, `models/`, `datasets/`, `notebooks/`, and `results/` can be added when the implementation and experimental evaluation are released.

## Research Paper

**Zenodo:** https://zenodo.org/records/21924391

## Citation

```bibtex
@misc{kavi2026dualbranch,
  author       = {Nithveen Kavi P},
  title        = {Dual-Branch Multimodal Deep Learning Framework for
                  Encrypted Traffic Analysis and Zero-Day Anomaly Detection
                  in Next-Generation Networks},
  year         = {2026},
  publisher    = {Zenodo},
  url          = {https://zenodo.org/records/21924391}
}
```

## Author

**Nithveen Kavi P**  
Founder — **EFLabs Pvt. Ltd.**

### Research Interests

- Artificial Intelligence
- Machine Learning
- Deep Learning
- Cybersecurity
- Cyber Defence
- Network Security
- Explainable AI
- Intelligent Security Systems

## Research Organization

### EFLabs Pvt. Ltd.

This research was carried out under the research and development initiatives of **EFLabs Pvt. Ltd.**

EFLabs focuses on technology development and research across areas including:

- Artificial Intelligence
- Machine Learning
- Software Development
- Automation
- Cybersecurity
- Research & Development

## Acknowledgment

This research was carried out under the research and development initiatives of **EFLabs Pvt. Ltd.**, providing a technical environment for exploring practical applications of artificial intelligence, deep learning, and cybersecurity.

The research also acknowledges the open-source research community and publicly available datasets, tools, and frameworks supporting research in artificial intelligence and cybersecurity.

## Research Status

**Status:** Research / Framework Development

This repository documents the proposed research framework, methodology, and associated research materials.

Experimental implementation, trained models, datasets, and benchmark results will be added as they become available.

## Ethical and Responsible Use

This project is intended for **academic, defensive cybersecurity, and research purposes**.

The framework is designed to support:

- Network anomaly detection
- Security monitoring
- Threat research
- Defensive analysis
- Cybersecurity research

It should not be used to conduct unauthorized activity against networks, systems, or individuals.

## License

This repository is intended for academic and research use.

See the `LICENSE` file for the specific terms governing the use, modification, and distribution of the repository contents.

## Keywords

`Cybersecurity` `Network Security` `Encrypted Traffic` `Zero-Day Detection` `Anomaly Detection` `Deep Learning` `Multimodal Learning` `CNN` `MLP` `SHAP` `Explainable AI` `TLS 1.3` `HTTP/3` `QUIC` `Cyber Defence` `Machine Learning`

---

**Research • Artificial Intelligence • Cybersecurity • Deep Learning**
