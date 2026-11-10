# VidPass speech model

This is the speech model VidPass downloads to make transcripts on your computer: NVIDIA's
[Parakeet TDT 0.6B v2](https://huggingface.co/nvidia/parakeet-tdt-0.6b-v2), in the int8 ONNX
version made by the [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) project.

The files are unchanged copies of sherpa-onnx's August 2025 export, kept here so that the download
never changes. (sherpa-onnx replaces its own download whenever it runs the export again.)

## The download

[`parakeet-tdt-0.6b-v2-int8.tar.bz2`](https://github.com/LocalJon/vidpass-speech-model/releases/download/parakeet-v2-int8-2025-08/parakeet-tdt-0.6b-v2-int8.tar.bz2),
482,520,984 bytes, SHA-256 `8b7461a35673b591fb46029bcf835a9765a5e689cdb714ef77b57be7183053e8`.

It holds these files, plus a `README.txt` with the credits below:

| File | Bytes | SHA-256 |
| --- | ---: | --- |
| `encoder.int8.onnx` | 652,184,296 | `a32b12d17bbbc309d0686fbbcc2987b5e9b8333a7da83fa6b089f0a2acd651ab` |
| `decoder.int8.onnx` | 7,257,753 | `b6bb64963457237b900e496ee9994b59294526439fbcc1fecf705b31a15c6b4e` |
| `joiner.int8.onnx` | 1,739,080 | `7946164367946e7f9f29a122407c3252b680dbae9a51343eb2488d057c3c43d2` |
| `tokens.txt` | 9,384 | `ec182b70dd42113aff6c5372c75cac58c952443eb22322f57bbd7f53977d497d` |
| `test_wavs/0.wav` | 237,964 | `5fceacff0315d49cb59fcc505bcecf1ed5f2f35c2897b1e65a59f30e5d922150` |

Each file is identical to the one in
[csukuangfj/sherpa-onnx-nemo-parakeet-tdt-0.6b-v2-int8](https://huggingface.co/csukuangfj/sherpa-onnx-nemo-parakeet-tdt-0.6b-v2-int8/tree/1ab9323565ddb038682214b292f588070a538ce2)
on Hugging Face at commit `1ab9323565ddb038682214b292f588070a538ce2`, where sherpa-onnx publishes its
exports. To check one, download it from there by that commit and compare the SHA-256.

The archive is made by [`.github/workflows/publish.yml`](.github/workflows/publish.yml), run by hand:
it downloads each file from Hugging Face by that commit, checks it against
[`files.sha256`](files.sha256), packs the files with [`archive/README.txt`](archive/README.txt) and
publishes the result. It never replaces a release that exists.

## Credits and license

The model weights are NVIDIA's, licensed under the
[Creative Commons Attribution 4.0 International license (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
The ONNX export is by the sherpa-onnx project, whose code is licensed under the Apache License 2.0.
Nothing here was changed. NVIDIA and sherpa-onnx don't endorse VidPass or this copy.
