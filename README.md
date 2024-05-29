# How to add?

1. Go to the folder of the project
2. Open Git Bash
3. Input the following code

Code: 

`git submodule add https://github.com/ItsNotDaan/KiCad_Lib_ItsNotDaan.git Library/GitHub_Library`


## To Update if needed:

Code:

`git submodule update --remote --merge`

## To push changed to main:
```bash
git checkout externalChanges
git add .
git commit -m "Restored Version"
git push origin externalChanges
```

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

# Add to custom KiCad Project:

### Symbol Library:
Preferences -> Manage Symbol Libraries... -> Project Specific Libraries -> Bottom Left (+) icon.
- Nickname: `GitHub_Library`
- Library Path: `${KIPRJMOD}/Library/GitHub_Library/PCB_Lib_ItsNotDaan.kicad_sym`
Press OK

### Footprint Library:
Preferences -> Manage Symbol Libraries... -> Project Specific Libraries -> Bottom Left (+) icon.
- Nickname: `GitHub_Library`
- Library Path: `${KIPRJMOD}/Library/GitHub_Library/PCB_Lib_ItsNotDaan.pretty`
Press OK
