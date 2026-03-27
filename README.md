# ort-prebuilt

Pre-built ONNX Runtime libraries for [solar2d-plugin-onnxruntime](https://github.com/labolado/solar2d-plugin-onnxruntime).

## Why

ONNX Runtime dropped x86 (32-bit) Windows builds after v1.16.3. Solar2D Windows Simulator requires x86 DLLs. This repo builds ORT from source for platforms that lack official pre-built binaries.

## Usage

Download from [Releases](https://github.com/labolado/ort-prebuilt/releases):

```
onnxruntime-win-x86-{version}.zip
├── lib/
│   ├── onnxruntime.dll
│   └── onnxruntime.lib
└── include/
    └── onnxruntime_c_api.h
```

## Build

Trigger via GitHub Actions → `Build ORT x86` → enter version (e.g. `1.20.1`).

Builds run on `windows-latest` using MSVC x86. Takes ~30-60 minutes.
