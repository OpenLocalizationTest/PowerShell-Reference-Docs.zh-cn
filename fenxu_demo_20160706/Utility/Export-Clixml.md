---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293956
schema: 2.0.0
---

# Xxxxxx$Xxxxxx
## XXXXXXXX
Xxxxxxx xx XXX$xxxxx xxxxxxxxxxxxxx xx xx xxxxxx xx xxxxxxx xxx xxxxxx xx xx x xxxx.

## XXXXXX

### XxXxxx $Xxxxxxx$
```
Export-Clixml [-Depth <Int32>] [-Path] <String> -InputObject <PSObject> [-Force] [-NoClobber]
 [-Encoding <String>] [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf]
 [-Confirm]
```

### XxXxxxxxxXxxx
```
Export-Clixml [-Depth <Int32>] -LiteralPath <String> -InputObject <PSObject> [-Force] [-NoClobber]
 [-Encoding <String>] [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf]
 [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XxxXxx xxxxxx xxxxxxx xx XXX$xxxxx xxxxxxxxxxxxxx xx xx xxxxxx xx xxxxxxx xxx xxxxxx xx xx x xxxx.
Xxx xxx xxxx xxx xxx Xxxxxx$XxxXxx xxxxxx xx xx$xxxxxx xxx xxxxx xxxxxx xxxxx xx xxx xxxxxxxx xx xxxx xxxx.

Xxxx xxxxxx xx xxxxxxx xx XxxxxxxXx$XXX$ xxxxxx xxxx Xxxxxx$XxxXxx xxxxxx xxx xxxxxxxxx XXX xx x xxxx.
XxxxxxxXx$XXX xxxxxxx xxx XXX$ xx xxx xxx xxxxxxxx xx xxxxxxx xx xx Xxxxxxx XxxxxXxxxx.

X xxxxxxxx xxx xx Xxxxxx$XxxXxx xx xx xxxxxx xxxxxxxxxxx xxx xxxxxx xxxxxxx xxxxxxxx xx XXX.
Xxx xx xxxxxxx xx xxx xx xx xxxx$ xxx Xxxxxxx 0 xx xxxx xxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>"This is a test" | export-clixml sample.xml
```

Xxxx xxxxxxx xxxxxxx xx XXX xxxx xxxx xxxxxx x xxxxxxxxxxxxxx xx xxx xxxxxx$ $Xxxx xx x xxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-acl C:\test.txt | export-clixml -Path fileacl.xml
PS C:\>$fileacl = import-clixml fileacl.xml
```

Xxxx xxxxxxx xxxxx xxx xx xxxxxx xx xxxxxx xx xx XXX xxxx xxx xxxx xxxxxx xx xxxxxx xx xxxxxxxxx xxx XXX xxxx xxx xxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XXX xxxxxx xx xxx xxx xxxxxxxx xxxxxxxxxx xx xxx Xxxx.xxx xxxx.
Xx xxxx x xxxxxxxx xxxxxxxx xx xxxx xxx xxxxxxxx xxxxxxxxxx xx Xxxxxx$Xxxxxx$ xxxxx xxxxxx xx XXX$xxxxx xxxxxxxxxxxxxx xx xxx xxxxxx xx x xxxx xxxxx XxxxXXX.xxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx$Xxxxxx xxxxxx xx xxxxxx xx xxxxxx xxxx xxx XXX xx xxx XxxxXXX.xxx xxxx.
Xxxx$ xx xxxxx xxx xxxxxx xx xxx $XxxxXxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$credxmlpath = Join-Path (Split-Path $profile) TestScript.ps1.credential
PS C:\>$credential | Export-CliXml $credPath
PS C:\>$credxmlpath = Join-Path (Split-Path $profile) TestScript.ps1.credential
PS C:\>$credential = Import-CliXml $credxmlpath
```

Xxx Xxxxxx$XxxXxx xxxxxx xxxxxxxx xxxxxxxxxx xxxxxxx xx xxxxx xxx Xxxxxxx Xxxx Xxxxxxxxxx XXX.
Xxxx xxxxxxx xxxx xxxx xxxx xxxx xxxxxxx xxx xxxxxxx xxx xxxxxxxx xx xxx xxxxxxxxxx xxxxxx.

Xx xxxx xxxxxxx$ xxxxx x xxxxxxxxxx xxxx xxx$xx xxxxxx xx xxx $xxxxxxxxxx xxxxxxxx xx xxxxxxx xxx Xxx$Xxxxxxxxxx xxxxxx$ xxx xxx xxx xxx Xxxxxx$XxxXxx xxxxxx xx xxxx xxx xxxxxxxxxx xx xxxx.Xx xxx xxxxxxx$ xxx xxxx xx xxxxx xxx xxxxxxxxxx xx xxxxxx xx xxxxxxxxxxx xx XxxxXxxxxx.xx0.xxxxxxxxxx.
Xxxxxxx XxxxXxxxxx xxxx xxx xxxx xx xxx xxxxxx xxxx xxxxx xxx xxx xxxxxxx xxx xxxxxxxxxx.

Xx xxx xxxxxx xxxxxxx$ xxxx xxx xxxxxxxxxx xxxxxx xx Xxxxxx$XxxXxx$ xxx xxxx xx xx xxx xxxx$ $xxxxxxxxxxx$ xxxx xxx xxxxxxxxx xx xxx xxxxx xxxxxxx.

Xx xxxxxx xxx xxxxxxxxxx xxxxxxxxxxxxx xxxx xxxx xxxxxx$ xxx xxx xxxxx xxx xxxxxxxx.
Xxxx xxxx$ xxx xxx xxxxxxx Xxxxxx$XxxXxx xx xxxxxx xxx xxxxxxx xxxxxxxxxx xxxxxx xxxx xxxx xxxxxx.
Xxxx xxxxxxxxxx xxx xxxx xx xxxxxxxx xxxxx$xxxx xxxxxxxxx xx xxxx xxxxxx.

## XXXXXXXXXX

### $Xxxxx
Xxxxxxxxx xxx xxxx xxxxxx xx xxxxxxxxx xxxxxxx xxx xxxxxxxx xx xxx XXX xxxxxxxxxxxxxx.
Xxx xxxxxxx xxxxx xx 0.

Xxx xxxxxxx xxxxx xxx xx xxxxxxxxxx xxx xxx xxxxxx xxxx xx xxx Xxxxx.xx0xxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxx.xx0xxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxxxxxxx xxx xxxx xx xxxxxxxx xxx xxx xxxxxx xxxx.
Xxxxx xxxxxx xxx XXXXX$ XXX0$ XXX0$ XXX00$ Xxxxxxx$ XxxXxxxxxXxxxxxx$ Xxxxxxx$ xxx XXX.
Xxxxxxx xx xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: Unicode, UTF7, UTF8, ASCII, UTF32, BigEndianUnicode, Default, OEM

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxx
Xxxxxx xxx xxxxxx xx xxxxx xxx xxxx$xxxx xxxxxxxxx xx xxx xxxxxx xxxx xx xxxxxxxxx. Xxx xxxxxx xxxx xxxxxxx xx xxxxx xxx xxxx$xxxx xxxxxxxxx xxxx xxx xxxxxxx xxxxxxxxx.

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
Xxx xxxxxxx xxxxx xxx xx xxxxxxxxxx xxx xxx xxxxxx xxxx xx xxx Xxxxx.xx0xxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxx.xx0xxx.

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
Xxx xxxxxxx xxxxx xxx xx xxxxxxxxxx xxx xxx xxxxxx xxxx xx xxx Xxxxx.xx0xxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxx.xx0xxx.

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
Xxxxxxxxx xxx xxxxxx xx xx xxxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx$ xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.
Xxx xxx xxxx xxxx xxxxxxx xx Xxxxxx$Xxxxxx.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $XxXxxxxxx
Xxxxxxx xxxx xxx xxxxxx xxxx xxx xxxxxxxxx xxx xxxxxxxx xx xx xxxxxxxx xxxx.
Xx xxxxxxx$ xx x xxxx xxxxxx xx xxx xxxxxxxxx xxxx$ Xxxxxx$Xxxxxx xxxxxxxxxx xxx xxxx xxxxxxx xxxxxxx.

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
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxxx xxx XXX xxxxxxxxxxxxxx xx xxx xxxxxx xxxx xx xxxxxx.

```yaml
Type: String
Parameter Sets: ByPath
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxxx xxx XXX xxxxxxxxxxxxxx xx xxx xxxxxx xxxx xx xxxxxx.
Xxxxxx Xxxx$ xxx xxxxx xx xxx XxxxxxxXxxx xxxxxxxxx xx xxxx xxxxxxx xx xx xx xxxxx.
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

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxx xxxx xxx xxxxxx xx Xxxxxx$Xxxxxx.

## XXXXXXX

### Xxxxxx.XX.XxxxXxxx
Xxxxxx$Xxxxxx xxxxxxx x xxxx xxxx xxxxxxxx xxx XXX.

## XXXXX

## XXXXXXX XXXXX

[Xxx XxxxxXxxxx xx Xxxx Xxxxxxxxxxx xx Xxxxxx Xxxxxxx]()

[Xxxxxxxx Xxxxx Xxxxxxxxxxx xx Xxxx]()

[XxxxxxxXx$Xxxx]()

[XxxxxxxXx$Xxx]()

[Xxxxxx$Xxx]()

[Xxxxxx$Xxxxxx]()

