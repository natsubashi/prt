This source of Python is compiled to a executable onefile(.exe) by pyinstaller.

Require Tools:
- python 3.10.6~

Option:
- VSCode https://code.visualstudio.com/download
- git (minGit) https://github.com/git-for-windows/git/releases

If do you want to change the source, you should make a venv and use pip pyinstaller to the venv.  
install python or download Winpython (open a terminal in portablemode VSCode)

extract vscode.zip and make "data" folder in directory where is same code.exe, This way will done to be portablemode vscode.

python only:
- After install,
- "python -m venv ."
- ".\Scripts\activate"
- pip install pyinstaller
- pyinstaller source.py --onefile --noconsole
- >>dist>>source.exe

winPython: https://winpython.github.io/  3.12.6.0.7zip
- extract winPython
- .\scripts env_for_icons.bat  add>
  - SET PATH=C:\xxxx\MinGit\ming64\bin;%PATH%
  - vscode\Code.exe
  - (Recommended for open vsc with this way by this bat)
- open VSCode, Import python project(Ex. Hello World). This process is effected to generate enviroment of python in inside vscode.
  - If you want to use git, Download minGit and Set the path of minGit to VSCode.
    - Ex. vscode > user-data > User > setting.json >> add "git.path": "C:\xxxx\MinGit\ming64\bin\git.exe"
  - Next, open CMD in winPython and execute commands of #python only section.
    
Python (ms-python.python)
Git Graph (mhutchie.git-graph)
Python Indent (kevinrose.vsc-python-indent)
Highlight (fabiospampinato.vscode-highlight)
Japanese Language Pack (ms-ceintl.vscode-language-pack-ja)


Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process


vscodeのセットアップ
visualstudioで作ったwindowsformapp1.csprojおよびwindowsformapp1.slnをvscodeで読み込ませると、Intellisenceがはたらくようになる？

npgsql2.2.1.nupkgを、vscodeのnuget拡張のaddPackageからnpgsql2.2.1を指定して入手　unzipして中のnpgsql.dllおよびmono.security.dllをps1ファイルがあるカレントディレクトリにコピー
キャメルケースに注意しながら、-ReferencedAssembliesに列挙 ディレクトリに置いたdllは ".\Npgsql.dll", `のように列挙する
Npgsql C onnectionでないとエラーになる
usingは
using Npgsql;
using Mono.Security;
でよい　ただしくps1内でreferencedassembliesできているならば





