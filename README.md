# Speech & ASR Evaluations Index

Index of evaluations and experiments conducted to assess Automatic Speech Recognition (ASR) / Speech-to-Text (STT) system performance under various conditions.

**Author:** Daniel Rosehill
**Related Index:** [Experiments-And-Evaluations-Index](https://github.com/danielrosehill/Experiments-And-Evaluations-Index)

---

## Evaluations

### WPM & Background Noise Impact

**Research Question:** To what extent do background noise and variations in speaking pace (WPM) affect ASR transcription accuracy as measured by Word Error Rate (WER)?

**Evaluation Repository:** [Whisper-WPM-Background-Noise-Eval](https://github.com/danielrosehill/Whisper-WPM-Background-Noise-Eval)

**Dataset:** [ASR-WPM-And-Background-Noise-Eval](https://huggingface.co/datasets/danielrosehill/ASR-WPM-And-Background-Noise-Eval)

**Variables Tested:**
- Speaking pace (fast, normal, slow, whispered, loud)
- Background noise types (cafe, music, conversations, transit, traffic, sirens, dogs, baby sounds)
- Microphone distance (close, normal, far)

---

### English-Hebrew Code-Switched Speech

**Research Question:** How well do standard STT systems handle code-switched English-Hebrew speech patterns common among English-speaking immigrants in Israel?

**Dataset:** [English-Hebrew-Mixed-Sentences](https://huggingface.co/datasets/danielrosehill/English-Hebrew-Mixed-Sentences)

**Focus Areas:**
- Transcription accuracy for mixed-language sentences
- Domain-specific vocabulary handling (government, healthcare, documents)
- Performance on naturally interspersed Hebrew words in English speech

---

### Microphone Selection Impact

**Research Question:** To what extent does microphone selection affect ASR transcription accuracy?

**Evaluation Repository:** [Microphone-Audio-Samples](https://github.com/danielrosehill/Microphone-Audio-Samples)

---

### Local Whisper Model Comparison

**Research Question:** What is the difference in accuracy between various Whisper models on local inference, and how do derivative engines compare against original Whisper?

**Evaluation Repository:** [Local-ASR-STT-Benchmark](https://github.com/danielrosehill/Local-ASR-STT-Benchmark)

**Notes:** Evaluation conducted on AMD GPU hardware (ROCm)

---

### Fine-Tuned vs Stock Whisper Models

**Research Question:** How much accuracy improvement can be achieved through fine-tuning Whisper models compared to stock models on local inference?

**Evaluation Repositories:**
- [Fine-Tune-Accuracy-Evaluation](https://github.com/danielrosehill/Fine-Tune-Accuracy-Evaluation)
- [Whisper-Fine-Tune-Accuracy-Eval](https://github.com/danielrosehill/Whisper-Fine-Tune-Accuracy-Eval)

---

### Long-Form Audio Transcription

**Research Question:** How do ASR systems perform on extended audio recordings compared to shorter clips?

**Evaluation Repository:** [Long-Form-Audio-Eval](https://github.com/danielrosehill/Long-Form-Audio-Eval)

---

### Personal STT Benchmarking

**Research Question:** General benchmarking of STT systems for personal use cases.

**Evaluation Repository:** [Personal-STT-Benchmarking](https://github.com/danielrosehill/Personal-STT-Benchmarking)

---

### Transcription Cleanup Evaluation

**Research Question:** Evaluating transcription cleanup and post-processing methods.

**Evaluation Repository:** [Transcription-Cleanup-Eval-1225](https://github.com/danielrosehill/Transcription-Cleanup-Eval-1225)

---

## Datasets

| Dataset | Purpose | Link |
|---------|---------|------|
| ASR-WPM-And-Background-Noise-Eval | Controlled audio samples for testing pace, noise, and distance variables | [Hugging Face](https://huggingface.co/datasets/danielrosehill/ASR-WPM-And-Background-Noise-Eval) |
| English-Hebrew-Mixed-Sentences | 516 audio-text pairs for code-switched English-Hebrew speech evaluation | [Hugging Face](https://huggingface.co/datasets/danielrosehill/English-Hebrew-Mixed-Sentences) |

---

## License

MIT
