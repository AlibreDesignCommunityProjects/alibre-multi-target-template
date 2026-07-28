# Alibre Multi-Target Template

- This is an empty starter solution for writing an Alibre Design add-on in C#, F#, or VB.NET, with the build settings already sorted out.
  - What it does
    - Provides one project skeleton per language, so you can pick whichever you prefer.
    - Builds each project for .NET Framework 4.8.1, .NET 8, and .NET 9 from the same source.
    - Targets 64-bit and references the Alibre automation library in each project.
    - Contains build configuration only, so there is no add-on code to unpick.
  - Getting started
    - Open `source/AlibreXMultiTargetTemplate.sln`.
    - Delete the language projects you do not want.
    - Add your own add-on classes to the project you kept.
    - Build in Release and copy the output into your Alibre Design add-ons directory.
  - Where things live
    - `source/` holds the solution and the three project skeletons.
    - `documentation/` holds reference notes.
  - Use it under the MIT License.
