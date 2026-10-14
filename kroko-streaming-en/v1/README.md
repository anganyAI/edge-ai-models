# Kroko Streaming ASR - English

English streaming speech-to-text model based on Zipformer2 architecture.

## Source

- **Original**: [Banafo/Kroko-ASR](https://huggingface.co/Banafo/Kroko-ASR)
- **Quantized version**: [hudaiapa88/sherpa-stt-onnx](https://huggingface.co/hudaiapa88/sherpa-stt-onnx/tree/main/en/kroko_64l)
  at revision `fe61e648310e068a5558c3d4e4d02c25742820a4`, the same source and variant as
  `kroko-streaming-fr`

## Model Details

- **Architecture**: Zipformer2 Transducer
- **Language**: English (en)
- **Variant**: 64L (64 layers)
- **Quantization**: INT8
- **Sample Rate**: 16000 Hz
- **Total Size**: ~154 MB

## Files

| File | Size | Description |
|------|------|-------------|
| encoder.int8.onnx | 146 MB | Encoder model (INT8 quantized) |
| decoder.int8.onnx | 592 KB | Decoder model (INT8 quantized) |
| joiner.int8.onnx | 329 KB | Joiner model (INT8 quantized) |
| tokens.txt | 6.6 KB | Token vocabulary |

SHA-256 of the files as published at that revision:

- encoder.int8.onnx `e00580c44a08638b…` (see the LFS pointer for the full digest)
- decoder.int8.onnx `e006d1a4d779ea3f…`
- joiner.int8.onnx `9297a98e7716bbfa…`

## License

- Community models: CC-BY-SA
- Engine (sherpa-onnx): Apache-2.0
