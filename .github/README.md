# Alibre Multi-Target Template

A starter solution for building Alibre Design (AlibreX) add-ons that target multiple .NET runtimes, with parallel project setups for C#, F#, and VB.NET so you can start in your preferred language.

## What's Included
- A Visual Studio solution (`source/AlibreXMultiTargetTemplate.sln`) with three sibling projects.
- C# (`AlibreXMultiTargetTemplateCs`), F# (`AlibreXMultiTargetTemplateFs`), and VB.NET (`AlibreXMultiTargetTemplateVb`) project skeletons, so you can start in your preferred language.
- Multi-targeting preconfigured for `net481`, `net8.0`, and `net9.0`.
- An `x64` platform target and a reference to `AlibreX.dll` already wired into every project.

These projects are empty scaffolds: they establish the build configuration and the Alibre reference but contain no add-on source code yet. Add your own classes to begin.

## Requirements
- Alibre Design (the projects reference `AlibreX.dll`; the included reference path points at version `29.0.0.29060`).
- .NET SDK capable of building `net481`, `net8.0`, and `net9.0` (Windows, x64).
- Visual Studio 2022 (17.x) or a compatible toolchain.

## Getting Started
1. Open `source/AlibreXMultiTargetTemplate.sln`.
2. Update the `AlibreX` reference `HintPath` in each project file to match your local Alibre Design installation directory.
3. Restore and build. Each project produces assemblies for all three target frameworks.

## Customizing
- Keep the language project you want and remove the others from the solution if you only need one.
- Add your add-on source files to the chosen project; the AlibreX reference and target frameworks are already in place.
- Adjust the `TargetFrameworks` value in the project file(s) if you need to support fewer or different runtimes.

## License
See [LICENSE](../LICENSE).
