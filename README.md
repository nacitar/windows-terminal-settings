# windows-terminal-settings

Installation via PowerShell (DELETES ANY EXISTING CONFIGURATION):
```powershell
$configDir = "${env:LOCALAPPDATA}\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\LocalState"
Remove-Item -Recurse -Force $configDir -ErrorAction Ignore
git clone https://github.com/nacitar/windows-terminal-settings.git $configDir
```


Icons were made via the included .svg files using ImageMagick:
```
magick convert -background none input.svg -define icon:auto-resize icon.ico
```