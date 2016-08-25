---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294005
schema: 2.0.0
---

# Remove-TypeData
## XXXXXXXX
Xxxxxxx xxxxxxxx xxxxx xxxx xxx xxxxxxx xxxxxxx

## XXXXXX

### RemoveTypeDataSet (Default)
```
Remove-TypeData -TypeData <TypeData> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

### RemoveTypeSet
```
Remove-TypeData [-TypeName] <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

### RemoveFileSet
```
Remove-TypeData -Path <String[]> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XxxxXxxx xxxxxx xxxxxxx xxxxxxxx xxxx xxxx xxxx xxx xxxxxxx xxxxxxx.
Xxxx xxxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxx xxx xxxxxxxx xxxx xxx xxxxxxx xx xxx xxxxxxx xxxxxxx.

Xxx xxx xxx xxxxxxxxxx xxx xxxxxxx xx xxxxxxx xx Xxxxxxx XxxxxXxxxx xx xxxxxxxx xxxx xx Xxxxxx$XxxxXxxx xxxxxxxx xxx  Xxxxx.xx0xxx xxxxx.
Xxxxxx$XxxxXxxx xxxxxxx xxxxx xxxxxxxx xxxxxxxxxx xxx xxxxxxx xxxx xxx xxxxxxx xxxxxxx.
Xxxxxx$XxxxXxxx xxxx xxx xxxxxx xxx Xxxxx.xx0xxx xxxxx xx xxxxxx xxx xxxxxxxx xxxx xxxxxxxxxxx xxxx xxx Xxxxx.xx0xxx xxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx Xxxxx.xx0xxx xxxxx$ xxx xxxxx$Xxxxx.xx0xxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

Xxxx xxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

## XXXXXXXX

### Xxxxxxx 0
```
PS C:\>Remove-TypeData -TypeName System.Array
```

Xxxx xxxxxxx xxxxxxx xxxx xxx xxxxxxx xxx xxxx xxxx xxx xxx Xxxxxx.Xxxxx xxxx$ xxxxxxxxx xxxx xxxx xxxx xxx xxxxx xx x Xxxxx.xx0xxx xxxx xxx xxxxxxx xxxx xxxx xxxx xxx xxxxx xx xxx xxxxxxx xx xxxxx xxx Xxxxxx$XxxxXxxx xxxxxx.

### Xxxxxxx 0
```
The first command uses the Get-TypeData cmdlet to get extended type data for the System.DateTime type.The output shows that a DateTime property has been added to all System.DateTime objects in Windows PowerShell.
PS C:\>Get-TypeData System.DateTime
TypeName        Members
--------        -------
System.DateTime {[DateTime, System.Management.Automation.Runspaces.ScriptPropertyData]}

The second command uses the Get-Date cmdlet, which returns a System.DateTime object. The command uses dot notation to get the value of the DateTime property of the System.DateTime object that Get-Date returns.
PS C:\>(Get-Date).DateTime
Friday, January 20, 2012 9:01:00 PM

The third command uses the Get-TypeData cmdlet to get all extended type data for the System.DateTime type and the Remove-TypeData cmdlet to delete the extended type data.
PS C:\>Get-TypeData System.DateTime | Remove-TypeData

The fourth command shows the effect of deleting the extended type data for the System.DateTime type. The command repeats the second command. However, because the System.DateTime property no longer exists, a command to get its value returns nothing.
PS C:\>(Get-Date).DateTime
PS C:\>
```

Xxxx xxxxxxx xxxxx xxx xxxxxx xx xxxxxxxx xxxxxxxx xxxx xxxx xxxx x xxxxxxx.

### Xxxxxxx 0
```
PS C:\>Get-Module | Remove-TypeData
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxxxx xxxx xxxx xxx xxxxxx xxxxxxx.
Xxxx xxx xxxx xx xxxxxx xx Xxxxxx$XxxxXxxx$ Xxxxxx$XxxxXxxx xxxx xxx xxxx xx xxx xxxxxx xxxx xxx xxxxxxx xxx xxxx xxxx xxx xxx xxxxxxx xx xxxx xxxx.

### Xxxxxxx 0
```
PS C:\>Remove-TypeData -Path C:\WINDOWS\System32\WindowsPowerShell\v1.0\Modules\PSScheduledJob, C:\WINDOWS\System32\WindowsPowerShell\v1.0\Modules\PSWorkflow\PSWorkflow.types.ps1xml
```

Xxxx xxxxxxx xxxx xxx Xxxx xxxxxxxxx xx xxx Xxxxxx$XxxxXxxx xxxxxx xx xxxxxx xxx xxxxxxxx xxxxx xxxx xxx xxxxxxx xx xxx Xxxxx.xx0xxx xxxxx xxxx xxx xxxxx xx xxx XXXxxxxxxxxXxx xxx XXXxxxxxxx xxxxxxx.
Xxxx xxxxxxx xxxx xxx xxxxxx xxxxxxx xxxx xxxx xxxx xx xxxxx xx xxxxx xxx Xxxxxx$XxxxXxxx xxxxxx.
Xxx xxxxxxx xxxxxxxx xxxx xxxx xxx xxxxxxx xxxx xxxx xxxxxxxx xxxx xxx xxxxxxx xxxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxxxxxx$ xxx xxxxx$Xxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

### Xxxxxxx 0
```
PS C:\>Invoke-Command -Session $s {Get-TypeData -TypeName *CIM* | Remove-TypeData}
```

Xxxx xxxxxxx xxxxxxx xxxxxxxx xxxxx xxxx x xxxxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx Xxxxxx$Xxxxxxx xxxxxx xx xxxxxx xxxxxxxx xxxx xxxx xxx xxx XXX xxxxx xx xxx xxxxxxxx xx xxx $x xxxxxxxx.

## XXXXXXXXXX

### -InformationAction
Xxxxx xxx xxxxx xxx xxxx xxxxx xx xxx xx xxxx Xxxxx.xx0xxx xxxxx.
Xxxxxxxxx xxx xxx xxxxxxxxx.
Xx xxx xxxx xxx xxxx$ xxx xxxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxxxx.

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
Xxxxx xxx xxxxx xxx xxxx xxxxx xx xxx xx xxxx Xxxxx.xx0xxx xxxxx.
Xxxxxxxxx xxx xxx xxxxxxxxx.
Xx xxx xxxx xxx xxxx$ xxx xxxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxxxx.

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

### -Path
Xxxxxxx xxxx xxx xxxxxxx xxxxxxxx xxxx xxxx xxxx xx xxxxxxx xx xxx xxxxxxxxx xxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx.

Xxxxx xxx xxxxx xxx xxxx xxxxx xx xxx xx xxxx Xxxxx.xx0xxx xxxxx.
Xxxxxxxxx xxx xxx xxxxxxxxx.
Xx xxx xxxx xxx xxxx$ xxx xxxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: RemoveFileSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TypeData
Xxxxxx xxx xxxxxxxxx xxxx xxxx xxxx xxx xxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx XxxxXxxx xxxxxxx $Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.Xxxxxxxxx.XxxxXxxx$ xx x xxxxxxx xxxx xxxx XxxxXxxx xxxxxxx$ xxxx xx x Xxx$XxxxXxxx xxxxxxx.
Xxx xxx xxxx xxxx XxxxXxxx xxxxxxx xx Xxxxxx$XxxxXxxx.

```yaml
Type: TypeData
Parameter Sets: RemoveTypeDataSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -TypeName
Xxxxxxx xxx xxxxxxxx xxxx xxxx xxx xxx xxxxxxxxx xxxxx.
Xxx xxxxx xx xxx Xxxxxx xxxxxxxxx$ xxxxx xxx xxxxx xxxx.
Xxxxxxxxx$ xxx xxxx xxxx xxxx xx xxxxxxxx.
Xxxxxxxxx xxx xxx xxxxxxxxx.

Xxx xxx xxxx xxxx xxxxx xx Xxxxxx$XxxxXxxx.
Xxxx xxx xxxx xx xxxxxx xx Xxxxxx$XxxxXxxx$ Xxxxxx$XxxxXxxx xxxx xxx xxxx xxxx xx xxx xxxxxx xxx xxxxxxx xxx xxxx xxxx xxx xxx xxxxxx xxxx.

```yaml
Type: String
Parameter Sets: RemoveTypeSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
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

### System.Management.Automation.Runspaces.TypeData
Xxx xxx xxxx XxxxXxxx xxxxxx$ xxxx xx xxx xxxx xxxx xxx Xxx$XxxxXxxx xxxxxx xxxxxxx$ xx Xxxxxx$XxxxXxxx.

### System.String
Xxx xxx xxxx xxx xxxx xxxxx xx Xxxxxx$XxxxXxxx.
Xxxx xxx xxxx xx xxxxxx xx Xxxxxx$XxxxXxxx$ Xxxxxx$XxxxXxxx xxxx xxx xxxx xxxx xx xxx xxxxxx xxx xxxxxxx xxx xxxx xxxx xxx xxx xxxxxx xxxx.

## XXXXXXX

### None
Xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xxxxxx$XxxxXxxx xxx xxxxxx xxxx xxx xxxxxxxx xxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxxxxx xxxxxx xxxxxxxx xxxx xxxx xxxx xx xx xxx xxxxxxxx$ xxx xxx xxx xxxx xxxxx xx xxx xxxxxxx xxxxxxx$ xxxx xx xxxxxxxx xxxxx xxxx xxx xxxxxxx xx xxxxxxx xxxx xxxx xxx xxxx xxxxxxxx xxxx xxx xxxxxxx xxxxxxx.

## XXXXXXX XXXXX

[Get-TypeData]()

[Update-TypeData]()

[about_Types.ps1xml]()

