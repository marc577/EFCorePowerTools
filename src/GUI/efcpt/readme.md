# efcpt - EF Core Power Tools CLI

Cross platform command line tool that for advanced EF Core reverse engineering. See the a full guide explaining all the features [here](https://github.com/ErikEJ/EFCorePowerTools/wiki/Reverse-Engineering).

## Getting started

The tool runs on any computer with the .NET 6.0 runtime installed.

1. Install/update the tool

```bash
dotnet tool install -g ErikEJ.EFCorePowerTools.CLI
```

```bash
dotnet tool update -g ErikEJ.EFCorePowerTools.CLI
```

2. Run the tool from the folder where you want the code to be generated (usually where your .NET project is located)

```bash
efcpt "Data Source=(local);Initial Catalog=Northwind;User id=user;Pwd=secret123;Encrypt=false" mssql
```

A configuration file `efcpt-config.json` is created in the output folder, and you can open this file in your editor to modify the default options. If your editor supports it (for example VS Code), it will provide syntax guidance for the file.

To get command line syntax help, run

```bash
efcpt help
```