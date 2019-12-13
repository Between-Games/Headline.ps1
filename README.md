# Headline.ps1

PowerShell script that generates a headline using the provided parameters.

## Prerequisites

The script makes use of the `Set-Clipboard` function which was first made available on the Windows Powershell 5.0 version. If you have an older version of Windows PowerShell or using PowerShell Core, you may instead download the [ClipboardText](https://www.powershellgallery.com/packages/ClipboardText) module. Once done, the script should function correctly.

```
Install-Module -Name ClipboardText;
```

## Execution

The script can and should be called using the following ordered parameters:

* `$headline`: The value that will be deconstructed to create the headline
* `$linePrefix`: The value that will be inserted at the very front of each line
* `$lineSuffix`: The valuethat will be inserted at the very end of each line

```
.\Headline.ps1

# ╔════╗╔═╗╔═╗   ╔═╗╔═╗      ╔═╗
# ║ ╔╗ ║║ ║║ ║   ║ ║║ ║      ║ ║
# ║ ║║ ║║ ║║ ║   ║ ║║ ║      ║ ║
# ║ ║║ ║║ ║║ ║   ║ ║║ ║      ║ ║
# ║ ║║ ╚╝ ║║ ╚═══╝ ║║ ╚═════╗║ ╚═════╗
# ╚═╝╚════╝╚═══════╝╚═══════╝╚═══════╝
```

```
.\Headline.ps1 "test"

# ╔═══════╗╔═══════╗╔═══════╗╔═══════╗
# ╚══╗ ╔══╝║ ╔═════╝║ ╔═════╝╚══╗ ╔══╝
#    ║ ║   ║ ╚═════╗║ ╚═════╗   ║ ║
#    ║ ║   ║ ╔═════╝╚═════╗ ║   ║ ║
#    ║ ║   ║ ╚═════╗╔═════╝ ║   ║ ║
#    ╚═╝   ╚═══════╝╚═══════╝   ╚═╝
```

```
.\Headline.ps1 "test" "// "

// ╔═══════╗╔═══════╗╔═══════╗╔═══════╗
// ╚══╗ ╔══╝║ ╔═════╝║ ╔═════╝╚══╗ ╔══╝
//    ║ ║   ║ ╚═════╗║ ╚═════╗   ║ ║
//    ║ ║   ║ ╔═════╝╚═════╗ ║   ║ ║
//    ║ ║   ║ ╚═════╗╔═════╝ ║   ║ ║
//    ╚═╝   ╚═══════╝╚═══════╝   ╚═╝
```

```
.\Headline.ps1 "html" "<!-- " " -->"

<!-- ╔═╗   ╔═╗╔═══════╗╔═══════╗╔═╗       -->
<!-- ║ ║   ║ ║╚══╗ ╔══╝║ ╔╗ ╔╗ ║║ ║       -->
<!-- ║ ╚═══╝ ║   ║ ║   ║ ║║ ║║ ║║ ║       -->
<!-- ║ ╔═══╗ ║   ║ ║   ║ ║║ ║║ ║║ ║       -->
<!-- ║ ║   ║ ║   ║ ║   ║ ║║ ║║ ║║ ╚═════╗ -->
<!-- ╚═╝   ╚═╝   ╚═╝   ╚═╝╚═╝╚═╝╚═══════╝ -->
```

## Author

* Gabriel Roy - Repository Owner - [S-A-R-C](https://github.com/S-A-R-C)

See also the list of [contributors](https://bitbucket.org/S-A-R-C-TEAM/profile/members) who are linked to this project.

## License

This project is licensed under the MIT License - see the LICENSE file for details

## Acknowledgments

* Thank you to Michael Klement for the the [ClipboardText](https://www.powershellgallery.com/packages/ClipboardText) module