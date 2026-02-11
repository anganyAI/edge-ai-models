# NVIDIA Parakeet TDT 0.6B v3 - Multilingual ASR

Multilingual offline speech-to-text model based on FastConformer-TDT architecture.

## Source

- **Original**: [nvidia/parakeet-tdt-0.6b-v3](https://huggingface.co/nvidia/parakeet-tdt-0.6b-v3)
- **ONNX version**: [sherpa-onnx-nemo-parakeet-tdt-0.6b-v3-int8](https://github.com/k2-fsa/sherpa-onnx/releases/tag/asr-models)

## Model Details

- **Architecture**: FastConformer-TDT (Transducer with Duration Tracking)
- **Parameters**: 600M (0.6B)
- **Languages**: 25 European languages (bg, hr, cs, da, nl, en, et, fi, fr, de, el, hu, it, lv, lt, mt, pl, pt, ro, sk, sl, es, sv, ru, uk)
- **Quantization**: INT8
- **Sample Rate**: 16000 Hz (auto-resamples other rates)
- **Tokenizer**: SentencePiece (8,192 tokens)
- **Total Size**: ~640 MB
- **Features**: Automatic language detection, punctuation & capitalization, word/segment timestamps

## Files

| File | Size | Description |
|------|------|-------------|
| encoder.int8.onnx | 622 MB | FastConformer encoder (INT8 quantized) |
| decoder.int8.onnx | 12 MB | TDT decoder (INT8 quantized) |
| joiner.int8.onnx | 6.1 MB | Joiner model (INT8 quantized) |
| tokens.txt | 92 KB | SentencePiece vocabulary (8,192 tokens + special tokens) |

## License

- Model: CC-BY-4.0
- Engine (sherpa-onnx): Apache-2.0
