# Alibre Multi-Target Template

A starter Visual Studio solution for building Alibre Design (AlibreX) add-ons in C#, F#, or VB.NET with multi-targeted .NET builds.

Use this as a starting point. It contains no finished add-on. The solution holds three sibling project skeletons, one per language, each set to reference `AlibreX.dll` and to multi-target `net481`, `net8.0`, and `net9.0` on x64. The projects carry no add-on source yet, so add your own classes to the language project you want and remove the others if you need only one.

## Table Of Contents

- [What Is Here](#what-is-here)
- [Official Alibre Resources](#official-alibre-resources)
- [Requirements](#requirements)
- [Quick Start](#quick-start)
- [Key Files](#key-files)
- [Key Folders](#key-folders)
- [Notes](#notes)
- [License](#license)

## What Is Here

- A Visual Studio solution (`source/AlibreXMultiTargetTemplate.sln`) with three sibling projects.
- Empty project skeletons for C# (`AlibreXMultiTargetTemplateCs`), F# (`AlibreXMultiTargetTemplateFs`), and VB.NET (`AlibreXMultiTargetTemplateVb`).
- Multi-targeting set to `net481`, `net8.0`, and `net9.0` in every project.
- An `x64` platform target and an `AlibreX.dll` reference wired into each project.
- Build configuration only. The projects hold no add-on classes.

## Official Alibre Resources

Alibre's official resources for API development and AI/LLM/agent workflows: <https://www.alibre.com/api/>

## Requirements

- Alibre Design. The reference `HintPath` points at version `29.0.0.29060`; adjust it to your install.
- A .NET SDK able to build `net481`, `net8.0`, and `net9.0`.
- Windows, x64.
- Visual Studio 2022 (17.x) or a compatible MSBuild toolchain.

## Quick Start

1. Open `source/AlibreXMultiTargetTemplate.sln`.
2. Update the `AlibreX` reference `HintPath` in each project file to match your Alibre Design install directory.
3. Restore and build. Each project produces assemblies for all three target frameworks.

## Key Files

| File | Purpose |
| --- | --- |
| `source/AlibreXMultiTargetTemplate.sln` | Visual Studio solution referencing the C#, F#, and VB.NET projects. |
| `source/AlibreXMultiTargetTemplateCs/AlibreXMultiTargetTemplateCs.csproj` | C# project skeleton. Targets `net481`, `net8.0`, `net9.0`; x64; nullable enabled; `LangVersion` 9.0. |
| `source/AlibreXMultiTargetTemplateFs/AlibreXMultiTargetTemplateFs.fsproj` | F# project skeleton. Same target frameworks; x64; XML documentation generation on. |
| `source/AlibreXMultiTargetTemplateVb/AlibreXMultiTargetTemplateVb.vbproj` | VB.NET project skeleton. Same target frameworks; x64. |
| `source/alibre.disclaimer.txt` | MIT note and Alibre trademark and ownership disclaimer. |
| `LICENSE` | MIT license text. |
| `.gitignore` | Build output and editor ignores. |

## Key Folders

| Folder | Purpose |
| --- | --- |
| `source/` | Solution and the three language projects. |
| `source/AlibreXMultiTargetTemplateCs/` | C# project. |
| `source/AlibreXMultiTargetTemplateFs/` | F# project. |
| `source/AlibreXMultiTargetTemplateVb/` | VB.NET project. |
| `.github/` | Repository docs and templates: this README, contributing guide, code of conduct, issue templates, and pull request template. |
| `documentation/` | Placeholder for documentation. Currently empty. |
| `submodules/` | Placeholder for git submodules. Currently empty. |
| `reviews/` | Code review notes. |

## Notes

- The projects are empty scaffolds. They set up build configuration and the AlibreX reference but hold no add-on classes.
- Keep the language project you want and remove the others from the solution if you need only one.
- Adjust the `TargetFrameworks` value in a project file to support fewer or different runtimes.
- The bundled `HintPath` points at `C:\Program Files\Alibre Design 29.0.0.29060\Program\AlibreX.dll`. Change it to your local path.
- Alibre, Alibre Design, and Alibre Script names and related materials belong to their respective owners.

## License

See [LICENSE](../LICENSE). MIT.
