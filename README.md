# Aras Innovator FileType Extension Package
## Description
Official unofficial extension package for the FileType ItemType in Aras Innovator. Contains missing file type extensions especially for software files. 

The additional FileTypes are very helpful for exotic file types that are not self explaining for the end user. The additional FileTypes help users to understand to understand the context of a File more easily. It´s not a killer enhancement, but it´s a nice and low cost improvement. 

Following FileTypes are included:

tbd
7z, exe, ini, bat, ico, bin, tar, app, ...


## Why this package?

#Consistency Across Environments:
Standardizing the file type table ensures that all users maintain a consistent environment. Without standardization, different users might have variations in their tables, leading to compatibility issues when exchanging data or collaborating on the project.

#Avoids Runtime Errors:
Inconsistent table structures can result in runtime errors, making it challenging to identify and debug issues. Standardization reduces the risk of runtime errors related to the file type management, providing a more stable and predictable development environment.

#Enhances Collaboration:
Standardization facilitates collaboration by providing a common ground for all contributors. When everyone follows the same structure, it becomes easier for developers to understand, review, and build upon each other's work. This, in turn, accelerates the development process and fosters a more cohesive community of contributors.

#Simplifies Maintenance
A standardized file type table simplifies maintenance tasks. Updates and modifications to the table can be implemented more smoothly when everyone adheres to a shared structure. This ensures that new file types and changes are seamlessly integrated into the existing system without causing disruptions.

#Mitigates Data Integrity Risks:
Inconsistent file type tables pose risks to data integrity. Standardization helps mitigate these risks by providing a reliable framework for managing file types. Users can confidently rely on the stability of the table, ensuring that data associated with specific file types remains accurate and dependable.

#Sustainable Development Practices:
Standardization aligns with sustainable development practices. It establishes a foundation for long-term project growth and maintenance, making it easier for the project to evolve over time. Adopting standardized structures contributes to the project's longevity and adaptability.


## IMPORTANT

Innovator automatically assings the new FileTypes to the Files in the Vault! This step cannot be reverted easily. Only use this project if you really want to use the FileTypes!

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
