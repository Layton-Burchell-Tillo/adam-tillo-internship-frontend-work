# Getting started

## Download the files

1. Click the `Code` button in the top right of [the repository page](https://github.com/Layton-Burchell-Tillo/adam-tillo-internship-frontend-work) and select "Download ZIP".
2. Right-click the downloaded file and select "Extract Archive" or equivalent.

## Download a program for using the files

Generally the easiest editor to get started with is [VSCode](https://code.visualstudio.com/). Download it and get it installed.

After it is installed:
1. Open VSCode
2. In the top-left, select `File > Open Folder`
3. Select the folder you extracted the archive into (see Download the Files step 2)

## Download Node and PNPM to run the files

### Windows

As per the instructions on [the Node js website](https://nodejs.org/en/download) for installing LTS + Windows + Chocolatey + PNPM, you'll need [Chocolatey](https://chocolatey.org/install) which is a windows package manager.

#### Installing Chocolatey

1. You need to run some Powershell terminal commands as Admin. To open Powershell as admin: Hold the Win key, then press X, then press A and accept the admin warning
2. As per [the Node site](https://nodejs.org/en/download) copy/paste this code into Powershell and run it
    ```
    # Download and install Chocolatey:
    powershell -c "irm https://community.chocolatey.org/install.ps1|iex"

    # Download and install Node.js:
    choco install nodejs --version="24.16.0"

    # Verify the Node.js version:
    node -v # Should print "v24.16.0".

    # Download and install pnpm:
    corepack enable pnpm

    # Verify pnpm version:
    pnpm -v
    ```

If a number came out at the end, that worked! If not, something went wrong and I'll need details to help with it. If that happens, go to the Issues tab of github and create an issue explaining as much as possible (but make sure you don't include any personal info!)

### Mac

1. As per [the Node site](https://nodejs.org/en/download) copy/paste this code into Powershell and run it
    ```
    # Download and install Chocolatey:
    powershell -c "irm https://community.chocolatey.org/install.ps1|iex"

    # Download and install Node.js:
    choco install nodejs --version="24.16.0"

    # Verify the Node.js version:
    node -v # Should print "v24.16.0".

    # Download and install pnpm:
    corepack enable pnpm

    # Verify pnpm version:
    pnpm -v
    ```

If a number came out at the end, that worked! If not, something went wrong and I'll need details to help with it. If that happens, go to the Issues tab of github and create an issue explaining as much as possible (but make sure you don't include any personal info!)

## Running the project

1. Back in VSCode, open a new terminal. Do this by selecting `Terminal > New terminal` in the top-left of the editor
2. In the terminal, enter `pnpm install`
3. In the terminal, enter `pnpm dev`

This should run the server!

You can see the output by going to http://localhost:3000

Best of luck, and happy coding! 👾
