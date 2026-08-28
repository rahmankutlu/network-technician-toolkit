# Third-party notices

Network Technician Toolkit (NTT) 1.0.0 · © 2026 Abdurrahman KUTLU · https://rahmankutlu.com

NTT ships as a self-contained build, so the packages below are redistributed inside
`NTT-Setup-1.0.0-win-x64.exe` and `NTT-Portable-1.0.0-win-x64.zip`. Each license below was
read from the package's own `.nuspec` metadata rather than assumed.

## Redistributed packages

| Package | Version | License | Project |
|---|---|---|---|
| CommunityToolkit.Mvvm | 8.2.2 | MIT | https://github.com/CommunityToolkit/dotnet |
| Dapper | 2.1.35 | Apache-2.0 | https://github.com/DapperLib/Dapper |
| Microsoft.Data.Sqlite | 8.0.11 | MIT | https://learn.microsoft.com/dotnet/standard/data/sqlite/ |
| Microsoft.Data.Sqlite.Core | 8.0.11 | MIT | https://learn.microsoft.com/dotnet/standard/data/sqlite/ |
| Microsoft.Extensions.DependencyInjection | 8.0.0 | MIT | https://dot.net/ |
| Microsoft.Extensions.DependencyInjection.Abstractions | 8.0.0 | MIT | https://dot.net/ |
| **PacketDotNet** | 1.4.7 | **MPL-2.0** | https://github.com/dotpcap/packetnet |
| Serilog | 4.0.0 | Apache-2.0 | https://github.com/serilog/serilog |
| Serilog.Sinks.File | 6.0.0 | Apache-2.0 | https://github.com/serilog/serilog-sinks-file |
| SQLitePCLRaw.bundle_e_sqlite3 | 3.0.2 | Apache-2.0 | https://github.com/ericsink/SQLitePCL.raw |
| SQLitePCLRaw.core | 3.0.2 | Apache-2.0 | https://github.com/ericsink/SQLitePCL.raw |
| SQLitePCLRaw.lib.e_sqlite3 | 3.0.2 | Apache-2.0 | https://github.com/ericsink/SQLitePCL.raw |
| SQLitePCLRaw.provider.e_sqlite3 | 3.0.2 | Apache-2.0 | https://github.com/ericsink/SQLitePCL.raw |
| System.CodeDom | 8.0.0 | MIT | https://dot.net/ |
| System.Management | 8.0.0 | MIT | https://dot.net/ |
| System.Memory | 4.5.5 | MIT (.NET Library License) | https://github.com/dotnet/runtime |
| System.Runtime.CompilerServices.Unsafe | 6.0.0 | MIT | https://github.com/dotnet/runtime |
| System.Text.Encoding.CodePages | 6.0.0 | MIT | https://github.com/dotnet/runtime |

The .NET 8 runtime and WPF are redistributed as part of the self-contained publish, under the
MIT license (https://github.com/dotnet/runtime/blob/main/LICENSE.TXT).

SQLite itself, reached through SQLitePCLRaw, is in the public domain (https://sqlite.org/copyright.html).

## PacketDotNet and MPL-2.0

PacketDotNet is the one dependency that is not permissively licensed. MPL-2.0 is a
file-level copyleft: redistributing the library as-is only requires this notice and a
pointer to the source, which is what the table above provides. Modifying PacketDotNet's own
source files would additionally require publishing those modified files under MPL-2.0. NTT
uses the package unmodified.

## Not redistributed

- **Packet Monitor** (`pktmon.exe`) — part of Windows 10 1809 and later. NTT drives the copy
  already on the machine; nothing is redistributed. Switch discovery and packet capture use
  it instead of a third-party capture driver.
- **Segoe Fluent Icons / Segoe MDL2 Assets** — the icon fonts used by the interface ship with
  Windows and are used, not redistributed. On a Windows build without Segoe Fluent Icons the
  interface falls back to Segoe MDL2 Assets.
