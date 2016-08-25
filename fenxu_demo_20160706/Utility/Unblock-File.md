---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294021
schema: 2.0.0
---

# Unblock-File
## XXXXXXXX
Xxxxxxxx xxxxx xxxx xxxx xxxxxxxxxx xxxx xxx Xxxxxxxx.

## XXXXXX

### ByPath (Default)
```
Unblock-File [-Path] <String[]> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

### ByLiteralPath
```
Unblock-File -LiteralPath <String[]> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxxx$Xxxx xxxxxx xxxx xxx xxxx xxxxx xxxx xxxx xxxxxxxxxx xxxx xxx Xxxxxxxx.
Xx xxxxxxxx Xxxxxxx XxxxxXxxxx xxxxxx xxxxx xxxx xxxx xxxxxxxxxx xxxx xxx Xxxxxxxx xx xxx xxx xxx xxxx$ xxxx xxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxx xxxxxx xx XxxxxxXxxxxx.
Xx xxxxxxx$ xxxxx xxxxx xxx xxxxxxx xx xxxxxxx xxx xxxxxxxx xxxx xxxxxxxxx xxxxx.

Xxxxxx xxxxx xxx Xxxxxxx$Xxxx xxxxxx$ xxxxxx xxx xxxx xxx xxx xxxxxx xxx xxxxxx xxxx xx xx xxxx xx xxxx.

Xxxxxxxxxx$ xxx Xxxxxxx$Xxxx xxxxxx xxxxxxx xxx Xxxx.Xxxxxxxxxx xxxxxxxxx xxxx xxxxxx$ xxxxx xxx x xxxxx xx $0$ xx xxxxxxxx xxxx xx xxx xxxxxxxxxx xxxx xxx Xxxxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx Xxxxxxx XxxxxXxxxx xxxxxxxxx xxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

Xxxx xxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxxx x xxxx
```
PS C:\>Unblock-File -Path C:\Users\User01\Documents\Downloads\PowerShellTips.chm
```

Xxxx xxxxxxx xxxxxxxx xxx XxxxxXxxxxXxxx.xxx xxxx.

### Xxxxxxx 0$ Xxxxxxx xxxxxxxx xxxxx
```
PS C:\>dir C:\Downloads\*PowerShell* | Unblock-File
```

Xxxx xxxxxxx xxxxxxxx xxx xx xxx xxxxx xx xxx X$$Xxxxxxxxx xxxxxxxxx xxxxx xxxxx xxxxxxx $XxxxxXxxxx$.
Xx xxx xxx x xxxxxxx xxxx xxxx xxx xxxxx xxx xxxx xxxxxxxx xxxx xxx xxxxx xxx xxxx.

### Xxxxxxx 0$ Xxxx xxx xxxxxxx xxxxxxx
```
The first command uses the Stream parameter of the Get-Item cmdlet get files with the Zone.Identifier stream.Although you could pipe the output directly to the Unblock-File cmdlet (Get-Item * -Stream "Zone.Identifier" -ErrorAction SilentlyContinue | ForEach {Unblock-File $_.FileName}), it is prudent to review the file and confirm that it is safe before unblocking.
PS C:\>Get-Item * -Stream "Zone.Identifier" -ErrorAction SilentlyContinue
   FileName: C:\ps-test\Start-ActivityTracker.ps1

Stream                   Length
------                   ------
Zone.Identifier              26

The second command shows what happens when you run a blocked script in a Windows PowerShell session in which the execution policy is RemoteSigned. The RemoteSigned policy prevents you from running scripts that are downloaded from the Internet unless they are digitally signed.
PS C:\>C:\ps-test\Start-ActivityTracker.ps1
c:\ps-test\Start-ActivityTracker.ps1 : File c:\ps-test\Start-ActivityTracker.ps1 cannot
be loaded. The file c:\ps-test\Start-ActivityTracker.ps1 is not digitally signed. The script
will not execute on the system. For more information, see about_Execution_Policies at
http://go.microsoft.com/fwlink/?LinkID=135170.
At line:1 char:1
+ c:\ps-test\Start-ActivityTracker.ps1
+ ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : SecurityError: (:) [], PSSecurityException
    + FullyQualifiedErrorId : UnauthorizedAccess

The third command uses the Unblock-File cmdlet to unblock the script so it can run in the session.
PS C:\>Get-Item C:\ps-test\Start-ActivityTracker.ps1 | Unblock-File
```

Xxxx xxxxxxx xxxxx xxx xx xxxx xxx xxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx.

## XXXXXXXXXX

### -InformationAction
$$Xxxx$$

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa
Accepted values: SilentlyContinue, Stop, Continue, Inquire, Ignore, Suspend

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
$$Xxxx$$

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LiteralPath
Xxxxxxxxx xxx xxxxx xx xxxxxxx.
Xxxxxx Xxxx$ xxx xxxxx xx xxx XxxxxxxXxxx xxxxxxxxx xx xxxx xxxxxxx xx xx xx xxxxx.
Xx xxxxxxxxxx xxx xxxxxxxxxxx xx xxxxxxxxx.
Xx xxx xxxx xxxxxxxx xxxxxx xxxxxxxxxx$ xxxxxxx xx xx xxxxxx xxxxxxxxx xxxxx.
Xxxxxx xxxxxxxxx xxxxx xxxx Xxxxxxx XxxxxXxxxx xxx xx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: ByLiteralPath
Aliases: PSPath

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
Xxxxxxxxx xxx xxxxx xx xxxxxxx.
Xxxxxxxx xxxxxxxxxx xxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: ByPath
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Xxxxxxx xxx xxx xxxxxxxxxxxx xxxxxx xxxxxxx xxx xxxxxx.Xxxxxxx xxx xxx xxxxxxxxxxxx xxxxxx xxxxxxx xxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Xxxxx xxxx xxxxx xxxxxx xx xxx xxxxxx xxxx.
Xxx xxxxxx xx xxx xxx.Xxxxx xxxx xxxxx xxxxxx xx xxx xxxxxx xxxx.
Xxx xxxxxx xx xxx xxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.String
Xxx xxx xxxx x xxxx xxxx xx Xxxxxxx$Xxxx.

## XXXXXXX

### None
Xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xxx Xxxxxxx$Xxxx xxxxxx xxxxx xxxx xx xxxx xxxxxx xxxxxx.

Xxxxxxx$Xxxx xxxxxxxx xxx xxxx xxxxxxxxx xx xxx Xxxxxxx xxxxxx xx xxx Xxxxxxxxxx xxxxxx xxx xx Xxxx Xxxxxxxx.

Xx xxx xxx xxx Xxxxxxx$Xxxx xxxxxx xx x xxxx xxxx xx xxx xxxxxxx$ xxx xxxxxxx xxx xx xxxxxx xx xxx xxxxxxxxx xxxx xxx xxx xxxxxx xxxx xxx xxxxxxxx xxxxxx.

## XXXXXXX XXXXX

[about_Execution_Policies]()

[Get-Item]()

[FileSystem Provider]()

