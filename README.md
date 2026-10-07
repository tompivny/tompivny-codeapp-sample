# tompivny-codeapp-sample

A small demo of the project types in [TALXIS DevKit Build](https://github.com/TALXIS/tools-devkit-build).

It has two projects:

- `src/Contoso.Sample.Solution` - a Power Platform solution (`ProjectType=Solution`).
- `src/Contoso.Sample.CodeApp` - a Power Apps code app (`ProjectType=CodeApp`).

The solution references the code app with a `ProjectReference`. When you build the solution, the code app is built and packed into the solution zip.

## Build

You need the .NET SDK and Node.js.

```
dotnet build src/Contoso.Sample.Solution
```

The output is `src/Contoso.Sample.Solution/bin/Debug/net472/Contoso.Sample.Solution.zip`.
