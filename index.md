---
layout: default
title: "Barry Cheng — Portfolio"
---
Welcome! I’m **Barry Cheng** from Taiwan, an electric guitarist with 15+ years of playing experience and over 5 years of machine learning research experience in the music industry. My work sits at the intersection of **music performance**, **composition**, and **music AI research**, with a particular focus on guitar tone, expressive performance, and musician-centric tools.

This page collects selected examples of my **musical** and **technical** work.

- 🎸 Band: *Diving Raccoon* (instrumental math rock / progressive rock)  
- 🧠 Research focus: music representation learning & generative guitar tone modeling  

---

## Music & Audio Projects

### 1. Diving Raccoon — Instrumental Math Rock / Progressive Rock

**Role:** Founder, lead guitarist, primary composer  

I founded **Diving Raccoon**, an instrumental math-rock / progressive-rock band exploring rhythm, harmony, and narrative expression without lyrics. The band has performed at **50+ live shows across Taiwan**, shaping my experience in arrangement, dynamics, and ensemble communication.

#### (a) *Connie’s Forest* — Single (2023)

- **Link:** [https://music.youtube.com/watch?v=ePmPhZQ6ac0](https://music.youtube.com/watch?v=ePmPhZQ6ac0)  
- **My contribution:**
  - Composed guitar parts and main structure  
  - Performed electric guitar and contributed to arrangement/production  
- **Impact:** Helped define the band’s sound and led to an invitation to perform at **The Next Big Thing**, one of Taiwan’s most influential emerging-artist stages.

#### (b) *Arctica* — EP (2024)

- **Link:** [https://music.youtube.com/playlist?list=OLAK5uy_kwGbhyMvgb_N0VXnKn-NSCVKg9AeFaT6Y](https://music.youtube.com/playlist?list=OLAK5uy_kwGbhyMvgb_N0VXnKn-NSCVKg9AeFaT6Y)  
- **My contribution:**
  - Conceptualized the EP around the ancient polar continent “Arctica”  
  - Composed guitar parts and main structure  
  - Performed electric guitar and contributed to arrangement/production  
- **Impact:** Received enthusiastic responses from listeners and the indie community, promoted the band to wider audience.

---

## Music Technology & Research Projects

### 2. Zero-Shot Amplifier Modeling (2024)

**Demo video:** [https://www.youtube.com/watch?v=IVN9JTTxZkk](https://www.youtube.com/watch?v=IVN9JTTxZkk)  

A research and engineering project I developed in Positive Grid, focused on modeling **unseen guitar amplifiers** using only a brief **reference audio clip**, enabling instant tone capture without per-amp training.

#### Core idea
- Learn a shared **Tone Embedding** space capturing timbral characteristics.  
- Use this embedding to condition a **hypernetwork**, which adjusts a neural generator to reproduce the target amp’s behavior.  
- Enables:
  - Zero-shot modeling  
  - Tone interpolation  
  - Intuitive user-controlled timbre shaping  

#### My contributions
- **Architecture & training**
  - Designed the tone-embedding model, hypernetwork, and GCN-based generator  
  - Built datasets, training pipeline, and evaluation metrics  
- **Real-time integration**
  - Integrated model into a **JUCE / Eigen** plugin  
  - Implemented **ONNX-powered** real-time tone capture  
  - Optimized latency for live performance  
- **User experience**
  - Designed tone-editing controls and interactive UI  
  - Focused on musician-friendly workflows  
- **Impact**
  - Prototype developed in ~3 months  
  - Integrated into company roadmap for a **2026 commercial release**

