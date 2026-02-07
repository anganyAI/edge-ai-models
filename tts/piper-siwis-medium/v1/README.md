---
license: mit
---

# Piper fr_FR-siwis-medium

French female TTS voice from [Piper](https://github.com/rhasspy/piper) (VITS architecture).

## Model Details

- **Voice:** Female, single speaker
- **Training data:** SIWIS French speech corpus
- **Quality:** Medium
- **Sample rate:** 22,050 Hz
- **Size:** ~61 MB

## Files

| File | Description |
|------|-------------|
| `fr_FR-siwis-medium.onnx` | VITS TTS model (ONNX) |
| `fr_FR-siwis-medium.onnx.json` | Model configuration |

Requires shared `espeak-ng-data/` directory for phonemization (located at `tts/espeak-ng-data/`).

## Source

- https://huggingface.co/rhasspy/piper-voices
- https://rhasspy.github.io/piper-samples/ (audio samples)

## License

MIT License
