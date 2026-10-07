# tompivny-codeapp-sample

A small demo of the project types in [TALXIS DevKit Build](https://github.com/TALXIS/tools-devkit-build).

It has two projects:

- `src/Contoso.Sample.Solution` - a Power Platform solution (`ProjectType=Solution`).
- `src/Contoso.Sample.CodeApp` - a Power Apps code app (`ProjectType=CodeApp`).

The solution references the code app with a `ProjectReference`. When you build the solution, the code app is built and packed into the solution zip.

## Build

You need the .NET SDK and Node.js.

```
dotnet publish Contoso.Sample.slnx
```

Outputs:

- `src/Contoso.Sample.Solution/bin/Debug/net472/Contoso.Sample.Solution.zip` - the solution with the code app inside.
- `src/Contoso.Sample.Solution/bin/Debug/Contoso.Sample.Solution.<version>.nupkg` - the same solution as a NuGet package.
