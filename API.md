# code api

| platform            |
| ------------------- |
| cli-alpine-arm64    |
| cli-alpine-x64      |
| cli-darwin-arm64    |
| cli-darwin-x64      |
| cli-linux-arm64     |
| cli-linux-armhf     |
| cli-linux-x64       |
| cli-win32-arm64     |
| cli-win32-x64       |
| darwin              |
| darwin-arm64        |
| darwin-universal    |
| linux-arm64         |
| linux-armhf         |
| linux-deb-arm64     |
| linux-deb-armhf     |
| linux-deb-x64       |
| linux-rpm-arm64     |
| linux-rpm-armhf     |
| linux-rpm-x64       |
| linux-snap-x64      |
| linux-x64           |
| win32-arm64         |
| win32-arm64-archive |
| win32-arm64-user    |
| win32-x64           |
| win32-x64-archive   |
| win32-x64-user      |

---

```sh
QUALITY=stable
VSCODE_ARCH=arm64
platform=cli-alpine-${VSCODE_ARCH}
URL=https://update.code.visualstudio.com/api/latest/cli-alpine-${VSCODE_ARCH}/${QUALITY}
URL=https://update.code.visualstudio.com/1.96.4/api/cli-alpine-${VSCODE_ARCH}/${QUALITY}

# version_id=e54c774e0add60467559eb0d1e229c6452cf8447
# URL=https://update.code.visualstudio.com/${version_id}/${platform}/insider

curl -Ss "${URL}"
```

## Get all version

```sh
curl -Ss https://update.code.visualstudio.com/api/releases/stable
```

```sh
curl -Ss https://update.code.visualstudio.com/api/releases/insider
```

## Get all commits

```sh
# curl -Ss https://update.code.visualstudio.com/api/commits/stable/server-linux-arm64-web
# curl -Ss https://update.code.visualstudio.com/api/commits/stable/server-linux-x64-web
curl -Ss https://update.code.visualstudio.com/api/commits/insider/server-linux-arm64-web
```

## Get download link

```sh
curl -Ss https://update.code.visualstudio.com/api/versions/1.96.4/cli-alpine-x64/stable
```

```sh
curl -Ss https://update.code.visualstudio.com/api/update/win32-x64/stable/26076a4de974ead31f97692a0d32f90d735645c0
```

```sh
curl -sL https://update.code.visualstudio.com/api/update/web-standalone/stable/latest
```

## Redirect to version download link

```sh
curl -Ss https://update.code.visualstudio.com/1.96.4/cli-alpine-arm64/stable
```

```sh
curl https://update.code.visualstudio.com/commit:cd4ee3b1c348a13bafd8f9ad8060705f6d4b9cba/server-linux-x64/stable
```

---

```sh
# curl -LkO https://vscode.download.prss.microsoft.com/dbazure/download/stable/latest/vscode-web.tar.gz
# curl -Ss https://update.code.visualstudio.com/1.96.4/vscode-web/stable
# curl -Ss https://update.code.visualstudio.com/api/commits/stable/server-linux-arm64-web
# curl -Ss https://update.code.visualstudio.com/api/commits/stable/latest
# curl -Ss https://update.code.visualstudio.com/api/releases/stable
```
