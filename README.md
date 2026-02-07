# Edge AI Models

Pre-extracted AI models for the SttTestApp React Native application.

## Models

| Model | Version | Size | Description |
|-------|---------|------|-------------|
| **parakeet-offline** | v1 | ~640MB | NVIDIA Parakeet TDT offline STT model (int8, transducer) |
| **whisper-small** | v1 | ~357MB | OpenAI Whisper Small multilingual STT model (int8, encoder-decoder) |
| **zipformer-streaming** | v1 | ~405MB | Zipformer streaming STT model (French) |
| **kroko-streaming-fr** | v1 | ~154MB | Kroko French streaming STT model (int8) |
| **speaker** | v1 | ~38MB | 3D-Speaker embedding model for diarization |
| **denoiser** | v1 | ~524KB | GTCRN audio denoiser |
| **pyannote-segmentation** | v1 | ~1.5MB | Pyannote 3.0 multi-speaker segmentation (int8) |
| **vad/silero** | v1 | ~2.2MB | Silero VAD v6 voice activity detection (8/16 kHz) |
| **vad/ten** | v1 | ~324KB | TEN VAD real-time voice activity detection (int8 + full) |

## Directory Structure

```
stt-models/
├── parakeet-offline/
│   └── v1/
│       ├── encoder.int8.onnx
│       ├── decoder.int8.onnx
│       ├── joiner.int8.onnx      # Transducer architecture
│       └── tokens.txt
├── whisper-small/
│   └── v1/
│       ├── encoder.int8.onnx
│       ├── decoder.int8.onnx      # Encoder-decoder architecture (no joiner)
│       └── tokens.txt
├── zipformer-streaming/
│   └── v1/
│       ├── encoder-epoch-29-avg-9-with-averaged-model.int8.onnx
│       ├── decoder-epoch-29-avg-9-with-averaged-model.int8.onnx
│       ├── joiner-epoch-29-avg-9-with-averaged-model.int8.onnx
│       ├── tokens.txt
│       └── README.md
├── kroko-streaming-fr/
│   └── v1/
│       ├── encoder.int8.onnx
│       ├── decoder.int8.onnx
│       ├── joiner.int8.onnx
│       ├── tokens.txt
│       └── README.md
├── speaker/
│   └── v1/
│       └── 3dspeaker_speech_eres2net_base_sv_zh-cn_3dspeaker_16k.onnx
├── denoiser/
│   └── v1/
│       └── gtcrn_simple.onnx
├── pyannote-segmentation/
│   └── v1/
│       └── model.int8.onnx
└── vad/
    ├── silero/
    │   └── v1/
    │       ├── silero_vad.onnx
    │       └── README.md
    └── ten/
        └── v1/
            ├── ten-vad.onnx
            ├── ten-vad.int8.onnx
            └── README.md
```

## Source

Models sourced from [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx/releases).

## Usage

These models are downloaded by the SttTestApp Model Manager to enable offline speech-to-text functionality.
