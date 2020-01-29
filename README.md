# IPFS Add Folder [![Build Status](https://dev.azure.com/cladular/ipfs-add-folder/_apis/build/status/cladular.ipfs-add-folder?branchName=master)](https://dev.azure.com/cladular/ipfs-add-folder/_build/latest?definitionId=4&branchName=master)

Recursively adds a folder to IPFS.

## Usage

```
npm install -g ipfs-add-folder --ignore-scripts
ipfs-add-folder <project-directory> <ipfs-node-url>
```
**Note:** The package must be installed with `--ignore-scripts` in order for the tool to work properly.

### Pinning Files & Folders

If you wish to `pin` the added files and folders you can use the `--pin` (or `-p`) option:

```
ipfs-add-folder <project-directory> <ipfs-node-url> --pin
```

### Quiet Execution

When the root hash created by the `add` operation is required for later operations (such as registering it in IPNS), you can use the `--quiet` (or `-q`) option:

```
ipfs-add-folder <project-directory> <ipfs-node-url> --quiet
```
