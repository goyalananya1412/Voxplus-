# VoxPulse: Contrastive Speech Analytics & Temporal Flaw Grounding

> **Multimodal AI Hackathon 2026 — Track C Submission**
VoxPulse - AI-Based Speech Quality Analyzer
VoxPulse is an advanced speech analysis prototype designed to evaluate public speaking and spoken delivery failures. By removing subjective human opinions, this system provides objective performance metrics and easily actionable feedback through audio signal analytics.
🔗 Project Quick Links
Live Web Dashboard: Your Vercel Link Here
Demo Video (YouTube): Your YouTube Link Here (Note: Insert your demo video link here)
🛠️ Software Architecture (Decoupled Design)
To make our project extremely lightweight and scalable, we have utilized a decoupled architecture:
Frontend (UI Layer): Built with vanilla HTML5, CSS3, and JavaScript, deployed on Vercel for instantaneous rendering.
Backend (Analytics Brain): A standalone Python pipeline that processes audio waveforms in a standard 16 kHz mono environment.
Data Bridge: The frontend and backend communicate with each other via a structured JSON payload (evaluation_results.json).
📊 Engineered Contrastive Dataset
Prioritizing data quality over quantity, we have prepared a gradient spectrum of flaws on a single shared rhetorical transcript using ElevenLabs stability parameters:
speech_01_normal.mp3 - Standard baseline reference model.
speech_02_pause.mp3 - Monotone track with awkward structural silence breaks.
speech_03_low_mumbling_volume.mp3 - Low energy whisper and inaudible speech track.
speech_04_rushed.mp3 - Hyper-accelerated track with syntax distortion.
⚙️ Core Technical Features
Advanced Feature Extraction: Logarithmic Loudness Envelope (RMS dB) extraction using the librosa library and continuous F0 pitch tracking via the pYIN algorithm.
Temporal Grounding: Extracting precise forced word alignment using the torchaudio MMS_FA CTC model and isolating exact millisecond deviation regions using Dynamic Time Warping (DTW).
Causal Feedback & AI Coach: A JSON-parsed visual dashboard that translates numerical errors into color-coded Causal Explanation Cards and features an interactive AI Chat Assistant box.
👥 Team Matrix & Roles
Ishita (Lead Data Engineer): Dataset sourcing, text transcription alignment, and baseline generation.
Ananya (Senior Backend Developer): Core Python audio feature processing and mathematical framework mapping.
Anshika (Application UI Developer): HTML/JS responsive web panel building, Vercel deployment, and AI assistant integration.
