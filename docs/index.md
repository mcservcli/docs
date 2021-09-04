CLI utility to manage MC server installations.

# Features

- Install required JDKs
- Download server files
- Generate start scripts (with optimized JVM flags)
- Update to the latest build


# Supported Platforms

| Platform | Supported |
| ------ | ----- |
| Windows | ✔ |
| Linux | ✔ |
| macOS¹ | 🚧 |

¹ In theory macOS should be supported, there are just no macOS specific implementations yet

# Supported Server Distributions

| Distribution | Install | Update | Metadata¹ |
| --- | --- | --- | --- |
| PaperMC | ✔ | ✔ | ✔ |
| Waterfall | ✔ | ✔ | ❌ |
| Travertine | ✔ | ✔ | ❌ |
| PurPur | ✔ | ✔ | ❌ |
| Velocity² | ✔ | ✔³ | ❌ |

¹ Metadata is required to ensure the correct Java version is installed and use proper JVM flags

² Velocity does not provide checksums on their Downloads so no checksum verification will be made when downloading
velocity

³ Velocity does not provide information on when a new build got released over an API, therefore mcserv will re-download
Velocity each time you run the update command.
