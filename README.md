# dotnet-cleanse

A dotnet command tool that removes all build artifacts and folders, recursively and completely.

## Motivation

Visual Studio and `dotnet clean` both leave behind folders and other artifacts. This tool removes bin and obj folders with extreme prejudice.

Should behave essentially like this command from [this article](https://montemagno.com/easily-clean-bin-obj-folders/):

```powershell
Get-ChildItem .\ -include bin,obj -Recurse | foreach ($_) { remove-item $_.fullname -Force -Recurse }
```

## Installation

## Usage

