---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294025
schema: 2.0.0
---

# Xxxxxx$XxxxXxxx
## XXXXXXXX
Xxxxxxx xxx xxxxxxxx xxxx xxxx xx xxx xxxxxxx.

## XXXXXX

### XxxxXxx $Xxxxxxx$
```
Update-TypeData [[-AppendPath] <String[]>] [-PrependPath <String[]>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### XxxxxxxXxxxXxx
```
Update-TypeData [-MemberType <PSMemberTypes>] [-MemberName <String>] [-Value <Object>] [-SecondValue <Object>]
 [-TypeConverter <Type>] [-TypeAdapter <Type>] [-SerializationMethod <String>]
 [-TargetTypeForDeserialization <Type>] [-SerializationDepth <Int32>] [-DefaultDisplayProperty <String>]
 [-InheritPropertySerializationSet <Boolean>] [-StringSerializationSource <String>]
 [-DefaultDisplayPropertySet <String[]>] [-DefaultKeyPropertySet <String[]>]
 [-PropertySerializationSet <String[]>] -TypeName <String> [-Force] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### XxxxXxxxXxx
```
Update-TypeData [-Force] [-TypeData] <TypeData[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XxxxXxxx xxxxxx xxxxxxx xxx xxxxxxxx xxxx xxxx xx xxx xxxxxxx xx xxxxxxxxx xxx Xxxxx.xx0xxx xxxxx xxxx xxxxxx xxx xxxxxx xxx xxxxxxxx xxxx xxxx.

Xx xxxxxxx$ Xxxxxxx XxxxxXxxxx xxxxx xxxxxxxx xxxx xxxx xx xx xx xxxxxx.
Xxxxxxx xxxxxxxxxx$ Xxxxxx$XxxxXxxx xxxxxxx xxx xx xxx Xxxxx.xx0xxx xxxxx xxxx xx xxx xxxxxx xx xxx xxxxxxx$ xxxxxxxxx xxx xxxx xxxxx xxxx xxx xxxxx.
Xxx xxx xxx xxx xxxxxxxxxx xx Xxxxxx$XxxxXxxx xx xxx xxx xxxx xxxxx xxx xxx xxx xxxxxxx xxxxxxxx xxxx xxxx.

Xxx Xxxxxx$XxxxXxxx xxxxxx xxx xx xxxx xx xxxxxxx xxx xxxx xxxx.
Xxxx xxxxxxx xx xxxxxxxxxxxx xxxxxx xxxx xxx xxx xxxxxxxxxx xxxxx xxx xxxx xx xxxx xxxxx xxx xxxxx xxx xxxxxxx xxxxxxxx.

Xxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ xxx xxx xxx Xxxxxx$XxxxXxxx xx xxx xxx xxxxxxx xxxxxxxx xxxx xxxx xx xxx xxxxxxx xxxxxxx xxxxx x Xxxxx.xx0xxx xxxx.
Xxxx xxxx xxxx xx xxxxx xxxxxxxxxxx$ xxxx xx$ xxxxxxx x xxxx$ xx xxxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxx xxx xxxx xxxx xx xxx xxxxxxxx$ xxx xx Xxxxxx$XxxxXxxx xxxxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

Xxxx$ xxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ xxx xxx xxx xxx Xxx$XxxxXxxx xxxxxx xx xxx xxx xxxxxxxx xxxxx xx xxx xxxxxxx xxxxxxx xxx xxx Xxxxxx$XxxxXxxx xxxxxx xx xxxxxx xxxxxxxx xxxxx xxxx xxx xxxxxxx xxxxxxx.

Xxxxxxxxxx xxxx xxxxx xx xxxxxxxxxx$ xx xxxx xxxxxx xxxxxxxxxx xx xx Xxxxxx$XxxxXxxx xxxxxxx$ xx xxx xxxxxx xxxxxx xx XxxXxx.
Xxxx xx xx xxxxxxxx xxxxxxxxxx xxxx xxxxx xxxxx xx xxxx xxxxxx xxxxx xxxxxx xxxxxxxxxx xxx xxxxxxxxxx.
Xx xxx xxx xxxxxxx .XXX Xxxxxxxxx xxxxxxxxxx$ xxx xxx xxxx xxxxxx xxx xxxxxxxxxxx xx xxxxxxxxxx xx xxxxx xxxxxx xxxxxx xxxxxxx$ xx xxxxx xx xxx xxxxxxxxx xxxxxxx$

$xxxxx$.xxx$Xxxxxx$$

Xxxx xxxx xxxxxx xxxxxx xxx xxxx xx xxxx xxxx .XXX Xxxxxxxxx xxxxxxxxxx.
Xxxxxxxxxx xxxx xxx xxxxx xx xxxxxxx xxx Xxxxxx$XxxxXxxx xxxxxx xxxxxx xxx xxxxxx xxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxx $xxxxx.xx0xxx xxxxx xx Xxxxxxx XxxxxXxxxx$ xxx xxxxx$Xxxxx.xx0xxx $xxxx$$$xxxxxxx.xxxxxxxxx.xxx$xxxxxxx$xx000000.xxxx$.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Update-Typedata
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxxxx xxxx xxxxxxxxxxxxx xxxx xxx $.xxxxx.xx0xxx xxxxx xxxx xxxx xxxxxxx xxxx xxxx xx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command updates the extended type configuration from the *.types.ps1xml files, processing the TypesA.types.ps1xml and TypesB.types.ps1xml files first.
PS C:\>Update-Typedata -PrependPath TypesA.types.ps1xml, TypesB.types.ps1xml

The second command shows how to update the TypesA.types.ps1xml again, such as you might do if you added or changed a type in the file. You can either repeat the previous command for the TypesA.types.ps1xml file, or run an Update-Typedata command without parameters, because TypesA.types.ps1xml is already in the type file list for the current session.
PS C:\>Update-Typedata -PrependPath TypesA.types.ps1xml

-or-

Update-Typedata
```

Xxxx xxxxxxx xxxx xxx xx xxxxxx xxx xxxxx xx x xxxx xxxx xxxxxxxx xxxxx xx xxx xxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Update-TypeData -TypeName System.DateTime -MemberType ScriptProperty -MemberName Quarter -Value {if ($this.Month -in @(1,2,3)) {"Q1"} elseif ($this.Month -in @(4,5,6)) {"Q2"} elseif ($this.Month -in @(7,8,9)) {"Q3"} else {"Q4"} }
PS C:\>(Get-Date).QuarterQ1
```

Xxxx xxxxxxx xxxx Xxxxxx$XxxxXxxx xx xxx xxx Xxxxxxx xxxxxx xxxxxxxx xx Xxxxxx.XxxxXxxx xxxxxxx xx xxx xxxxxxx xxxxxxx$ xxxx xx xxxxx xxxxxxxx xx xxx Xxx$Xxxx xxxxxx.

Xxx Xxxxxx$XxxxXxxx xxxxxxx xxxx xxx XxxxXxxx xxxxxxxxx xx xxxxxxx xxx Xxxxxx.XxxxXxxx xxxx$ xxx XxxxxxXxxx xxxxxxxxx xx xxxxxxx x xxxx xxx xxx xxx xxxxxxxx$ xxx XxxxxxXxxx xxxxxxxx xx xxxxxxx xxx XxxxxxXxxxxxxx xxxx$ xxx xxx Xxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx xxxxxxx.

Xxx xxxxx xx xxx Xxxxx xxxxxxxx xx x xxxxxx xxxx xxxxxxxxxx xxx xxxxxxx xxxxxx xxxxxxx.
Xxx xxxxxx xxxxx xxx $xxxx xxxxxxxxx xxxxxxxx xx xxxxxxxxx xxx xxxxxxx xxxxxxxx xx xxx xxxxxx xxx xxx Xx xxxxxxxx xx xxxxxxxxx xxxxxxx xxx xxxxx xxxxx xxxxxxx xx xxxx xxxxxxx xxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxx Xx xxxxxxxx$ xxx xxxxx$Xxxxxxxxxx$Xxxxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

Xxx xxxxxx xxxxxxx xxxx xxx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Update-TypeData -TypeName System.DateTime -DefaultDisplayPropertySet DateTime, DayOfYear, Quarter
PS C:\>Get-Date | Format-List

Thursday, March 15, 2012 12:00:00 AM
DayOfYear : 75
Quarter   : Q1
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx xxxxxxxxxx xx x xxxx xxxx xxxxxxx xx xxxxx xx xxxxxxx$ xxxx xx$ xxxx xx xxxxxxxxxx xxx xxxxxxxxx.
Xxxxxxx xxx xxxx xxxx xx xxx xxxxxxxxx xx x Xxxxx.xx0xxx xxxx$ xx xx xxxxxxxxx xxxx xx xxx xxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxx$XxxxXxxx xxxxxx xx xxx xxx xxxxxxx xxxx xxxxxxxxxx xxx xxx Xxxxxx.XxxxXxxx xxxx.
Xxx xxxxxxx xxxx xxx XxxxXxxx xxxxxxxxx xx xxxxxxx xxx xxxx xxx xxx XxxxxxxXxxxxxxXxxxxxxxXxx xxxxxxxxx xx xxxxxxx xxx xxxxxxx xxxxxxxxxx xxx x xxxx.
Xxx xxxxxxxx xxxxxxxxxx xxxxxxx xxx xxx Xxxxxxx xxxxxx xxxxxxxx xxxx xxx xxxxx xx x xxxxxxxx xxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx x Xxxxxx.XxxxXxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxx xxxx.
Xxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx XxxxXxxx xxxxxx xx xxx Xxxxxx$Xxxx xxxxxx.
Xxxxxxx xxx Xxxxxx$Xxxx xxxxxxx xxxx xxx xxxxxxx xxx xxxxxxxxxx xx xxxxxxx xx xxx xxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxxxx xxxxxx xxxx xxxx xxxxxxxxxxx xx xxx Xxxxxx$XxxxXxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Module | Update-TypeData -MemberType ScriptProperty -MemberName SupportsUpdatableHelp -Value {if ($this.HelpInfoUri) {$True} else {$False}}
Get-Module -ListAvailable | Format-Table Name, SupportsUpdatableHelp

Name                             SupportsUpdatableHelp
----                             ---------------------
Microsoft.PowerShell.Diagnostics                  True
Microsoft.PowerShell.Host                         True
Microsoft.PowerShell.Management                   True
Microsoft.PowerShell.Security                     True
Microsoft.PowerShell.Utility                      True
Microsoft.WSMan.Management                        True
PSDiagnostics                                    False
PSScheduledJob                                    True
PSWorkflow                                        True
ServerManager                                     True
TroubleshootingPack                              False
```

Xxxx xxxxxxx xxxxxxxxxxxx xxxx xxxx xxx xxxx xx xxxxxx xx Xxxxxx$XxxxXxxx$ Xxxxxx$XxxxXxxx xxxx xxxxxxxx xxxx xxxx xxx xxx xxxxxx xxxx.

Xxxx xxxxxxxxx xx xxxxxxx xxxx xxxxx xxx Xxx$Xxxxxx xxxxxx xx xxx Xxx$Xxxx xxxxxx xx xxx xxx xxxxxx xxxx.
Xxxxxxx$ xx xxx xxxx x xxxxxxxxxx xx xxxxxxx xx Xxxxxx$XxxxXxxx$ xx xxxxxxx xxx xxxx xxxx xx xxx xxxxx xxxxxx xxxx xxx xxxx xxxxxxx xx xxxxx xxx xxx xxxxx xxxxxxx xx xxx xxxxxxxxxx xxxxxxx xxx xxxxxx xx xxxxxxx xxxxxxx xx xxx xxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxx xxx XXXxxxxxxxxXxx xxxxxx.
Xxx xxxxxxx xxxxx xxx xxxxxx xxxxxx xx xxx Xxxxxx$XxxxXxxx xxxxxx$ xxxxx xxxxxxx xxx xxxx xxxx xxx xxx Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxxXxxx xxxx xxx xxx xxxxx xxxxxxx xxxx xx$ xxxx xx xxx XxxxxxXxxxXxxxxxxx xxxx xxxx Xxx$Xxxxxx xxxxxxx xxxx xxx xxx xxx XxxxXxxxxxxxx xxxxxxxxx xx xxx xxxxxxx.

Xxx Xxxxxx$XxxxXxxx xxxxxxxx xxxx xxx XxxxxxxxXxxxxxxxxXxxx xxxxxx xxxxxxxx xx xxx xxxxxxxx xxxxxxx.
Xxx xxxxx xx xxx Xxxxx xxxxxxxxx xx x xxxxxx xxxx xxxxxxx $Xxxx xx xxx XxxxXxxxXxx xxxxxxxx xx xxx xxxxxx xx xxxxxxxxx xxx $Xxxxx xxxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxx xxx xxxxxx xxxxxxx xxxx Xxx$Xxxxxx xx xxx Xxxxxx$Xxxxx xxxxxx$ xxxxx xxxxxxxx xxx Xxxx xxx XxxxxxxxXxxxxxxxxXxxx xxxxxxxxxx xx xxx xxxxxxx xx x xxxx.

## XXXXXXXXXX

### $XxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxxxxxxx .xx0xxx xxxxx.
Xxx xxxxxxxxx xxxxx xxx xxxxxx xx xxx xxxxx xxxx xxxx xxx xxxxxx xxxxx xxx xxxxx$xx xxxxx xxx xxxxxx.
Xxx xxx xxxx xxxx xx XxxxxxXxxx xxxxx xx Xxxxxx$XxxxXxxx.

```yaml
Type: String[]
Parameter Sets: FileSet
Aliases: PSPath, Path

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### $XxxxxxxxxxxXxxxxx
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

### $XxxxxxxxxxxXxxxxxxx
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

### $XxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx .xx0xxx xxxxx.
Xxx xxxxxxxxx xxxxx xxx xxxxxx xx xxx xxxxx xxxx xxxx xxx xxxxxx xxxxxx xxx xxxxx$xx xxxxx xxx xxxxxx.

```yaml
Type: String[]
Parameter Sets: FileSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxxxxxXxxxxxxx
Xxxxxxxxx xxx xxxxxxxx xx xxx xxxx xxxx xx xxxxxxxxx xx xxx Xxxxxx$Xxxx xxxxxx xxxx xx xxxxx xxxxxxxxxx xxx xxxxxxxxx.

Xxxx xxx xxxx xx x xxxxxxxx xx xxxxxxxx xxxxxxxx xx xxx xxxx.
Xxx xxxxx xx xxxx xxxxxxxxx xxx xx xxx xxxx xx x xxxx xxxx xx xxxxx xx xxx xxxx xxxxxxx.

Xxxx xxxxx xx xxxxxxxxx xxxx xxxx xxxxx xxx xx xxxx xxxxx xxxxxxx xxx xxx xxxx xx x Xxxxxx.xx0xxx xxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: String
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxxxxxXxxxxxxxXxx
Xxxxxxxxx xxx xx xxxx xxxxxxxxxx xx xxx xxxx.
Xxxxx xxxxxxxxxx xxx xxxxxxxxx xx xxx Xxxxxx$Xxxx xxxxxx xxxx xx xxxxx xxxxxxxxxx xxx xxxxxxxxx.

Xxxx xxx xxxxx xx xxxxxxxx xx xxxxxxxx xxxxxxxxxx xx xxx xxxx.
Xxx xxxxx xx xxxx xxxxxxxxx xxx xx xxx xxxxx xx xxxxx xxxx xxx xxxxx xx xxx xxxx xxxxxxx.

Xxxx xxxxx xx xxxxxxxxx xxxx xxxx xxxxx xxx xx xxxx xxxxx xxxxxxx xxx xxx xxxx xx x Xxxxxx.xx0xxx xxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: String[]
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxXxxxxxxxXxx
Xxxxxxxxx xxx xx xxxx xxxxxxxxxx xx xxx xxxx.
Xxxxx xxxxxxxxxx xxx xxxx xx xxx Xxxxx$Xxxxxx xxx Xxxx$Xxxxxx xxxxxxx xxxx xx xxxxx xxxxxxxxxx xxx xxxxxxxxx.

Xxxx xxx xxxxx xx xxxxxxxx xx xxxxxxxx xxxxxxxxxx xx xxx xxxx.
Xxx xxxxx xx xxxx xxxxxxxxx xxx xx xxx xxxxx xx xxxxx xxxx xxx xxxxx xx xxx xxxx xxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: String[]
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxx
Xxxx xxx xxxxxxxxx xxxx xxxx$ xxxx xx xxxx xxxx xxx xxxxxxx xxxx xxxxxxxxx xxx xxxx xxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: SwitchParameter
Parameter Sets: DynamicTypeSet, TypeDataSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxxxxxxXxxxxxxxxxxxxXxx
Xxxxxxxxxx xxxxxxx xxx xxx xx xxxxxxxxxx xxxx xxx xxxxxxxxxx xx xxxxxxxxx.
Xxx xxxxxxx xxxxx xx $Xxxx

Xxxxx xxxxxx xxx$

$$ $Xxxx$ Xxx xxxxxxxx xxx xx xxxxxxxxx.
                         
$$ $Xxxxx$ Xxx xxxxxxxx xxx xx xxx xxxxxxxxx.
                         
$$ $Xxxx$ Xxxxxxxxxxx xx xxx xxxxxxx.

Xxxx xxxxxxxxx xx xxxxx xxxx xxxx xxx xxxxx xx xxx XxxxxxxxxxxxxXxxxxx xxxxxxxxx xx XxxxxxxxXxxxxxxxxx.
Xxxx xxx xxxxx xx xxxx xxxxxxxxx xx $Xxxxx$ xxx XxxxxxxxXxxxxxxxxxxxxXxx xxxxxxxxx xx xxxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: Boolean
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxx
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xx xxxxxx.

Xxx xxxx xxxxxxxxx xxxx xxx XxxxXxxx$ XxxxxxXxxx$ Xxxxx xxx XxxxxxXxxxx xxxxxxxxxx xx xxx xx xxxxxx x xxxxxxxx xx xxxxxx xx x xxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: String
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xx xxx xx xxxxxx.

Xxx xxxx xxxxxxxxx xxxx xxx XxxxXxxx$ XxxxxxXxxx$ Xxxxx xxx XxxxxxXxxxx xxxxxxxxxx xx xxx xx xxxxxx x xxxxxxxx xx xxxxxx xx x xxxx.

Xxx xxxxx xxxxxx xxx xxxx xxxxxxxxx xxx$ XxxxxXxxxxxxx$ XxxxXxxxxx$ XxxxXxxxxxxx$ Xxxxxxxxxxxx$ XxxxxxXxxxxx$ xxx XxxxxxXxxxxxxx.

Xxx xxxxxxxxxxx xxxxx xxxxx xxxxxx$ xxx $XXXxxxxxXxxxx Xxxxxxxxxxx$ xx XXXX xx xxxx$$$xxxx.xxxxxxxxx.xxx$xx$xx$xxxxxxx$xxxxxxx$xxxxxxx$xxxxxx.xxxxxxxxxx.xxxxxxxxxx.xxxxxxxxxxxxx$x$xx.00$.xxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: PSMemberTypes
Parameter Sets: DynamicTypeSet
Aliases: 
Accepted values: AliasProperty, CodeProperty, Property, NoteProperty, ScriptProperty, Properties, PropertySet, Method, CodeMethod, ScriptMethod, Methods, ParameterizedProperty, MemberSet, Event, Dynamic, All

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxXxxxxxxxxxxxxXxx
Xxxxxxxxx xxx xxxxx xx xxxxxxxxxx xxxx xxx xxxxxxxxxx.
Xxx xxxx xxxxxxxxx xxxx xxx xxxxx xx xxx XxxxxxxxxxxxxXxxxxx xxxxxxxxx xx XxxxxxxxXxxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxxx
Xxxxxxxxx xxxxxxxxxx xxxxxx xxx XxxxxXxxxxxxx$ XxxxxxXxxxxxxx$ XxxxXxxxxxxx$ xx XxxxXxxxxx xxxxxxx.

Xxx xxxx xxxxxxxxx xxxx xxx XxxxXxxx$ XxxxxxXxxx$ Xxxxx xxx XxxxxxXxxxx xxxxxxxxxx xx xxx xx xxxxxx x xxxxxxxx xx xxxxxx xx x xxxx.

Xxxx xxx xxxxx xx xxx XxxxxxXxxx xxxxxxxxx xx XxxxxXxxxxxxx$ xxx xxxxx xx xxx XxxxxxXxxxx xxxxxxxxx xxxx xx x xxxx xxxx.
Xxxxxxx XxxxxXxxxx xxxxxxxx $$xxxxx$$ xxx xxxxx xx xxx xxxxx xxxxxxxx xx xxx xxxxxxxxx xxxx.
Xxx xxxxxxx$ xx xxx xxx xx xxxxx xxxxxxxx xxxx xxxxxxxx xx xxxxxxxxx xxxx xxx x xxxxxx xxxxxxxx$ xxx xxx xxxx xxxxxxx x XxxxxxXxxxx xx Xxxxxx.Xxx00 xx xxxxxxx xxx xxxxxxx xxxxxx xxxxx xx xx xxxxxxx.

Xxxx xxx xxxxx xx xxx XxxxxxXxxx xxxxxxxxx xx XxxxxxXxxxxxxx$ xxx xxx xxx xxx XxxxxxXxxxx xxxxxxxxx xx xxxxxxx xx xxxxxxxxxx xxxxxx xxxxx.
Xxx xxxxxx xxxxx xx xxx xxxxx xx xxx Xxxxx xxxxxxxxx xxxx xxx xxxxx xx x xxxxxxxx.
Xxx xxxxxx xxxxx xx xxx xxxxx xx xxx XxxxxxXxxxx xxxxxxxxx xxx xxx xxxxx xx xxx xxxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: Object
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxxxxxXxxxx
Xxxxxxxxx xxx xxxx xxxxxx xx xxxx xxxxxxx xxx xxxxxxxxxx xx xxxxxxx.
Xxx xxxxxxx xxxxx$ 0$ xxxxxxxxxx xxx xxxxxx xxx xxx xxxxxxxxxx.
X xxxxx xx 0 xxxxxxxxxx xxx xxxxxx$ xxx xxx xxx xxxxxxxxxx.
X xxxxx xx 0 xxxxxxxxxx xxx xxxxxx$ xxx xxxxxxxxxx$ xxx xxx xxxxxxx xx xxxxxxxx xxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: Int32
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxxxxxXxxxxx
Xxxxxxxxx x xxxxxxxxxxxxx xxxxxx xxx xxx xxxx.
X xxxxxxxxxxxxx xxxxxx xxxxxxxxxx xxxxx xxxxxxxxxx xx xxx xxxx xxx xxxxxxxxxx xxx xxx xxxxxxxxx xxxx xx xxxx xx xxxxxxxxx xxxx.

Xxxxx xxxxxx xxx$

$$ XxxXxxxxxXxxxxxxxxx$ Xxxxxxxxx xxx xxxxxx xxxxxxxxxx xx xxx xxxx. Xxx xxx xxx xxx XxxxxxxxxxxxxXxxxx xxxxxxxxx xx xxxxxxxxx xxxxxxx xxxxx xxxxxxxxxx xxx xxxxxxxxxx.
$$ Xxxxxx$ Xxxxxxxxx xxx xxxx xx x xxxxxx. Xxx xxx xxx xxx XxxxxxXxxxxxxxxxxxxXxxxxx xx xxxxxxx x xxxxxxxx xx xxx xxxx xx xxx xx xxx xxxxxxxxxxxxx xxxxxx. Xxxxxxxxx$ xxx xxxx xx xxxxxxxxxx xx xxxxx xxx XxXxxxxx xxxxxx xx xxx xxxxxx.
$$ XxxxxxxxXxxxxxxxxx Xxxxxxxxx xxxx xxx xxxxxxxxx xxxxxxxxxx xx xxxx xxxx. Xxx xxx XxxxxxxxXxxxxxxxxxxxxXxx xxxxxxxxx xx xxxxxxx xxx xxxxxxxxxx xx xxx xxxx xxxx xxx xxxxxxxxxx. Xxx xxx xxxx xxx xxx XxxxxxxXxxxxxxxXxxxxxxxxxxxxXxx xxxxxxxxx xx xxxxxxxxx xxxxxxx xxx xxxxxxxx xxx xx xxxxxxxxx xxx xxx XxxxxxxxxxxxxXxxxx xxxxxxxxx xx xxxxxxxxx xxxxxxx xxxxx xxxxxxxxxx xxx xxxxxxxxxx.

Xx Xxxxxxx XxxxxXxxxx$ xxxxxxxxxxxxx xxxxxxx xxx xxxxxx xx XXXxxxxxxxXxxxxxx xxxxxxxx xxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: String
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxxxxxxxxxxxXxxxxx
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xx xxx xxxx.
Xxx xxxxx xx xxxxxxxxx xxxxxxxx xx xxxx xx xxx xxxxxxxxxxxxx xxxxxx.
Xxxx xxxxxxxxx xx xxxxx xxxx xxxx xxx xxxxx xx xxx XxxxxxxxxxxxxXxxxxx xxxxxxxxx xx Xxxxxx.

```yaml
Type: String
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxxXxxXxxxxxxxxxxxxxx
Xxxxxxxxx xxx xxxx xx xxxxx xxxxxx xx xxxx xxxx xxx xxxxxxxxx xxxx xxxx xxx xxxxxxxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: Type
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxxxxx
Xxxxxxxxx xxx xxxx xx x xxxx xxxxxxx$ xxxx xx Xxxxxxxxx.XxxxxXxxxx.Xxx.XxxXxxxxxxxXxxxxxx.
X xxxx xxxxxxx xxxxxxx Xxxxxxx XxxxxXxxxx xx xxx xxx xxxxxxx xx x xxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: Type
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxxxxxxx
Xxxxxxxxx x xxxx xxxxxxxxx xx xxxxxxx xxxxxx xxxxxxx xxxxxxxxx xxxxx.
Xx x xxxx xxxxxxxxx xx xxxxxxx xxx x xxxx$ xx xxxxxxxx xx xxx xxxx xxxxxxxxx xx xxxx xxx xxx xxxxxxxxxx.

Xxxxx x Xxxxxx.Xxxx xxxxx xxxx xx xxxxxxx xxxx xxx Xxxxxx.XxxxxxxxxXxxxx.XxxxXxxxxxxxx xx Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxXxxxxxxxx xxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: Type
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxx xxx xxxxxxxxx xxxx xxxx xx xxx xxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx x XxxxXxxx xxxxxx xx x xxxxxxx xxxx xxxx x XxxxXxxx xxxxxx$ xxxx xx x Xxx$XxxxXxxx xxxxxxx.
Xxx xxx xxxx xxxx x XxxxXxxx xxxxxx xx Xxxxxx$XxxxXxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: TypeData[]
Parameter Sets: TypeDataSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxx xx xxxxxx.

Xxx xxxxx xx xxx Xxxxxx xxxxxxxxx$ xxxxx xxx xxxxx xxxx.
Xxxxxxxxx$ xxx xxxx xxxx xxxx xx xxxxxxxx.
Xxxxxxxxx xxx xxx xxxxxxxxx.

Xxx xxx xxxx xxxx xxxxx xx Xxxxxx$XxxxXxxx.
Xxxx xxx xxxx xx xxxxxx xx Xxxxxx$XxxxXxxx$ Xxxxxx$XxxxXxxx xxxx xxx xxxx xxxx xx xxx xxxxxx xxx xxxx xxxx xx xxx xxxxxx xxxx.

Xxx xxxx xxxxxxxxx xxxx xxx XxxxxxXxxx$ XxxxxxXxxx$ Xxxxx xxx XxxxxxXxxxx xxxxxxxxxx xx xxx xx xxxxxx x xxxxxxxx xx xxxxxx xx x xxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: String
Parameter Sets: DynamicTypeSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $Xxxxx
Xxxxxxxxx xxx xxxxx xx xxx xxxxxxxx xx xxxxxx.

Xx xxx xxx xx XxxxxXxxxxxxx$ XxxxXxxxxxxx$ XxxxxxXxxxxxxx$ xx XxxxXxxxxx xxxxxx$ xxx xxx xxx xxx XxxxxxXxxxx xxxxxxxxx xx xxx xxxxxxxxxx xxxxxxxxxxx..

Xxx xxxx xxxxxxxxx xxxx xxx XxxxxxXxxx$ XxxxxxXxxx$ Xxxxx xxx XxxxxxXxxxx xxxxxxxxxx xx xxx xx xxxxxx x xxxxxxxx xx xxxxxx xx x xxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: Object
Parameter Sets: DynamicTypeSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxx
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

### $XxxxXx
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

### Xxxxxx.Xxxxxx
Xxx xxx xxxx x xxxxxx xxxx xxxxxxxx xxx xxxxxx xx xxx XxxxxxXxxx$ XxxxXxxx$ xx XxxxXxxx xxxxxxxxxx xx Xxxxxx$XxxxXxxx.

## XXXXXXX

### Xxxx
Xxxx xxxxxx xxxx xxx xxxxxx xxx xxxxxx.

## XXXXX

## XXXXXXX XXXXX

[xxxxx$Xxxxx.xx0xxx]()

[Xxx$XxxxXxxx]()

[Xxxxxx$XxxxXxxx]()

