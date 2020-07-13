# KiJLC

![KiJLC logo](img/KiJLC_128x128.png)

An inofficial plugin for eeschema and pcbnew to export BOM and CPL files compliant with JLCSMT. We're not affiliated with JLC. Please double check your data as there might still be bugs.

## Usage

Clone the repo to `~/.kicad/scripting/plugins/KiJLC` and it will load the next time pcbnew is opened. Example:  
```sh
mkdir -p ~/.kicad/scripting/plugins
cd ~/.kicad/scripting/plugins
git clone https://github.com/fullyautomated/KiJLC
```

For eeschema create a new BOM plugin entry under Tools->Generate Bill of Materials:

![BOM Dialog](img/BOM_dialog.png)

Command line:

```sh
/usr/bin/python3  "~/.kicad/scripting/plugins/KiJLC/bom2jlc.py" "%I" "%O"
```
