# Aras Innovator FileType Extension Package
## Description
Official unofficial extension package for the FileType ItemType in Aras Innovator. Contains missing file type extensions especially for software files. 
Following FileTypes are included:

## Why this package?
tbd

## Project Details

#### Built Using:
Aras 12.0 SP7

#### Versions Tested:
Aras 12.0 SP7 and Release 2023

#### Browsers Tested:
Chrome


## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Prerequisites

1. Aras Innovator installed (version 12.0 SPx preferred)
2. Aras Package Import tool
3. Import package of this project

### Install Steps

#### Database Installation
1. Backup your database and store the BAK file in a safe place.
2. Open up the Aras Package Import tool.
3. Enter your login credentials and click **Login**
    * _Note: You must login as root for the package import to succeed!_
4. Enter the package name in the TargetRelease field.
    * Optional: Enter a description in the Description field.
5. Enter the path to your local `..\fileTypeExtension\Import\imports.mf` file in the Manifest File field.
6. Select **ai.ext.filetype.extensionpackage** in the Available for Import field.
7. If the target database has the Technical Documentation application installed, select the **ai.ext.filetype.extensionpackage** package.
8. If the target database has the MPP application installed, select the **ai.ext.filetype.extensionpackage** package.
9. Select Type = **Merge** and Mode = **Thorough Mode**.
10. Click **Import** in the top left corner.
11. Close the Aras Package Import tool.

The new FileTypes should now be available in your Innovator

## Usage

1. Login to Aras.
2. File uploads that represent files from the extension package are recognized correctly.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## Credits

Created by @AngelaIp

## License

This project is published to Github under the Microsoft Public License (MS-PL). See the [LICENSE file](./LICENSE.md) for license rights and limitations.
