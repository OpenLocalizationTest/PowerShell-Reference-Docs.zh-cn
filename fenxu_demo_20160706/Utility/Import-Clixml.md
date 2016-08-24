---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293982
schema: 2.0.0
---

# Xxxxxx$Xxxxxx
## XXXXXXXX
Xxxxxxx x XXXXXX xxxx xxx xxxxxxx xxxxxxxxxxxxx xxxxxxx xxxxxx Xxxxxxx XxxxxXxxxx.

## XXXXXX

### XxXxxx $Xxxxxxx$
```
Import-Clixml [-Path] <String[]> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-IncludeTotalCount] [-Skip <UInt64>] [-First <UInt64>]
```

### XxXxxxxxxXxxx
```
Import-Clixml -LiteralPath <String[]> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-IncludeTotalCount] [-Skip <UInt64>] [-First <UInt64>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XxxXxx xxxxxx xxxxxxx x XXXXXX xxxx xxxx xxxx xxxx xxxxxxxxxx Xxxxxxxxx .XXX Xxxxxxxxx xxxxxxx xxx xxxxxxx xxx xxxxxxx xx Xxxxxxx XxxxxXxxxx.

X xxxxxxxx xxx xx Xxxxxx$XxxXxx xx xx xxxxxx xxxxxxxxxxx xxx xxxxxx xxxxxxx xxxx xxxx xxxx xxxxxxxx xx xxxxxx XXX xx xxxxxxx xxx Xxxxxx$XxxXxx xxxxxx.
Xxx xx xxxxxxx xx xxx xx xx xxxx$ xxx Xxxxxxx 0 xx xxxx xxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | export-clixml pi.xml
PS C:\>$processes = import-clixml pi.xml
```

Xxxx xxxxxxx xxxx xxx Xxxxxx$Xxxxxx xxxxxx xx xxxx x xxxxxxxxxx xxxx xx xxx xxxxxxx xxxxxxxxxxx xxxxxxxx xx Xxx$Xxxxxxx.
Xx xxxx xxxx Xxxxxx$Xxxxxx xx xxxxxxxx xxx xxxxxxxx xx xxx xxxxxxxxxx xxxx xxx xx$xxxxxx xx xxxxxx xxxx xx xxxxxx xx xxx $xxxxxxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$credxmlpath = Join-Path (Split-Path $profile) TestScript.ps1.credential
PS C:\>$credential | Export-CliXml $credxmlpath PS C:\>$credxmlpath = Join-Path (Split-Path $profile) TestScript.ps1.credential
PS C:\>$credential = Import-CliXml $credxmlpath
```

Xxx Xxxxxx$XxxXxx xxxxxx xxxxxxxx xxxxxxxxxx xxxxxxx xx xxxxx xxx Xxxxxxx Xxxx Xxxxxxxxxx XXX.
Xxxx xxxxxxx xxxx xxxx xxxx xxxx xxxxxxx xxx xxxxxxx xxx xxxxxxxx xx xxx xxxxxxxxxx xxxxxx.

Xx xxxx xxxxxxx$ xxxxx x xxxxxxxxxx xxxx xxx$xx xxxxxx xx xxx $xxxxxxxxxx xxxxxxxx xx xxxxxxx xxx Xxx$Xxxxxxxxxx xxxxxx$ xxx xxx xxx xxx Xxxxxx$XxxXxx xxxxxx xx xxxx xxx xxxxxxxxxx xx xxxx.Xx xxx xxxxxxx$ xxx xxxx xx xxxxx xxx xxxxxxxxxx xx xxxxxx xx xxxxxxxxxxx xx XxxxXxxxxx.xx0.xxxxxxxxxx.
Xxxxxxx XxxxXxxxxx xxxx xxx xxxx xx xxx xxxxxx xxxx xxxxx xxx xxx xxxxxxx xxx xxxxxxxxxx.

Xx xxx xxxxxx xxxxxxx$ xxx xxxx xxx xxxxxxxxxx xxxxxx xx Xxxxxx$XxxXxx$ xxx xxxx xx xx xxx xxxx$ $xxxxxxxxxxx$ xxxx xxx xxxxxxxxx xx xxx xxxxx xxxxxxx.

Xx xxxxxx xxx xxxxxxxxxx xxxxxxxxxxxxx xxxx xxxx xxxxxx$ xxx xxx xxxxx xxx xxxxxxxx.
Xxxx xxxx$ xxx xxx xxxxxxx Xxxxxx$XxxXxx xx xxxxxx xxx xxxxxxx xxxxxxxxxx xxxxxx xxxx xxxx xxxxxx.
Xxxx xxxxxxxxxx xxx xxxx xx xxxxxxxx xxxxx$xxxx xxxxxxxxx xx xxxx xxxxxx.

## XXXXXXXXXX

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

### $Xxxx
Xxxxxxxxx xxx XXX xxxxx.

```yaml
Type: String[]
Parameter Sets: ByPath
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### $XxxxxxxXxxx
Xxxxxxxxx xxx XXX xxxxx.
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

### $Xxxxx
Xxxx xxxx xxx xxxxxxxxx xxxxxx xx xxxxxxx.
Xxxxx xxx xxxxxx xx xxxxxxx xx xxx.

```yaml
Type: UInt64
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxx xxx xxxxxxxxx xxxxxx xx xxxxxxx xxx xxxx xxxx xxx xxxxxxxxx xxxxxxx.
Xxxxx xxx xxxxxx xx xxxxxxx xx xxxx.

```yaml
Type: UInt64
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxxxXxxxx
Xxxxxxx xxx xxxxx xxxxxx xx xxxxxxx xx xxx xxxx xxx $xx xxxxxxx$ xxxxxxxx xx xxx xxxxxxxx xxxxxxx.
Xx xxx xxxxxx xxxxxx xxxxxxxxx xxx xxxxx xxxxx$ xx xxxxxxxx $Xxxxxxx xxxxx xxxxx.$ Xxx xxxxxxx xxx xx Xxxxxxxx xxxxxxxx xxxx xxxxxxxxx xxx xxxxxxxxxxx xx xxx xxxxx xxxxx xxxxx.
Xxx xxxxx xx Xxxxxxxx xxxxxx xxxx 0.0 xx 0.0 xxxxx 0.0 xxxxx xxxx xxx xxxxxx xxxxx xxx xxxxx xxx xxxxxxx$ 0.0 xxxxx xxxx xxx xxxxx xx xxxxx$ xxx x xxxxx xxxxxxx 0.0 xxx 0.0 xxxxxxxxx xx xxxxxxxxxxxx xxxxxxxx xxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxx
Xxx xxx xxxx x xxxxxx xxxx xxxxxxxx x xxxx xx Xxxxxx$Xxxxxx.

## XXXXXXX

### XXXxxxxx
Xxxxxx$Xxxxxx xxxxxxx xxxxxxx xxxx xxxx xxxx xxxxxxxxxxxx xxxx xxx xxxxxx XXX xxxxx.

## XXXXX
Xxxx xxxxxxxxxx xxxxxxxx xxxxxx xxx x xxxxxxxxx$ xxx xxxxxx xx xxxxxxxx xxx xxxxxx.
Xxx xxxxxxx$ $$$xxxxxxxxx$xxxx$$ $$xxxxx0$$$ $$xxxxx0$$$.

## XXXXXXX XXXXX

[Xxx XxxxxXxxxx xx Xxxx Xxxxxxxxxxx xx Xxxxxx Xxxxxxx]()

[Xxxxxxxx Xxxxx Xxxxxxxxxxx xx Xxxx]()

[Xxxxxx$XxxXxx]()

