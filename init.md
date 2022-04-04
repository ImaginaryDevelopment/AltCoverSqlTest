# Repro Steps

## repo setup

```cmd
dotnet new -i "MiniScaffold::*"
dotnet new mini-scaffold -n AltCoverTest --githubUsername ImaginaryDevelopment
git init
```

## next steps

commit everything
remove analyzer and formatter - assumed not relevant to the repro

```cmd
.\build.cmd dotnettest
```
