This source of Python is compiled to a executable onefile(.exe) by pyinstaller.

Require Tools:
    python 3.10.6~
    Option:
        VSCode
        git (minGit)

If do you want to change the source, you should make a venv and use pip pyinstaller to the venv.

install python or download Winpython (open a terminal in portablemode VSCode)
    extract vscode.zip and make "data" folder in directory where is same code.exe, This way will done to be portablemode vscode.

python only:
    After install,
    "python -m venv ."
    ".\Scripts\activate"
    pip install pyinstaller
    pyinstaller source.py --onefile --noconsole
    >>dist>>source.exe

winPython
    extract winPython
    .\scripts env_for_icons.bat  add>   SET PATH=C:\~~~\MinGit\ming64\bin;%PATH%
                                        vscode\Code.exe
        (Recommended for open vsc with this way by this bat)
    open VSCode, Import python project(Ex. Hello World). This process is effected to generate enviroment of python in inside vscode.
    If you want to use git, Download minGit and Set the path of minGit to VSCode.
        Ex. vscode > user-data > User > setting.json >> add "git.path": "C:\~~~\MinGit\ming64\bin\git.exe"
    Next, open CMD in winPython and execute commands of #python only section.
    
