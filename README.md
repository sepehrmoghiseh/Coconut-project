# Coconut Project – AI Music Generation (Audiocraft/MusicGen)

Generate short music clips guided by **mood** or **text prompts** (e.g., *happy*, *sad*, *calm*, *energetic*) using Facebook’s **Audiocraft / MusicGen**.  
Includes basic **NLP mood parsing**, **audio feature analysis** (tempo & spectral features), and **post-processing** (fades, trimming) for cleaner output.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://github.com/sepehrmoghiseh/Coconut-project/blob/master/Coconut_project_Final.ipynb)

---

## 🚀 Features
- Prompt → **MusicGen** generation (Facebook Audiocraft)
- Optional **mood/text classification** via TextBlob
- **Audio post-processing** with pydub (trim, fade in/out, normalization)
- **Feature extraction**: tempo, spectral centroid/bandwidth (for quick QA)
- All-in-one **Colab notebook** (GPU ready)

---

## 📂 Repo Structure

---

## 🧰 Requirements
> Colab already has most deps; the notebook installs the rest automatically.

- Python 3.9+
- GPU recommended (T4 or better on Colab)
- Libraries:
  - `audiocraft` (MusicGen)
  - `torch`, `torchaudio`
  - `pydub`
  - `pretty_midi`
  - `textblob`
  - `numpy`

Install locally (optional):
```bash
pip install torch torchaudio --index-url https://download.pytorch.org/whl/cu121
pip install "audiocraft>=1.0.0" pydub pretty_midi textblob numpy
