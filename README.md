# Issaclin32's scoop bucket

generated from https://github.com/Ash258/GenericBucket

## Files and helpers

### `bucket` Folder

- All manifests belong here
- `.gitkeep` file could be removed after you push your first manifest

### `.vscode` Folder

Contains all syntax highlighting, code formating, manifest creating tools you could use.

- Extensions
    - All extensions which will save your time while writing manifests are in recommended sections
    - You will be notified about installing them when you open project
- Settings
    - All settings are set to be compatible with Appveyor pipeline and upstream (official) repositories
        - No need to worry about formating restrictions between repositories.
- Code snippets
    - > Code snippets are templates that make it easier to enter repeating code patterns, such as loops or conditional-statements.
    - You could use workspace wide code snippets for speed up manifest creating
    - While editing json file write partitial name of snippet and press `tab`
    - Available Json snippets:
        - `app`
            - Create default manifest structure
        - `appArch`
            - Create default manifest structure with full acrchitecture
        - `arch`
            - Create only architecture property with 64bit and 32bit
        - `upAr`
            - Create autoupdate property with architecture
        - `persistCheck`
            - Installer / pre_install script for checking if file is already persisted or need to be created

### `bin` Folder

Scripts which will save you much time while debuging and writing manifests.
If you need help how to use them just run `Get-Help .\bin\<BINARY>.ps1`.

### `Scoop-Bucket.Tests.ps1` File

- Test which are executed inside Appveyor pipeline
- Also are executed as `pre-commit` hook

### `config files`

- `.appveyor.yml`
    - Definition of Appveyor CI pipeline
- `.editorconfig`
    - Universal configuration file, compatible with all types of editors
    - Defines how files should look
- `.gitattributes`
    - Simplifying line endings for git
    - No need to configure `auto.clrf` setting on each clone or new workspaces
