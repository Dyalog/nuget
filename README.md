# nuget
A tool to help use NuGet packages from Dyalog APL.

This code is used by Cider to support NuGet packages as dependencies. It requires Dyalog v19.0 and .NET 6.0 or later.

The code can also be used outside of Cider, but documentation is currently only in the form of the code in the Tests folder. 

To run these tests in Dyalog version 19.0, you must:

* Make sure you have installed .NET 6.0 or later and set DYALOG_DOTNET=1.
* Install NuGet using one of the following mechanisms:
  * ]Tatin.LoadPackage NuGet (once this package has been created, which should be within the next couple of days if all goes well)
  * ]get https://github.com/dyalog/nuget, which will establish NuGet.APLSource and NuGet.Tests

To get a list of runnable tests:

```
    Tests.test ''
The current test functions exist:
 test_clock  test_mailkit  test_parquet  test_selenium 
```

To run a test:

```
    Tests.test 'selenium'
Created project file "/tmp/nuget-test/nuget-test.csproj"
Added/Updated:  Selenium.WebDriver  Selenium.WebDriver.ChromeDriver 
Successfully loaded Dyalog - Home
```