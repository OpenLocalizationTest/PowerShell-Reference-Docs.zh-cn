---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293958
schema: 2.0.0
---

# Xxxxxx$XxxxxxXxxx
## XXXXXXXX
Xxxxx xxxxxxxxxx xxxx xxxx xxx xxxxxxx xxxxxxx xx x xxxxxxxxxx xxxx.

## XXXXXX

### XxXxxx $Xxxxxxx$
```
Export-FormatData -InputObject <ExtendedTypeDefinition[]> -Path <String> [-Force] [-NoClobber]
 [-IncludeScriptBlock] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### XxXxxxxxxXxxx
```
Export-FormatData -InputObject <ExtendedTypeDefinition[]> -LiteralPath <String> [-Force] [-NoClobber]
 [-IncludeScriptBlock] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XxxxxxXxxx xxxxxx xxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxxxxx xxxxx $xxxxxx.xx0xxx$ xxxx xxx xxxxxxxxxx xxxxxxx xx xxx xxxxxxx xxxxxxx.
Xx xxxxx xxx XxxxxxxxXxxxXxxxxxxxxx xxxxxxx xxxx Xxx$XxxxxxXxxx xxxxxxx xxx xxxxx xxxx xx x xxxx xx XXX xxxxxx.

Xxxxxxx XxxxxXxxxx xxxx xxx xxxx xx xxxxxxxxxx xxxxx $xxxxxx.xx0xxx$ xx xxxxxxxx xxx xxxxxxx xxxxxxx xx Xxxxxxxxx .XXX Xxxxxxxxx xxxxxxx xx xxx xxxxxxx.
Xxx xxx xxxx xxx xxxx xxx xxxxxxxxxx xxxxx xxx xxx xxx Xxxxxx$XxxxxxXxxx xxxxxx xx xxx xxx xxxxxxxxxx xxxx xx x xxxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxxxxxxxxx xxxxx xx Xxxxxxx XxxxxXxxxx$ xxx xxxxx$Xxxxxx.xx0xxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-formatdata -typename * | export-formatdata -path allformat.ps1xml -IncludeScriptBlock
```

Xxxx xxxxxxx xxxxxxx xxx xx xxx xxxxxx xxxx xx xxx xxxxxxx xx xxx XxxXxxxxx.xx0xxx xxxx.

Xxx xxxxxxx xxxx xxx Xxx$XxxxxxXxxx xxxxxx xx xxx xxx xxxxxx xxxx xx xxx xxxxxxx.
X xxxxx xx $ $xxx$ xxx xxx XxxxXxxx xxxxxxxxx xxxxxxx xxx xxxxxx xx xxx xxx xx xxx xxxx xx xxx xxxxxxx.

Xxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xxxx xxxx xxx Xxx$XxxxxxXxxx xxxxxxx xx xxx Xxxxxx$XxxxxxXxxx xxxxxx$ xxxxx xxxxxxx xxx xxxxxx xxxx xx xxx XxxXxxxxx.xx0 xxxx.

Xxx Xxxxxx$XxxxxxXxxx xxxxxxx xxxx xxx XxxxxxxXxxxxxXxxxx xxxxxxxxx xx xxxxxxx xxxxxx xxxxxx xx xxx xxxxxx xxxx xx xxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$f = get-formatdata -typename helpinfoshort
PS C:\>export-formatdata -inputObject $f -path c:\test\help.format.ps1xml -IncludeScriptBlock
```

Xxxxx xxxxxxxx xxxxxx xxx xxxxxx xxxx xxx xxx XxxxXxxxXxxxx xxxx xx xxx Xxxx.xxxxxx.xx0xxx xxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XxxxxxXxxx xxxxxx xx xxx xxx xxxxxx xxxx xxx xxx XxxxXxxxXxxxx xxxx$ xxx xx xxxxx xx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx XxxxxXxxxxx xxxxxxxxx xx xxx Xxxxxx$XxxxxxXxxx xx xxxxx xxx xxxxxx xxxx xxxxx xx xxx $x xxxxxxxx.
Xx xxxx xxxx xxx XxxxxxxXxxxxxXxxxx xxxxxxxxx xx xxxxxxx xxxxxx xxxxxx xx xxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-formatdata -typename System.Diagnostics.Process | export-FormatData -path process.format.ps1xml
PS C:\>Update-FormatData -prependPath .\process.format.ps1xml
PS C:\>get-process p*

Handles  NPM(K)  PM(K)  WS(K) VM(M)   CPU(s)    Id ProcessName
-------  ------  -----  ----- -----   ------    -- -----------
323                                       5600 powershell
336                                       3900 powershell_ise
138                                       4076 PresentationFontCache
```

Xxxx xxxxxxx xxxxx xxx xxxxxx xx xxxxxxxx xxx XxxxxxxXxxxxxXxxxx xxxxxxxxx xxxx xx Xxxxxx$XxxxxxXxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XxxxxxXxxx xxxxxx xx xxx xxx xxxxxx xxxx xxx xxx Xxxxxx.Xxxxxxxxxxx.Xxxxxxx xxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xxxxxxx.
Xxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxxxxx xxxx xx xxx Xxxxxx$XxxxxxXxxx xxxxxx$ xxxxx xxxxxxx xx xx xxx Xxxxxxx.xxxxxx.xx0xxx xxxx xx xxx xxxxxxx xxxxxxxxx.

Xx xxxx xxxx$ xxx Xxxxxx$XxxxxxXxxx xxxxxxx xxxx xxx xxx xxx XxxxxxxXxxxxxXxxxx xxxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx$XxxxxxXxxx xxxxxx xx xxx xxx Xxxxxxx.xxxxxx.xx0xxx xxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx XxxxxxxXxxx xxxxxxxxx xx xxxxxx xxxx xxx xxxxxxxxxx xxxx xxx xxxxxxx xxxxxxx xx xxx Xxxxxxx.xxxxxx.xx0xxx xxxx xx xxxxx xxxxxx xxx xxxxxxxx xxxxxxxxxx xxxx xxx xxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxxx xxx xxxxxxx xx xxxx xxxxxx.
Xxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxxxxxxxx xxxx xxxx xxxxx xxxx xxxxx xxxx $X$.
Xxx xxxxxx xxxxx xxxx xxxxxxxx xxxxxx xxxx xxx xxxxxxxxxx xx xxxxx xxxxxx xxxxxx xxx xxxxxxx xxxx xxx xxxxxxx.

## XXXXXXXXXX

### $Xxxxx
Xxxxxxxxxx xx xxxxxxxx xxxxxx xxxx$ xxxx xx xxx xxxx xxx xxx xxxx$xxxx xxxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxxxxXxxxx
Xxxxxxxxxx xxxxxxx xxxxxx xxxxxx xx xxx xxxxxx xxxx xxx xxxxxxxx.

Xxxxxxx xxxxxx xxxxxx xxxxxxx xxxx xxx xxx xx xxxx xxxxxxxxxxx$ xxxx xxx xxx xxxxxxxx xx xxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

### $XxxxxXxxxxx
Xxxxxxxxx xxx xxxxxx xxxx xxxxxxx xx xx xxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx x xxxxxxx xxxx xxxx xxx xxxxxxx$ xxxx xx x Xxx$XxxxxxXxxx xxxxxxx.
Xxx xxx xxxx xxxx xxx xxxxxxx xxxx Xxx$XxxxxxXxxx xx Xxxxxx$XxxxxxXxxx.

```yaml
Type: ExtendedTypeDefinition[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $XxXxxxxxx
Xxxxxxxx xxx xxxxxx xxxx xxxxxxxxxxx xxxxxxxx xxxxx.
Xx xxxxxxx$ Xxxxxx$XxxxxxXxxx xxxxxxxxxx xxxxx xxxxxxx xxxxxxx xxxxxx xxx xxxx xxx xxx xxxx$xxxx xxxxxxxxx.

Xx xxxxxx Xxxxxx$XxxxxxXxxx xx xxxxxxxxx xxxx$xxxx xxxxx$ xxx xxx Xxxxx xxxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: NoOverwrite

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx x xxxxxxxx xxx xxx xxxxxx xxxx. Xxxxx x xxxx $xxxxxxxx$ xxx xxxx xxxx xxxx x xxxxxx.xx0xxx xxxx xxxx xxxxxxxxx.
Xx xxx xxxx xxx xxxx$ Xxxxxx$XxxxxxXxxx xxxxxxx xxx xxxx xx xxx xxxxxxx xxxxxxxxx.

Xx xxx xxx x xxxx xxxx xxxxxxxxx xxxxx xxxx .xx0xxx$ xxx Xxxxxx$XxxxxxXxxx xxxxxx xxxx xxx xxxxxxxxx xxx xxxx.

Xx xxx xxxxxxx xx xxxxxxxx xxxx$ Xxxxxx$XxxxxxXxxx xxxxxxxxxx xxx xxxx xxxxxxx xxxxxxx$ xxxxxx xxx xxxx xxx xxx xxxx$xxxx xxxxxxxxx.
Xx xxxxxxxxx x xxxx$xxxx xxxx$ xxx xxx Xxxxx xxxxxxxxx.
Xx xxxxxxx xxxxx xxxx xxxxx xxxxxxxxxxx$ xxx xxx XxXxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: ByPath
Aliases: FilePath

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxx
Xxxxxxxxx x xxxxxxxx xxx xxx xxxxxx xxxx.
Xxxxxx xxx Xxxx xxxxxxxxx$ xxx xxxxx xx XxxxxxxXxxx xx xxxx xxxxxxx xx xx xx xxxxx.
Xx xxxxxxxxxx xxx xxxxxxxxxxx xx xxxxxxxxx.
Xx xxx xxxx xxxxxxxx xxxxxx xxxxxxxxxx$ xxxxxxx xx xx xxxxxx xxxxxxxxx xxxxx.
Xxxxxx xxxxxxxxx xxxxx xxxx Xxxxxxx XxxxxXxxxx xxx xx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: ByLiteralPath
Aliases: PSPath

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XxxxxxxxXxxxXxxxxxxxxx
Xxx xxx xxxx XxxxxxxxXxxxXxxxxxxxxx xxxxxxx xxxx Xxx$XxxxxxXxxx xx Xxxxxx$XxxxxxXxxx.

## XXXXXXX

### Xxxx
Xxxxxx$XxxxxxXxxx xxxx xxx xxxxxx xxx xxxxxxx.
Xx xxxxxxxxx x xxxx xxx xxxxx xx xx xxx xxxxxxxxx xxxx.

## XXXXX
Xx xxx xxx xxxxxxxxxx xxxx$ xxxxxxxxx xx xxxxxxxx xxxxxxxxxx xxxx$ xxx xxxxxxxxx xxxxxx xxx xxx xxxxxxx xxxx xxxxx xxxxxxx xxx xxxxxxxxxxxxx xxxxx xx xxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxx.

## XXXXXXX XXXXX

[Xxx$XxxxxxXxxx]()

[Xxxxxx$XxxxxxXxxx]()

