<div align="center">

# Mohammad Reza Mohebbian, PhD
### Machine Learning Engineer · Train → Evaluate → Ship to Prod

PhD in Electrical & Computer Engineering (University of Saskatchewan).  
I design, train, and productionize deep learning systems — from research-grade models to monitored services in the wild.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mr-mohebbian-1a236952/)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/channel/UCn9Rujwh7SfHF2RRvy_ks-g)
[![ORCID](https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white)](https://orcid.org/0000-0003-2645-4425)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/antecessor)

Toronto, Canada · Open to collaboration on applied AI systems

</div>

---

## Operating principle

```text
data → features/representations → training loops → offline eval →
online serving → observability → iterate
```

I treat model development as an engineering discipline: reproducible training, hard evaluation, latency/cost budgets, and deployment paths that survive contact with production traffic.

---

## What I ship

| Domain | What I build |
| --- | --- |
| **Computer Vision** | Segmentation, OCR / document understanding, MRI artifact detection, endoscopy analytics, technical-drawing embeddings |
| **Signals & Biomed** | Fetal ECG extraction (CycleGAN + attention), PPG → BP, sEMG force / gesture, anomaly detection with active learning |
| **NLP / LLMs** | LLM fine-tuning (e.g. MPT-7B), transformers from scratch, retrieval-aware document pipelines |
| **MLOps** | Dockerized training & inference, experiment tracking (MLflow), CI (CircleCI), GitOps (ArgoCD), K8s serving |

Industry work includes production ML at **Cubby**, **Procore**, and **Yardi**, plus applied research collaborations (e.g. MRI motion detection with Philips Canada).

---

## Featured systems

<table>
<tr>
<td width="50%" valign="top">

### [`FECGCycleGAN`](https://github.com/antecessor/FECGCycleGAN)
Attention-based CycleGAN for fetal ECG extraction from maternal ECG.  
Published in *IEEE JBHI* — ~98% R² mapping, ≥99% F1 fetal QRS detection.

</td>
<td width="50%" valign="top">

### [`mpt_7b_fine_tuning`](https://github.com/antecessor/mpt_7b_fine_tuning)
Hands-on LLM fine-tuning notebooks — data prep, adapters, training loops, and eval for production-minded LLM work.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [`MRI_Motion_Classification`](https://github.com/antecessor/MRI_Motion_Classification)
Generate + detect MRI motion artifacts; stacked ensemble severity classification for clinical imaging pipelines.

</td>
<td width="50%" valign="top">

### [`Wavenet`](https://github.com/antecessor/Wavenet) · [`TabTransformer`](https://github.com/antecessor/TabTransformer)
From-scratch PyTorch implementations of WaveNet and TabTransformer — architecture literacy, not just API usage.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [`FECG_Anomaly_ActiveLearning`](https://github.com/antecessor/FECG_Anomaly_ActiveLearning)
Active-learning loop for FECG anomaly annotation → model calibration → low-confidence sampling → fine-tune.

</td>
<td width="50%" valign="top">

### [`Transformers`](https://github.com/antecessor/Transformers) · [`BloodPressure_Estimation`](https://github.com/antecessor/BloodPressure_Estimation)
Attention implementations and PPG-only blood-pressure estimation — signal ML with a deployment mindset.

</td>
</tr>
</table>

---

## Research signal

- **35+** peer-reviewed journal & conference papers · **3** book chapters  
- Focus: health informatics, medical imaging, biomedical signal processing, pattern recognition  
- Selected work: [Attention-based CycleGAN for FECG (IEEE JBHI)](https://doi.org/10.1109/JBHI.2021.3111879) · [arXiv:2011.12138](https://arxiv.org/abs/2011.12138)  
- Full record: [ORCID 0000-0003-2645-4425](https://orcid.org/0000-0003-2645-4425)

<details>
<summary><b>Selected publications</b></summary>

- Mohebbian et al., *Fetal ECG Extraction From Maternal ECG Using Attention-Based CycleGAN*, IEEE JBHI, 2022  
- Mohebbian, Marateb, Wahid, *Semi-supervised active transfer learning for fetal ECG arrhythmia detection*, CMPB Update, 2023  
- Mohebbian et al., *Classifying MRI motion severity using a stacked ensemble approach*, Magnetic Resonance Imaging, 2021  
- Mohebbian & Wahid, *ECG compression using optimized B-spline*, Multimedia Tools and Applications, 2023  
- Mohebbian et al., *Automated Detection of Bleeding in Capsule Endoscopy Using On-Chip Multispectral Imaging Sensors*, IEEE Sensors Journal, 2021  

</details>

---

## Stack I actually use

```text
Languages   Python · Java · C++ · MATLAB · SQL
DL          PyTorch · TensorFlow · Transformers · CNNs · GANs · SSL (BYOL)
CV / OCR    OpenCV · Mask2Former · docTR · embeddings / dVAE-style reps
Signals     1-D CNNs · WaveNet · BSS / adaptive filtering · active learning
Serving     FastAPI · Docker · Kubernetes · ArgoCD · CircleCI · MLflow
```

---

## GitHub telemetry

<p align="center">
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=antecessor&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub stats" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=antecessor&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=antecessor&theme=tokyonight&hide_border=true" alt="GitHub streak" />
</p>

---

## Currently optimizing for

- **Reliable training → serving loops** with clear offline/online metrics  
- **Document & drawing intelligence** (OCR, segmentation, embedding search) in production  
- **LLM fine-tuning** that respects cost, latency, and evaluation rigor  
- Teaching applied ML clearly on [YouTube](https://www.youtube.com/channel/UCn9Rujwh7SfHF2RRvy_ks-g)

---

<div align="center">

**If you care about models that leave the notebook and earn their keep in prod — let's talk.**

`antecessor` · Canada · Machine Learning Engineer

</div>
