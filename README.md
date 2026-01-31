# PyTorch Windows ARM64 Wheels

Unofficial, native PyTorch wheels for Windows 11 on ARM64 (Snapdragon X Elite/Plus devices), built with QNNPACK and XNNPACK support.

## 🚀 Features
- **Native ARM64 Support**: No emulation, runs natively on Windows on Arm.
- **QNNPACK/XNNPACK Enabled**: Optimized for mobile and edge CPUs.
- **Python Support**: Builds for Python 3.11, 3.12, and 3.13.
- **No CUDA**: CPU-only build (NPU support via QNN delegation is separate).
- **Modern Toolchain**: Built with MSVC 2022.

## 📦 Installation

Go to the [Releases](https://github.com/Snapdragon-AI-Stack/pytorch-arm64-wheels/releases) page and download the `.whl` file matching your Python version.

```bash
# Example for Python 3.12
pip install torch-2.11.0a0+git...-cp312-cp312-win_arm64.whl
```

## 🛠️ Building from Source

This repository uses GitHub Actions to build the wheels.

### Triggering a Build
1. Go to the [Actions](https://github.com/Snapdragon-AI-Stack/pytorch-arm64-wheels/actions) tab.
2. Select **Build PyTorch Windows ARM64 Wheels**.
3. Click **Run workflow**.
4. (Optional) Check **Publish Release?** to automatically create a GitHub Release upon success.

### Local Build Prerequisites
- Visual Studio 2022 with C++ Desktop Development (ARM64 tools)
- Python 3.11+
- git with `core.longpaths` enabled
- `sccache` (recommended for faster rebuilds)

## 🤝 Contributing
Issues and pull requests are welcome!

## 📜 License
This project follows the PyTorch [License](https://github.com/pytorch/pytorch/blob/main/LICENSE).
