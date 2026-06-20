# msquic builds

Builds [microsoft/msquic](https://github.com/microsoft/msquic) via GitHub Actions for:

| Platform    | Architectures      | TLS                   |
|-------------|--------------------|-----------------------|
| Windows     | amd64, arm64       | schannel (modern Win) |
| Windows     | amd64              | quictls (older Win)   |
| Linux       | amd64, arm64       | quictls               |
| macOS       | amd64, arm64       | quictls               |
| Android     | arm64              | quictls               |

NuGet packages produced:
- `Microsoft.Native.Quic.MsQuic.Schannel` – Windows x64 + arm64
- `Microsoft.Native.Quic.MsQuic.QuicTls` – Windows x64 (older Windows)
- `Microsoft.Native.Quic.MsQuic.Linux` – Linux x64 + arm64

## Artifacts

Each run produces per-platform archives plus `nuget-windows-schannel/*.nupkg`.
