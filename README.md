# VoxPulse: Contrastive Speech Analytics & Temporal Flaw Grounding

> **Multimodal AI Hackathon 2026 — Track C Submission**

VoxPulse is an advanced speech evaluation system that constructs a custom contrastive dataset of "ideal" vs. "flawed" speeches, maps acoustic stress points using time-series analysis, and delivers actionable, rubric-based feedback via an interactive dashboard[span_0](start_span)[span_0](end_span)[span_1](start_span)[span_1](end_span).

---

## 🚀 Project Overview
Evaluating competitive spoken performances—such as Declamation, Extemporaneous, and Persuasive Oratory—is inherently subjective[span_2](start_span)[span_2](end_span). Judges often balance vocal delivery against textual quality, causing inconsistent scoring[span_3](start_span)[span_3](end_span). VoxPulse solves this by pairing master speech recordings with intentionally flawed variants to analyze acoustic discrepancies (pitch, energy, pacing, and pause intervals) and pinpoint exact regions of delivery failure[span_4](start_span)[span_4](end_span)[span_5](start_span)[span_5](end_span).

---

## 📊 Custom Contrastive Dataset & Stress Testing
Following the hackathon requirements, our custom dataset features:
* **The "Good" Baseline:** Clean audio recordings and verified transcripts sourced from champion public speakers and prominent figures[span_6](start_span)[span_6](end_span).
* **The "Bad" Spectrum:** Synthesized and self-recorded variants of the exact same transcripts featuring controlled delivery flaws (monotone delivery, rushing, awkward pauses, and fading volume)[span_7](start_span)[span_7](end_span).
* **Dataset Access:** The complete structured dataset (audio files, transcripts, alignment labels, and JSON metadata) is accessible via our [Public Google Drive Link](YOUR_GOOGLE_DRIVE_LINK_HERE)[span_8](start_span)[span_8](end_span).

---

## 🛠️ Architecture & Tech Stack
* **Frontend:** Interactive web interface built using HTML, CSS, and JavaScript, deployed via Vercel for seamless audio/transcript uploads[span_9](start_span)[span_9](end_span).
* **Backend Engine:** Standalone Python processing engine handling advanced feature extraction (FFT, MFCCs, pitch/F0 contours, pause intervals) and forced alignment[span_10](start_span)[span_10](end_span).
* **Causal Explainability:** Translates raw mathematical deltas into structured, human-readable feedback regarding specific delivery flaws[span_11](start_span)[span_11](end_span).

---

## ⚡ Local Setup & Installation

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/oomyfriendganesha/Voxpulse-.git](https://github.com/oomyfriendganesha/Voxpulse-.git)
   cd Voxpulse-
   
