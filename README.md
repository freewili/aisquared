# AiSquared Controller

Downloads for **AiSquared Controller**, a native workspace for coding agents,
projects and models across your machines. Use the built-in ai2code agent or
run Claude Code, Codex, Grok and OpenCode in project terminals; plan work,
queue prompts, review session changes and control remote sessions.

This repository holds the release packages only. Get the latest from
[Releases](https://github.com/freewili/aisquared/releases/latest).

## Windows

Choose one package. Both need an x64 CPU with AVX2.

| Package | Speech |
| --- | --- |
| `AiSquared-Controller-<version>-windows-x64.zip` | Built-in speech on the CPU |
| `AiSquared-Controller-<version>-windows-x64-cuda.zip` | Built-in speech on an NVIDIA GPU (Turing / RTX 20 series or newer, CUDA 13.3-compatible driver), or the CPU |

1. Extract the whole ZIP to a writable folder, such as `C:\Apps\AiSquared`.
2. Double-click **Launch AiSquared.cmd**, or run `bin\AISquared.exe`.
3. Install and sign in to your agent CLI, then select its project and press
   **Start**. For OpenCode or chat, configure a local or remote model first.

Each ZIP has a `.sha256` file beside it, records its source commit in
`VERSION.txt`, and lists every file's checksum in `SHA256SUMS.txt`.

Git is needed for branch information and session change snapshots. Agent CLIs,
llama-server and model files are installed separately; the app can download
GGUF models from Hugging Face.

## Updating

Choose **File > Stop agents and exit**, then replace the executable, the
bundled DLLs and the assets in `bin/`. Keep `data/`, `models/`, `engine/`,
`project-types/`, `agentpersona/`, `userpersona/` and any `bin/location.txt`.

Releases before 0.2.12, and the Linux and macOS packages, are published on
Intrepid's GitLab.

## License

Copyright Intrepid Control Systems, Inc. Free for personal and evaluation use;
other use needs a commercial license. Send license questions and requests to
[icsorders@intrepidcs.com](mailto:icsorders@intrepidcs.com). See
[LICENSE.txt](LICENSE.txt) for the terms. Bundled third-party components keep
their own licenses, included in each package.
