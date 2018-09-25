## Sogu
This script generates a list of
possible SOGU filenames based on serial numbers of active drives. It has the
added functionality of searching each drive from the generated file list.

## DESCRIPTION
This script uses C# code to generate a list of SOGU filenames based on the algorithm used in the SOGU implant.
The script then utilizes PowerShell to query the system for drive information and, if selected, locates any Sogu files found on disk. 
The script can be deployed domain-wide to enumerate hosts to locate malicious files.
                                               
## Commands to import this script for use                                
To import the powershell script for use enter the following commands in the PowerShell Console 

```
PS> cd c:\Users\<username>\<folder that contains this script>
PS> import-module SoguFileSearch.ps1
```
### Parameters
```
ShowFileNames         Displays a list of all possible Sogu log filenames generated for each drive.
CustomSerial          1. Displays a list of all possible Sogu log filenames generated based on the 
                      Serial Number provided by the user. 
                      2. A user can provide a single or list of serials in the form of an array in the powershell 
                      console or a user generated text file.
                      3. If the Serial Number entered does not correlate to an active local drive on the machine 
                      the user is prompted with an error message.







```
