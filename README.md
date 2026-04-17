# Speech & ASR Evaluations Index

Index of evaluations and experiments assessing Automatic Speech Recognition (ASR) and Speech-to-Text (STT) system performance under various conditions.

**Author:** Daniel Rosehill
**Related Index:** [Experiments-And-Evaluations-Index](https://github.com/danielrosehill/Experiments-And-Evaluations-Index)

---

## Evaluations

### Oct 2025 — Local Whisper Model Comparison

**Question:** What is the difference in accuracy between various Whisper models on local inference, and how do derivative engines compare against original Whisper?

**Links:** [GitHub](https://github.com/danielrosehill/Local-ASR-STT-Benchmark)

**Summary:** Benchmarked multiple Whisper model variants running locally on AMD GPU hardware (ROCm) through Speech Note on Ubuntu. Compared stock Whisper models of different sizes and derivative engines to identify the best-performing local STT option for the hardware.

---

### Nov 2025 — Long-Form Audio Transcription

**Question:** How do ASR systems perform on extended audio recordings compared to shorter clips?

**Links:** [GitHub](https://github.com/danielrosehill/Long-Form-Audio-Eval)

**Summary:** Single-shot STT benchmark focused on long-form audio. Evaluated how transcription quality degrades or holds up as recording length increases beyond typical short-clip evaluation sets.

---

### Nov 2025 — Podcast ASR Evaluation

**Question:** How accurately do ASR systems transcribe podcast-style audio?

**Links:** [Dataset](https://huggingface.co/datasets/danielrosehill/Podcast-ASR-Evaluation)

**Summary:** Evaluation of ASR performance on podcast recordings, testing how conversational speech patterns, multiple speakers, and natural audio quality affect transcription accuracy.

---

### Nov 2025 — STT System Comparison

**Question:** How do different STT systems compare head-to-head on the same audio inputs?

**Links:** [Space](https://huggingface.co/spaces/danielrosehill/STT-Comparison)

**Summary:** Side-by-side comparison of multiple STT systems on identical test audio, providing a direct performance comparison across providers.

---

### Nov 2025 — English-Hebrew Code-Switched Speech

**Question:** How well do standard STT systems handle code-switched English-Hebrew speech patterns common among English-speaking immigrants in Israel?

**Links:** [Dataset](https://huggingface.co/datasets/danielrosehill/English-Hebrew-Mixed-Sentences)

**Summary:** Created 516 audio-text pairs of English sentences with naturally interspersed Hebrew words across domains like government, healthcare, and documents. Tests how well ASR handles the kind of mixed-language speech typical of Anglophones living in Israel.

---

### Nov 2025 — Whisper Fine-Tune vs Commercial APIs

**Question:** Can fine-tuning Whisper achieve measurable WER reductions, even when comparing local inference against cloud-based commercial models?

**Links:** [Dataset](https://huggingface.co/datasets/danielrosehill/Whisper-Fine-Tune-One-Shot-Eval) · [Space](https://huggingface.co/spaces/danielrosehill/Whisper-Fine-Tune-Eval)

**Summary:** Fine-tuned Whisper Large Turbo running locally achieved 5.84% WER, beating the best commercial API (Assembly AI) tested via Eden AI. Demonstrates that even a quick fine-tune on personal voice data can outperform paid cloud ASR services.

---

### Nov 2025 — Tech Vocabulary ASR Training Data

**Question:** Can a specialized speech dataset improve ASR performance on technical and developer vocabulary?

**Links:** [Dataset](https://huggingface.co/datasets/danielrosehill/Tech-Sentences-For-ASR-Training)

**Summary:** Work-in-progress dataset of 205 human-recorded samples (38 min, 10K words) targeting developer and technical vocabulary for Whisper fine-tuning. Covers software engineering terms, GitHub references, and programming jargon that stock models commonly misrecognize.

---

### Nov 2025 — Voice-to-Vector RAG Pipeline Test

**Question:** Can voice data be reliably transcribed, structured, and upserted into a vector database for accurate retrieval?

**Links:** [Dataset](https://huggingface.co/datasets/danielrosehill/Sample-Voice-Context-Data)

**Summary:** Synthetic dataset simulating a job seeker narrating career trajectory, used to test a voice-to-vector-database RAG pipeline: MP3 → transcription → structured context → Pinecone/Ragie upsert → retrieval accuracy evaluation.

---

### Dec 2025 — Microphone Selection Impact

**Question:** To what extent does microphone selection affect ASR transcription accuracy?

**Links:** [GitHub](https://github.com/danielrosehill/Microphone-Audio-Samples)

**Summary:** Collected test samples across various microphones and evaluated STT accuracy differences. Tests whether hardware choice meaningfully impacts transcription quality for the same speaker and content.

---

### Dec 2025 — WPM & Background Noise Impact

**Question:** To what extent do background noise and variations in speaking pace (WPM) affect ASR transcription accuracy as measured by Word Error Rate (WER)?

**Links:** [GitHub](https://github.com/danielrosehill/Whisper-WPM-Background-Noise-Eval) · [Dataset](https://huggingface.co/datasets/danielrosehill/ASR-WPM-And-Background-Noise-Eval)

**Summary:** Controlled evaluation testing Whisper across multiple variables: speaking pace (fast, normal, slow, whispered, loud), background noise types (cafe, music, conversations, transit, traffic, sirens, dogs, baby sounds), and microphone distance (close, normal, far). Annotated audio recordings with WER measurements for each condition.

---

### Dec 2025 — Transcription Cleanup Evaluation

**Question:** How do various cloud audio understanding models perform on the transcribe-and-cleanup workflow?

**Links:** [GitHub](https://github.com/danielrosehill/Transcription-Cleanup-Eval-1225)

**Summary:** Evaluated multiple cloud-based audio understanding models on their ability to not just transcribe but also clean up and format transcriptions. Compared end-to-end quality of the combined transcription + post-processing pipeline.

---

### Dec 2025 — Fine-Tuned vs Stock Whisper Models

**Question:** How much accuracy improvement can be achieved through fine-tuning Whisper models compared to stock models on local inference?

**Links:** [GitHub (1)](https://github.com/danielrosehill/Fine-Tune-Accuracy-Evaluation) · [GitHub (2)](https://github.com/danielrosehill/Whisper-Fine-Tune-Accuracy-Eval) · [Dataset](https://huggingface.co/datasets/danielrosehill/Small-STT-Eval-Audio-Dataset)

**Summary:** Compared fine-tuned Whisper against stock Whisper on local inference using a 92-sample evaluation dataset covering technical vocabulary, English-Hebrew code-switching, and various speaking styles. Ground truth transcriptions provided for WER measurement.

---

### Mar 2026 — Gemini 3.1 Lite Audio Understanding

**Question:** How well does Gemini 3.1 Lite handle audio understanding tasks beyond simple transcription?

**Links:** [GitHub](https://github.com/danielrosehill/Gemini-31-Lite-Audio-Understanding-Eval) · [Dataset](https://huggingface.co/datasets/danielrosehill/Audio-Understanding-Test-Set) · [Space](https://huggingface.co/spaces/danielrosehill/Audio-Understanding-Experiment)

**Summary:** Tested Gemini 3.1 Flash Lite on 137 prompts across 22 categories paired with a 20-minute voice sample. Categories include speaker analysis, emotion detection, audio engineering, voice cloning, and forensic audio. 49 completed model outputs demonstrate the model's capabilities and limitations across diverse audio understanding tasks.

---

### Mar 2026 — Single-Shot ASR Evaluation

**Links:** [Space](https://huggingface.co/spaces/danielrosehill/Single-Shot-ASR-Eval)

**Summary:** Single-shot evaluation interface for quick ASR benchmarking against individual audio samples.

---

### Apr 2026 — Audio Understanding Bitrate Evaluation

**Question:** How low can MP3 bitrate go before transcription accuracy degrades on audio-input LLMs accessed via OpenRouter?

**Links:** [GitHub](https://github.com/danielrosehill/Audio-Understanding-Bitrate-Eval-0426) · [Dataset](https://huggingface.co/datasets/danielrosehill/Audio-Understanding-Bitrate-Eval-0426)

**Summary:** 12 OpenRouter audio-LLMs (Gemini family, GPT-Audio family, Voxtral, MiMo) × 4 dictation samples × 5 MP3 bitrates (16/24/32/48/64 kbps) = 240 API calls, scored by verbatim-transcription WER with per-call latency captured. Findings: bitrate barely matters above ~16 kbps for Gemini and Voxtral; Gemini 3 Flash Preview leads on accuracy (avg WER 0.014), Voxtral leads on accuracy-per-second (~1.0s latency); OpenAI's GPT-Audio models occasionally respond conversationally to the audio instead of transcribing it, even with an explicit verbatim prompt.

---

## Datasets

| Dataset | Samples | Purpose | Link |
|---------|---------|---------|------|
| ASR-WPM-And-Background-Noise-Eval | — | Controlled audio samples testing pace, noise, and distance variables | [HF](https://huggingface.co/datasets/danielrosehill/ASR-WPM-And-Background-Noise-Eval) |
| English-Hebrew-Mixed-Sentences | 516 | Code-switched English-Hebrew speech evaluation pairs | [HF](https://huggingface.co/datasets/danielrosehill/English-Hebrew-Mixed-Sentences) |
| Audio-Understanding-Test-Set | 137 | Multimodal audio understanding test prompts across 22 categories | [HF](https://huggingface.co/datasets/danielrosehill/Audio-Understanding-Test-Set) |
| Small-STT-Eval-Audio-Dataset | 92 | Technical vocabulary and code-switching STT evaluation | [HF](https://huggingface.co/datasets/danielrosehill/Small-STT-Eval-Audio-Dataset) |
| Sample-Voice-Context-Data | — | Voice-to-vector-database RAG pipeline testing | [HF](https://huggingface.co/datasets/danielrosehill/Sample-Voice-Context-Data) |
| Tech-Sentences-For-ASR-Training | 205 | Technical/developer vocabulary for ASR fine-tuning | [HF](https://huggingface.co/datasets/danielrosehill/Tech-Sentences-For-ASR-Training) |
| Whisper-Fine-Tune-One-Shot-Eval | — | Fine-tuned Whisper vs commercial ASR API comparison | [HF](https://huggingface.co/datasets/danielrosehill/Whisper-Fine-Tune-One-Shot-Eval) |
| Podcast-ASR-Evaluation | — | Podcast transcription ASR evaluation | [HF](https://huggingface.co/datasets/danielrosehill/Podcast-ASR-Evaluation) |
| Audio-Understanding-Bitrate-Eval-0426 | 4 | MP3 bitrate × 12-model audio-LLM sweep; verbatim WER + latency | [HF](https://huggingface.co/datasets/danielrosehill/Audio-Understanding-Bitrate-Eval-0426) |

## Spaces

| Space | Purpose | Link |
|-------|---------|------|
| Single-Shot-ASR-Eval | Quick single-shot ASR benchmarking | [HF](https://huggingface.co/spaces/danielrosehill/Single-Shot-ASR-Eval) |
| Audio-Understanding-Experiment | Audio understanding experiment results | [HF](https://huggingface.co/spaces/danielrosehill/Audio-Understanding-Experiment) |
| Whisper-Fine-Tune-Eval | Whisper fine-tune vs API benchmark results | [HF](https://huggingface.co/spaces/danielrosehill/Whisper-Fine-Tune-Eval) |
| STT-Comparison | Side-by-side STT system comparison | [HF](https://huggingface.co/spaces/danielrosehill/STT-Comparison) |

---

## License

MIT
