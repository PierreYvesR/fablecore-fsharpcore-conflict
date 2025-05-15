`dotnet restore` then `dotnet build` will produce the following warnings

```
warning MSB3277: Found conflicts between different versions of "FSharp.Core" that could not be resolved. [C:\git\fable-core-test\fablecore-fsharpcore-conflict\test-fablecore-fsharpcore\test-fablecore-fsharpcore.fsproj::TargetFramework=net48]
warning MSB3277: There was a conflict between "FSharp.Core, Version=7.0.0.0, Culture=neutral, PublicKeyToken=b03f5f7f11d50a3a" and "FSharp.Core, Version=9.0.0.0, Culture=neutral, PublicKeyToken=b03f5f7f11d50a3a". [C:\git\fable-core-test\fablecore-fsharpcore-conflict\test-fablecore-fsharpcore\test-fablecore-fsharpcore.fsproj::TargetFramework=net48]
...
```

This `net48` project references `Fable.Core 4.5.0` and `FSharp.Core 7.0.0`.

