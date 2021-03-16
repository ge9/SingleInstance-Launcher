# Single-Instance-launcher
Select multiple files from Windows Explorer menu and launch just one instance of process
- [Original readme](https://github.com/zenden2k/context-menu-launcher)
- Sample registry file for the Textrument Editor: ( Notepad++ )
```
Windows Registry Editor Version 5.00

[HKEY_CLASSES_ROOT\*\shell\TextrumentInst]
@="用 &Textrument 打开（新实例）"
"Icon"="D:\\Code\\FigureOut\\Textrument\\PowerEditor\\bin64\\Textrument.exe"
"MultiSelectModel"="Player"

[HKEY_CLASSES_ROOT\*\shell\TextrumentInst\Command]
@="\"D:\\Code\\NVPACK\\singleinstance.exe\" \"%1\" \"D:\\Code\\FigureOut\\Textrument\\PowerEditor\\bin64\\Textrument.exe\" $files --si-timeout 50 -multiInst -nosession" 

```