# IronBrew 2

VM-based Lua 5.1 obfuscation.

## Overview

IronBrew 2 is a Lua 5.1 obfuscator that uses VM-based obfuscation techniques to protect Lua scripts. This repository contains the complete source code imported from [pw4k/ironbrew-2](https://github.com/pw4k/ironbrew-2).

## Project Structure

- **IronBrew2/** - Core obfuscation library
  - **Bytecode Library/** - Lua bytecode handling (serialization, deserialization)
  - **Obfuscator/** - Obfuscation engine with opcodes, control flow, encryption
  - **Extensions/** - C# utility extensions
  
- **IronBrew2 CLI/** - Command-line interface for the obfuscator

- **Lua/** - Lua scripts and tools
  - **Minifier/** - Lua source code minification tools
  - **compress.lua** - Compression utilities

- **Tests/** - Test scripts for validation

## Build Requirements

- .NET Core 3.1 SDK or later
- C# 8.0 or later

## Building the Project

To build the project, use the Visual Studio solution file:

```bash
dotnet build IronBrew2_Core.sln
```

Or build individual projects:

```bash
dotnet build IronBrew2/IronBrew2.csproj
dotnet build "IronBrew2 CLI/IronBrew2 CLI.csproj"
```

## Dependencies

- System.Text.Encoding.CodePages (4.6.0-preview.18571.3)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Copyright (c) 2019 DefCon42
