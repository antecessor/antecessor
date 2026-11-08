<div align="center">

# Mohammad Reza Mohebbian, PhD
### Machine Learning Engineer · Kernels → Training → Serving → Monitoring

PhD in Electrical & Computer Engineering (University of Saskatchewan).  
I build production AI systems end-to-end: custom GPU kernels, RL / LLM / vision training, ONNX export, low-latency serving, and online model monitoring.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mr-mohebbian-1a236952/)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/channel/UCn9Rujwh7SfHF2RRvy_ks-g)
[![ORCID](https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white)](https://orcid.org/0000-0003-2645-4425)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/antecessor)

Toronto, Canada · Open to collaboration on applied AI systems

</div>

---

## Operating principle

```text
data → representations → train (SFT / RL) → offline eval →
export (ONNX / TensorRT) → serve → drift & quality monitors → iterate
```

I treat model work as systems engineering: Triton kernels where the hot path matters, reproducible training for LLMs and vision, hard offline gates, then production monitors that catch silent failure modes before users do.

---

## Systems depth

| Layer | What I actually do |
| --- | --- |
| **GPU / kernels** | Write & profile **Triton** kernels for attention, fused ops, and custom vision/signal blocks; cut latency & memory without rewriting whole stacks |
| **LLM training** | SFT / LoRA / adapters, preference data, **RL for LLMs** (PPO / GRPO-style loops, reward models, KL control), eval harnesses that survive A/B |
| **Vision training** | Segmentation, OCR, embeddings; **RL / policy fine-tuning** for vision agents & closed-loop perception when supervised labels are thin |
| **Export & runtime** | **ONNX** graphs, opset debugging, dynamic axes, quantization (INT8 / FP16), TensorRT / ONNX Runtime paths for prod |
| **Serving** | FastAPI / gRPC, Docker, Kubernetes, canary & shadow traffic, batching & GPU utilization under SLO |
| **Prod monitoring** | Latency / throughput / GPU mem, prediction drift, embedding drift, calibration, data quality, alert → rollback playbooks |

Industry work includes production ML at **Cubby**, **Procore**, and **Yardi**, plus applied research collaborations (e.g. MRI motion detection with Philips Canada).

---

## What I ship

| Domain | What I build |
| --- | --- |
| **Computer Vision** | Segmentation, OCR / document understanding, MRI artifact detection, endoscopy analytics, technical-drawing embeddings |
| **Signals & Biomed** | Fetal ECG extraction (CycleGAN + attention), PPG → BP, sEMG force / gesture, anomaly detection with active learning |
| **NLP / LLMs** | LLM fine-tuning (e.g. MPT-7B), transformers from scratch, RLHF-style preference loops, retrieval-aware document pipelines |
| **Systems / MLOps** | Triton kernels · ONNX export · MLflow · CircleCI · ArgoCD · K8s serving · online drift & quality monitors |

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
Hands-on LLM fine-tuning — data prep, adapters, training loops, and eval with a production mindset.

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

### [`Transformers`](https://github.com/antecessor/Transformers) · [`PPO-RL`](https://github.com/antecessor/PPO-RL)
Attention from scratch + PPO reinforcement learning — building blocks for LLM / policy training loops.

</td>
</tr>
</table>

---

## Production ML loop (how I think about “done”)

```text
1. Train     SFT / RL for LLM & vision · reward design · offline metrics
2. Harden    Triton hot paths · ONNX export · quantize · latency budget
3. Serve     K8s · canary · autoscaling · GPU packing
4. Monitor   p50/p99 · drift · calibration · data schema · alert → rollback
5. Improve   shadow eval · preference / RL updates · ship again
```

Silent model failure is still failure. Production-grade ML means dashboards and gates, not just a checkpoint in S3.

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
Languages     Python · CUDA/Triton · Java · C++ · MATLAB · SQL
Train         PyTorch · Transformers · LoRA/SFT · PPO / RL for LLMs & vision
Vision        OpenCV · Mask2Former · docTR · CNNs · GANs · SSL (BYOL)
Compile       ONNX · ONNX Runtime · TensorRT · quantization (FP16/INT8)
Kernels       Triton · fused attention / custom ops · Nsight profiling
Serve         FastAPI · gRPC · Docker · Kubernetes · ArgoCD · CircleCI
Observe       MLflow · Prometheus/Grafana-style SLOs · drift & quality monitors
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

- **Triton kernels** on inference hot paths (attention, fused vision/signal ops)  
- **RL training loops** for LLMs and vision policies with stable reward + KL control  
- **ONNX → runtime** pipelines that keep numerical parity under quantization  
- **Production monitors**: latency SLOs, prediction/embedding drift, calibration, rollback  
- Teaching applied systems ML on [YouTube](https://www.youtube.com/channel/UCn9Rujwh7SfHF2RRvy_ks-g)

---

<div align="center">

**If you care about kernels, RL training, ONNX runtimes, and models that stay honest in prod — let's talk.**

`antecessor` · Canada · Machine Learning Engineer

</div>
