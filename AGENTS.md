# AGENTS.md

Notes for working in this repo:
- CLI options and help live in `programs/zstdcli.c`.
- Compression flow and preferences live in `programs/fileio.c` and `programs/fileio_types.h`.
- Seekable format code is in `contrib/seekable_format` and must be linked into the CLI builds.
- Make build: run `make -C programs zstd` (or `make` from repo root).
- CMake build: configure from `build/cmake` (top-level `CMakeLists.txt` delegates there).
- When adding CLI options, also update `FIO_displayCompressionParameters()` if they should appear in verbose output.
