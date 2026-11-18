# ko-notes-models

Model archives that Ko Notes downloads when a person chooses a local model in its Settings. This repository holds
no code: the files are attached to its releases, and the app fetches them from here when its first address
(`models.koona.app`) does not answer.

Each model is one ustar archive, cut into parts of at most 1 GiB (`<model>-v1.tar.part-01`, `-02`, …). Inside it
every file is compressed on its own with Brotli (`<path>.br`), next to a `LICENSE` and a `NOTICE` that names where
the files come from. The files are the ones published on Hugging Face at the revision named, byte for byte;
nothing was retrained or changed. The app pins every part, every file and its SHA-256, so it accepts only these bytes.

Each model is licensed by its makers under its own license (below, and in `LICENSE` inside its archive). Anyone
who downloads or uses a model receives it under that license. We do not make these models and claim no rights in them.

## Qwen3.5 0.8B Base (4-bit MLX) (release `qwen3.5-0.8b-base-4bit-v1`)

- Made by: Qwen Team, Alibaba Cloud; license: **Apache License 2.0**
- From: https://huggingface.co/luokelabs/Qwen3.5-0.8B-Base-4bit at revision `76ddcd734a7263fae2f7382fbe718adb16bd5f59`
- `qwen3.5-0.8b-base-4bit-v1.tar`: 379,390,976 bytes in 1 part(s) (444,092,749 bytes of files), SHA-256 `2b43f4eee407509705b4720313a7ca0f6b5d09d31091519895d29112107a4b58`

## Parakeet Ultra 0.6B (Core ML) (release `parakeet-ultra-0.6b-v1`)

- Made by: Moondream, NVIDIA; license: **Creative Commons Attribution 4.0**
- From: https://huggingface.co/FluidInference/parakeet-ultra-coreml at revision `95eaa59a39d4394f047a4dc5cce480388a60d1b6`
- `parakeet-ultra-0.6b-v1.tar`: 548,309,504 bytes in 1 part(s) (632,182,363 bytes of files), SHA-256 `74ebf67b37bb721de38abeaa9b8ef0c9d64665f126b3b35e18615c84e4d7a2f1`

## Nemotron 3.5 ASR Streaming 0.6B (Core ML) (release `nemotron-3.5-asr-streaming-0.6b-v1`)

- Made by: NVIDIA; license: **OpenMDW License 1.1**
- From: https://huggingface.co/FluidInference/Nemotron-3.5-ASR-Streaming-Multilingual-0.6b-CoreML at revision `1a41b75758b0337ff67db7d5408280aaaf23074e`
- `nemotron-3.5-asr-streaming-0.6b-v1.tar`: 559,374,336 bytes in 1 part(s) (614,736,032 bytes of files), SHA-256 `aa3924a8535ef6c7e743165ac56156275124e145048cfe01086c6645ee15a70f`

## Whisper Large v3 Turbo (Core ML, WhisperKit) (release `whisperkit-large-v3-turbo-v1`)

- Made by: OpenAI; license: **MIT License**
- From: https://huggingface.co/argmaxinc/whisperkit-coreml at revision `0f63a7800b00dd0226abd051b906c246e1907482`
- `whisperkit-large-v3-turbo-v1.tar`: 447,763,456 bytes in 1 part(s) (645,670,456 bytes of files), SHA-256 `57e4f795740ef37011b70e3ce4a908adec3a05624d80fd9a87dc50ddd949b540`

## Qwen3.5 2B (4-bit MLX) (release `qwen3.5-2b-4bit-v1`)

- Made by: Qwen Team, Alibaba Cloud; license: **Apache License 2.0**
- From: https://huggingface.co/mlx-community/Qwen3.5-2B-4bit at revision `674aaa7240b91e8012fcad5d791b7dfe5ba90207`
- `qwen3.5-2b-4bit-v1.tar`: 1,416,666,624 bytes in 2 part(s) (1,742,366,945 bytes of files), SHA-256 `5c3efcd24f50238f635187cf0857909fd6defebc18193d211b900144811e51f9`

## Qwen3.5 4B (4-bit MLX) (release `qwen3.5-4b-4bit-v1`)

- Made by: Qwen Team, Alibaba Cloud; license: **Apache License 2.0**
- From: https://huggingface.co/mlx-community/Qwen3.5-4B-4bit at revision `0e7ffd5c629ef7719d4cbc04069232580bfa9d9c`
- `qwen3.5-4b-4bit-v1.tar`: 2,588,614,656 bytes in 3 part(s) (3,054,416,331 bytes of files), SHA-256 `3df1624ba498a9f2b8a964ebffcc5d752ca3158e7e60264df52904d384a2b123`

## LFM2.5 1.2B Instruct (4-bit MLX) (release `lfm2.5-1.2b-instruct-4bit-v1`)

- Made by: Liquid AI, Inc.; license: **LFM Open License v1.0**
- From: https://huggingface.co/LiquidAI/LFM2.5-1.2B-Instruct-MLX-4bit at revision `7ccafdb04c36936f4f1c4685198c6c9a40275932`
- `lfm2.5-1.2b-instruct-4bit-v1.tar`: 584,157,184 bytes in 1 part(s) (663,404,634 bytes of files), SHA-256 `a0170b959beb448e136f78ccd4543d8054accdccc432edfbfb290d0a2f2df09b`

  Its license does not cover commercial use by an entity with annual revenue of US$10 million or more (section 5).

## Ministral 3 3B Instruct 2512 (4-bit MLX) (release `ministral-3-3b-instruct-2512-4bit-v1`)

- Made by: Mistral AI; license: **Apache License 2.0**
- From: https://huggingface.co/mlx-community/Ministral-3-3B-Instruct-2512-4bit at revision `a962dcb09eee4169c890e544c9eb938f1113fdee`
- `ministral-3-3b-instruct-2512-4bit-v1.tar`: 2,267,359,232 bytes in 3 part(s) (2,762,406,185 bytes of files), SHA-256 `1d5e473d6f099fcd027afcc02623e7b258aceb1f95ba4a3b4da692d1aee15b76`

## Gemma 4 E2B-it (4-bit MLX) (release `gemma-4-e2b-it-4bit-v1`)

- Made by: Google DeepMind; license: **Apache License 2.0**
- From: https://huggingface.co/mlx-community/gemma-4-e2b-it-4bit at revision `238767527555cb75a05732a84dff5d6ba0dd6809`
- `gemma-4-e2b-it-4bit-v1.tar`: 2,614,462,464 bytes in 3 part(s) (3,583,097,322 bytes of files), SHA-256 `67b8fb95db5cf8c8a8fdc8f2d0be4e4de2d251b803f9484fd75fe47dc6365fea`
