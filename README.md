# Asobo Language File Modifier

## Usage
When you first start the program, you will be introduced to a command line (might change to a gui in the near future). The script will ask you to either automatically search for a language file, create a new file, or input a valid path to the file. If you choose to search, the script will try to find any language files on the current drive (Windows) or any folder in the system (Linux, not sure about MacOS, give it a try and let me know)

(don't worry, i don't collect your data lol this is an open source project)

Once the script finds any files, it will show the paths to them. You will have to choose a language file by its number in the list, starting from 0.

After you choose the file, you can start messing with the language file!

## Building
If you want to build the executable for yourself at any time:
1. Open the command line (both PowerShell and CMD work, on Linux (and probably MacOS too) it's usually Ctrl+Alt+T)
2. Git the repository
    * Either install git and clone the repo
        1. Install git
            * Windows: [Git](https://git-scm.com/download/win)
            * MacOS: use brew to install: `brew install git`
            * Linux: use your distribution's package manager to install
        2. Clone the repository: `git clone https://github.com/PizzArt/MALaF`
    * Or download the repository:

        ![Download ZIP image](/assets/download_zip.png)
3. Install PyInstaller using pip
    1. Install pip
        * Windows and MacOS python installations should have pip installed, reinstall python with pip if you don't have it
        * Linux: use your package manager to install `python-pip`
    2. Install PyInstaller: `pip install pyinstaller --user`
4. Change directory: `cd ./MALaF`
5. Use PyInstaller: `pyinstaller --clean -i ./assets/icon.png -n MALaF -F ./src/MALaF.py`
6. The executable should be in the `dist` folder
7. Done!

## Contributing
Feel free to contribute to the script, suggest new functions, report bugs if you find any, feedback is much appreciated.