---
license: apache-2.0
---

# TEN VAD

Real-time, lightweight Voice Activity Detection model from [TEN-framework/ten-vad](https://github.com/TEN-framework/ten-vad) by Agora.

## Model Details

- **Sample rate:** 16 kHz only
- **ONNX Runtime:** >= 1.17.1 required
- **Low latency:** Optimized for real-time speech-to-non-speech transitions

## Files

| File | Size | Description |
|------|------|-------------|
| `ten-vad.onnx` | 324 KB | Full precision VAD model |
| `ten-vad.int8.onnx` | 126 KB | INT8 quantized VAD model |

**Note:** These are the k2-fsa/sherpa-onnx hosted versions which include required metadata for sherpa-onnx integration.

## Source

- https://github.com/TEN-framework/ten-vad
- https://github.com/k2-fsa/sherpa-onnx/releases (model files)

## License

Apache License 2.0 with additional conditions - Copyright (c) 2025 Agora.
See the [full license](https://github.com/TEN-framework/ten-vad/blob/main/LICENSE) for details.
