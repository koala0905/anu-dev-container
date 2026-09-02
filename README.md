# ANU Dev Container

基於 [mcr.microsoft.com/devcontainers/typescript-node:5-24-trixie](https://github.com/devcontainers/images/tree/main/src/typescript-node) 的開發容器 image, 預先安裝 [opencode-ai](https://github.com/anomalyco/opencode)。

## 使用

```bash
docker pull ghcr.io/koala0905/anu-dev-container:latest

docker run -it --rm ghcr.io/koala0905/anu-dev-container:latest
```

或是直接以開發容器（Dev Container）方式使用：

```json
{
  "image": "ghcr.io/koala0905/anu-dev-container:latest"
}
```

## 手動 build

```bash
docker build -t ghcr.io/koala0905/anu-dev-container:latest .
```

## 自動發布

Push 到 `main` 分支時, 會透過 GitHub Actions 自動 build 並發布到 GitHub Container Registry (GHCR)。