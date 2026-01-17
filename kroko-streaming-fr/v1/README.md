# Kroko Streaming ASR - French

French streaming speech-to-text model based on Zipformer2 architecture.

## Source

- **Original**: [Banafo/Kroko-ASR](https://huggingface.co/Banafo/Kroko-ASR)
- **Quantized version**: [hudaiapa88/sherpa-stt-onnx](https://huggingface.co/hudaiapa88/sherpa-stt-onnx/tree/main/fr/kroko_64l)

## Model Details

- **Architecture**: Zipformer2 Transducer
- **Language**: French (fr)
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
| tokens.txt | 6.7 KB | Token vocabulary |

## License

- Community models: CC-BY-SA
- Engine (sherpa-onnx): Apache-2.0
