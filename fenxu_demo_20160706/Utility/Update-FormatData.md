---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294023
schema: 2.0.0
---

# Xxxxxx$XxxxxxXxxx
## XXXXXXXX
Xxxxxxx xxx xxxxxxxxxx xxxx xx xxx xxxxxxx xxxxxxx.

## XXXXXX

```
Update-FormatData [[-AppendPath] <String[]>] [-PrependPath <String[]>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XxxxxxXxxx xxxxxx xxxxxxx xxx xxxxxxxxxx xxxx xxxx xxxxxxxxxx xxxxx xxxx xxx xxxxxxx xxxxxxx.
Xxxx xxxxxx xxxx xxx xxxxxx xxx xxxxxxxxxx xxxx xxxxxxx xxxxxxxxxx Xxxxxxx XxxxxXxxxx.

Xxxxxxx xxxxxxxxxx$ Xxxxxx$XxxxxxXxxx xxxxxxx xxx xxxxxxxxxx xxxxx xxxx xx xxxxxx xxxxxxxxxx.
Xxx xxx xxx xxx xxxxxxxxxx xx Xxxxxx$XxxxxxXxxx xx xxx xxx xxxxxxxxxx xxxxx xx xxx xxxxxxx.

Xxxxxxxxxx xxxxx xxx xxxx xxxxx xx XXX xxxxxx xxxx xxx xxxxxx.xx0xxx xxxx xxxx xxxxxxxxx.
Xxx xxxxxxxxxx xxxx xx xxx xxxxx xxxxxxx xxx xxxxxxx xx Xxxxxxxxx .XXX Xxxxxxxxx xxxxxxx xx xxx xxxxxxx.

Xxxx Xxxxxxx XxxxxXxxxx xxxxxx$ xx xxxxx xxx xxxxxx xxxx xxxx xxx xxxxxxxxxx xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxxxxx xxxxxxxxx $$xxxxxx$ xxxx xxx xxxxxxx.
Xxx xxx xxx Xxxxxx$XxxxxxXxxx xx xxxxxx xxx xxxxxxxxxx xxxx xxxx xxx xxxxxxx xxxxxxx xxxxxxx xxxxxxxxxx Xxxxxxx XxxxxXxxxx.
Xxxx xx xxxxxx xxxx xxx xxxx xxxxx xx xxxxxxx x xxxxxxxxxx xxxx$ xxx xx xxx xxxx xx xxxxxxxxx xxx xxxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxxxxxxxxx xxxxx xx Xxxxxxx XxxxxXxxxx$ xxx xxxxx$Xxxxxx.xx0xxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>update-formatdata
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxxxxxx xxxxx xxxx xx xxxxxx xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>update-formatdata -appendpath trace.format.ps1xml, log.format.ps1xml
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxxxxxx xxxxx xxxx xxx xxxxxxx$ xxxxxxxxx xxx xxx xxxxx$ Xxxxx.xxxxxx.xx0xxx xxx Xxx.xxxxxx.xx0xxx.

Xxxxxxx xxx xxxxxxx xxxx xxx XxxxxxXxxx xxxxxxxxx$ xxx xxxxxxxxxx xxxx xx xxx xxx xxxxx xx xxxxxx xxxxx xxx xxxxxxxxxx xxxx xxxx xxx xxxxx$xx xxxxx.

Xxx XxxxxxXxxx xxxxxxxxx xx xxxx xxxxxxx xxx xxx xxxxx xxxxxxx xxxxxxxxxx xxxx xxx xxxxxxx xxxx xxx xxx xxxxxxxxxx xx xxx xxxxx$xx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>update-formatdata -prependPath c:\test\NewFiles.format.ps1xml

# Edit the NewFiles.format.ps1 file.

PS C:\>update-formatdata
```

Xxxx xxxxxxx xxxxx xxx xx xxxxxx x xxxxxxxxxx xxxx xxxxx xxx xxxx xxxxxx xx.

Xxx xxxxx xxxxxxx xxxx xxx XxxXxxxx.xxxxxx.xx0xxx xxxx xx xxx xxxxxxx.
Xx xxxx xxx XxxxxxxXxxx xxxxxxxxx xxxxxxx xxx xxxx xxxxxxxx xxxxxxxxxx xxxx xxx xxxxxxx xxxx xxx xxxxxxxxxx xx xxx xxxxx$xx xxxxx.

Xxxxx xxxxxx xxx XxxXxxxx.xxxxxx.xx0xxx xxxx xxx xxxxxxx xx xx xxxxx xxxxxxx$ xxx xxxxxx xxxxx xxx xxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx$XxxxxxXxxx xxxxxx xx xxxxxx xxx xxxxxxxxxx xxxxx.
Xxxxxxx xxx XxxXxxxx.xxxxxx.xx0xxx xxxx xxx xxxxxxxxxx xxxxxx$ Xxxxxx$XxxxxxXxxx xxxxxxxxxxxxx xxxxxxx xx xxxxxxx xxxxx xxxxxxxxxx.

## XXXXXXXXXX

### $XxxxxxXxxx
Xxxx xxx xxxxxxxxx xxxxxxxxxx xxxxx xx xxx xxxxxxx.
Xxx xxxxx xxx xxxxxx xxxxx Xxxxxxx XxxxxXxxxx xxxxx xxx xxxxx$xx xxxxxxxxxx xxxxx.

Xxxx xxxxxxxxxx .XXX xxxxxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxx xxxxxxxxxx xxxxxxxxxx xxxx xx xxxxx xxx xxxx .XXX xxxx.
Xx xxx xxx xxx XxxxxxXxxx xxxxxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxxx xxx xxxx xxxx xxx xxxxx$xx xxxxx xxxxxx xx xxxxxxxxxx xxx xxxxxxxxxx xxxx xxxx xxx xxx xxxxxx.

Xxx xxxx xxxxxxxxx xx xxx x xxxx xxxx xxxxxxx x .XXX xxxxxx xxxx xx xxx xxxxxxxxxx xx xxx xxxxx$xx xxxxxxxxxx xxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: PSPath, Path

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### $XxxxxxxxxxxXxxxxx
Xxxx xxxxxxxxxx .XXX xxxxxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxx xxxxxxxxxx xxxxxxxxxx xxxx xx xxxxx xxx xxxx .XXX xxxx.
Xx xxx xxx xxx XxxxxxXxxx xxxxxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxxx xxx xxxx xxxx xxx xxxxx$xx xxxxx xxxxxx xx xxxxxxxxxx xxx xxxxxxxxxx xxxx xxxx xxx xxx xxxxxx.

Xxx xxxx xxxxxxxxx xx xxx x xxxx xxxx xxxxxxx x .XXX xxxxxx xxxx xx xxx xxxxxxxxxx xx xxx xxxxx$xx xxxxxxxxxx xxxxx.

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
Xxxx xxxxxxxxxx .XXX xxxxxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxx xxxxxxxxxx xxxxxxxxxx xxxx xx xxxxx xxx xxxx .XXX xxxx.
Xx xxx xxx xxx XxxxxxXxxx xxxxxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxxx xxx xxxx xxxx xxx xxxxx$xx xxxxx xxxxxx xx xxxxxxxxxx xxx xxxxxxxxxx xxxx xxxx xxx xxx xxxxxx.

Xxx xxxx xxxxxxxxx xx xxx x xxxx xxxx xxxxxxx x .XXX xxxxxx xxxx xx xxx xxxxxxxxxx xx xxx xxxxx$xx xxxxxxxxxx xxxxx.

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
Xxxx xxx xxxxxxxxx xxxxxxxxxx xxxxx xx xxx xxxxxxx.
Xxx xxxxx xxx xxxxxx xxxxxx Xxxxxxx XxxxxXxxxx xxxxx xxx xxxxx$xx xxxxxxxxxx xxxxx.

Xxxx xxxxxxxxxx .XXX xxxxxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxx xxxxxxxxxx xxxxxxxxxx xxxx xx xxxxx xxx xxxx .XXX xxxx.
Xx xxx xxx xxx XxxxxxxXxxx xxxxxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxxx xxx xxxx xxxx xxx xxxxx xxxx xxx xxx xxxxxx xxxxxx xx xxxxxxxxxx xxx xxxxxxxxxx xxxx xxxx xxx xxxxx$xx xxxxx.

Xxx xxxx xxxxxxxxx xx xxx x xxxx xxxx xxxxxxx x .XXX xxxxxx xxxx xx xxxx xxxxxxxxxx xx xxx xxxxx$xx xxxxxxxxxx xxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
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
Xxx xxx xxxx x xxxxxx xxxx xxxxxxxx xxx xxxxxx xxxx xx Xxxxxx$XxxxxxXxxx.

## XXXXXXX

### Xxxx
Xxx xxxxxx xxxx xxx xxxxxx xxx xxxxxx.

## XXXXX
Xxxxxx$XxxxxxXxxx xxxx xxxxxxx xxx xxxxxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxxxx xxxx xxxx xxxxxxxx xxxx xxxxxxx.
Xx xxx xxxxxxxxxx xxxx xxx x xxxxxx xxxxxxx$ xxx xxx xxx xx Xxxxxx$XxxxxxXxxx xxxxxxx xx xxxxxx xxx xxxxxxxxxx xxxx xxx xxxxxxxx xxxxxxxx.
Xxx xx xxx xxxx xx xxxxxx xxx xxxxxx xxxxx.

## XXXXXXX XXXXX

