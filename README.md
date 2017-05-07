
# WonderfulWindowsWorkflow
A list of tweaks and applications to improve your workflow in Windows


# Adding a folder to 'this pc' menu and mapping it to a drive letter
What are the advantages of doing this?
- Direct access to commonly used folders on your drive
- Map a certain drive letter to this folder -> this makes installation of programs into that folder very convenient

How to do it:
## Adding the local drive as a network drive
Computer -> Map network drive -> chose drive letter and specify path //localhost/c$/'path'
Make sure to change the option in View -> Options -> Open file explorer to, is set to "this pc"

## Network Drive installation enable
Change this key in your registry or run 'EnableNetworkInstall.reg':
HKEY_LOCAL_MACHINE/SOFTWARE/Microsoft/Windows/CurrentVersion/Policies/System
create a new DWORD entry with the name EnableLinkedConnections and value 1

This registry change will allow installers to install directly into a selected folder mapped as a network drive.
In some cases, even with this fix, certain installers might disallow installing to a network location.
