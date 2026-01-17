# Edge AI Models

Pre-extracted AI models for the SttTestApp React Native application.

## Models

| Model | Version | Size | Description |
|-------|---------|------|-------------|
| **parakeet-offline** | v1 | ~640MB | NVIDIA Parakeet TDT offline STT model (int8) |
| **zipformer-streaming** | v1 | ~405MB | Zipformer streaming STT model (French) |
| **speaker** | v1 | ~38MB | 3D-Speaker embedding model for diarization |
| **denoiser** | v1 | ~524KB | GTCRN audio denoiser |

## Directory Structure

```
stt-models/
├── parakeet-offline/
│   └── v1/
│       ├── encoder.int8.onnx
│       ├── decoder.int8.onnx
│       ├── joiner.int8.onnx
│       └── tokens.txt
├── zipformer-streaming/
│   └── v1/
│       ├── encoder-epoch-29-avg-9-with-averaged-model.int8.onnx
│       ├── decoder-epoch-29-avg-9-with-averaged-model.int8.onnx
│       ├── joiner-epoch-29-avg-9-with-averaged-model.int8.onnx
│       ├── tokens.txt
│       └── README.md
├── speaker/
│   └── v1/
│       └── 3dspeaker_speech_eres2net_base_sv_zh-cn_3dspeaker_16k.onnx
└── denoiser/
    └── v1/
        └── gtcrn_simple.onnx
```

## Source

Models sourced from [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx/releases).

## Usage

These models are downloaded by the SttTestApp Model Manager to enable offline speech-to-text functionality.
