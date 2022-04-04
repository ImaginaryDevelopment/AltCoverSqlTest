# Repro Steps

## repo setup

```cmd
dotnet new -i "MiniScaffold::*"
dotnet new mini-scaffold -n AltCoverTest --githubUsername ImaginaryDevelopment
git init
```

## simplify repo

commit everything
remove analyzer and formatter - assumed not relevant to the repro

```cmd
.\build.cmd dotnettest
```

## work on reproduction of problem

add sqlclient, and docker

```cmd
dotnet paket add -p .\tests\AltCoverTest.Tests\AltCoverTest.Tests.fsproj System.Data.SqlClient
```
