# nuget
A tool to help use NuGet packages from Dyalog APL.

This code is used by Cider to support NuGet packages as dependencies. It requires Dyalog v19.0 and .NET 6.0 or later.

The code can also be used outside of Cider, but documentation is currently only in the form of the code in the Tests folder. To experiment with it from Dyalog version 19.0:

* Make sure you have installed .NET 6.0 or later and set DYALOG_NOTNET=1.
* Install NuGet using one of the following mechanisms:
** ]Tatin.LoadPackage NuGet (once this package has been created, which should be soon)
** Use ]get https://github.com/dyalog/nuget, which will establish NuGet.aplsource and NuGet.Tests
* Run some of the functions in the NuGet.Tests namespace
