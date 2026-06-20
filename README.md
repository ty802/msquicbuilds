# msquic builds

Builds [microsoft/msquic](https://github.com/microsoft/msquic) via GitHub Actions for:

| Platform    | Architectures      | TLS       |
|-------------|--------------------|-----------|
| Windows     | amd64, arm64       | schannel  |
| Linux       | amd64, arm64       | quictls   |
| macOS       | amd64, arm64       | quictls   |
| Android     | arm64              | quictls   |

NuGet packages (`Microsoft.Native.Quic.MsQuic.Schannel`) are produced for Windows (x64 + arm64).

## Artifacts

Each run produces per-platform archives plus `nuget-windows-schannel/*.nupkg`.
