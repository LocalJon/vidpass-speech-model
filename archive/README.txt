NVIDIA's Parakeet TDT 0.6B v2 speech model, in the int8 ONNX version made by
the sherpa-onnx project. The files are unchanged copies of sherpa-onnx's
August 2025 export (sherpa-onnx-nemo-parakeet-tdt-0.6b-v2-int8, Hugging Face
commit 1ab9323565ddb038682214b292f588070a538ce2), kept here so that the
download never changes.

The weights are NVIDIA's, licensed under the Creative Commons Attribution 4.0
International license (CC BY 4.0, https://creativecommons.org/licenses/by/4.0/):
https://huggingface.co/nvidia/parakeet-tdt-0.6b-v2
The ONNX export is by the sherpa-onnx project (https://github.com/k2-fsa/sherpa-onnx,
Apache License 2.0). NVIDIA and sherpa-onnx don't endorse this copy.

SHA-256 of each file:
a32b12d17bbbc309d0686fbbcc2987b5e9b8333a7da83fa6b089f0a2acd651ab  encoder.int8.onnx
b6bb64963457237b900e496ee9994b59294526439fbcc1fecf705b31a15c6b4e  decoder.int8.onnx
7946164367946e7f9f29a122407c3252b680dbae9a51343eb2488d057c3c43d2  joiner.int8.onnx
ec182b70dd42113aff6c5372c75cac58c952443eb22322f57bbd7f53977d497d  tokens.txt
5fceacff0315d49cb59fcc505bcecf1ed5f2f35c2897b1e65a59f30e5d922150  test_wavs/0.wav
