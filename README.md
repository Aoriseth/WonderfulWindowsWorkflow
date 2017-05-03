# WonderfulWindowsWorkflow
A list of tweaks and applications to improve your workflow in Windows


## Add local drive as network drive
Computer -> Map network drive -> chose drive letter and specify path //localhost/c$/'path'

## Network Drive installation enable
HKEY_LOCAL_MACHINE/SOFTWARE/Microsoft/Windows/CurrentVersion/Policies/System
create a new DWORD entry with the name EnableLinkedConnections and value 1
