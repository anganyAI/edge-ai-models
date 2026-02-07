---
license: mit
---

# Piper fr_FR-mls-medium

French multi-speaker TTS voice from [Piper](https://github.com/rhasspy/piper) (VITS architecture).

## Model Details

- **Voice:** Multi-speaker
- **Training data:** Multilingual LibriSpeech (MLS)
- **Quality:** Medium
- **Sample rate:** 22,050 Hz
- **Size:** ~74 MB

## Files

| File | Description |
|------|-------------|
| `fr_FR-mls-medium.onnx` | VITS TTS model (ONNX) |
| `fr_FR-mls-medium.onnx.json` | Model configuration (includes speaker map) |

Requires shared `espeak-ng-data/` directory for phonemization (located at `tts/espeak-ng-data/`).

## Source

- https://huggingface.co/rhasspy/piper-voices
- https://rhasspy.github.io/piper-samples/ (audio samples)

## License

MIT License
