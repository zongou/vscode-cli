# VS Code Cli

Setting up runtime environment with PRoot and run vscode server

使用 PRoot 配置运行环境并运行 vscode 网页版

## Server

Run a web version of vscode

运行 vscode 网页版

```sh
./vscli serve-web \
  --host=0.0.0.0 \
  --port=8000 \
  --without-connection-token \
  --log=trace \
  "$@"
```

## Patch

To work better on Android

为了更好的在 Android 上使用而打补丁

```sh
./vscli patch
```

## Revert

Revert patch

回退补丁

```sh
./vscli revert
```
