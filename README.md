
# Setup
1. 安装 ffmpeg
```bash
# on Ubuntu or Debian
sudo apt update && sudo apt install ffmpeg

# on Arch Linux
sudo pacman -S ffmpeg

# on MacOS using Homebrew (https://brew.sh/)
brew install ffmpeg

# on Windows using Chocolatey (https://chocolatey.org/)
choco install ffmpeg

# on Windows using Scoop (https://scoop.sh/)
scoop install ffmpeg
```

2. 安装 Poetry
```bash
curl -sSL https://install.python-poetry.org | python3 -
```

3. 安装依赖
```bash
poetry install
```



# Usage
1. HuggingFace 创建 Token 并赋予权限
2. nyrahealth/CrisperWhisper 获取模型许可
3. 登录 HuggingFace
```bash
huggingface-cli login
```
4. 下载模型
```bash
huggingface-cli download --resume-download nyrahealth/CrisperWhisper --local-dir ./models/CrisperWhisper --local-dir-use-symlinks False --token hf_xxx

huggingface-cli download --resume-download openai/whisper-large-v3-turbo --local-dir
 ./models/whisper-large-v3-turbo --local-dir-use-symlinks False
 ```
 