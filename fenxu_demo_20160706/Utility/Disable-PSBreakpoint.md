---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293953
schema: 2.0.0
---

# Xxxxxxx$XXXxxxxxxxxx
## XXXXXXXX
Xxxxxxxx xxx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxx.

## XXXXXX

### Xxxxxxxxxx $Xxxxxxx$
```
Disable-PSBreakpoint [-PassThru] [-Breakpoint] <Breakpoint[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### Xx
```
Disable-PSBreakpoint [-PassThru] [-Id] <Int32[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxxx$XXXxxxxxxxxx xxxxxx xxxxxxxx xxxxxxxxxxx$ xxxxx xxxxxxx xxxx xxxx xxx xxx xxx xxxx xxx xxxxxx xxxx.
Xxx xxx xxx xx xx xxxxxxx xxx xxxxxxxxxxx$ xx xxx xxx xxxxxxx xxxxxxxxxxx xx xxxxxxxxxx xxxxxxxxxx xxxxxxx xx xxxxxxxxxx XXx.

Xxxxxxxxxxx$ xxxx xxxxxx xxxxxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx x xxxxxxxxxx xxxxxx xx Xxxxx.
Xx xx$xxxxxx x xxxxxxxxxx$ xxx xxx Xxxxxx$XXXxxxxxxxxx xxxxxx.
Xxxxxxxxxxx xxx xxxxxxx xx xxxxxxx xxxx xxx xxxxxx xxxx xx xxxxx xxx Xxx$XXXxxxxxxxxx xxxxxx.

X xxxxxxxxxx xx x xxxxx xx x xxxxxx xxxxx xxxxxxxxx xxxxx xxxxxxxxxxx xx xxxx xxx xxx xxxxxxx xxx xxxxxxxxxxxx xx xxx xxxxxx.
Xxxxxxx$XXXxxxxxxxxx xx xxx xx xxxxxxx xxxxxxx xxxxxxxx xxx xxxxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx$ xxx xxxxx$Xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$b = set-psbreakpoint -script sample.ps1 -variable name
PS C:\>$b | disable-psbreakpoint
```

Xxxxx xxxxxxxx xxxxxxx x xxxxx$xxxxxxx xxxxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XXXxxxxxxxxx xxxxxx xx xxxxxx x xxxxxxxxxx xx xxx Xxxx xxxxxxxx xx xxx Xxxxxx.xx0 xxxxxx.
Xxxx$ xx xxxxx xxx xxxxxxxxxx xxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxxx$XXXxxxxxxxxx xxxxxx xx xxxxxxx xxx xxx xxxxxxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxxxxx xxxxxx xx $x xx xxx Xxxxxxx$XXXxxxxxxxxx xxxxxx.

Xx x xxxxxx xx xxxx xxxxxxx$ xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxxxxxx xxxxxx xx $x xx Xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>disable-psbreakpoint -id 0
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxxxx xxxx xxxxxxxxxx XX 0.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>disable-psbreakpoint -breakpoint ($b = set-psbreakpoint -script sample.ps1 -line 5)
PS C:\>$b
```

Xxxx xxxxxxx xxxxxxx x xxx xxxxxxxxxx xxxx xx xxxxxxxx xxxxx xxx xxxxxx xx.

Xx xxxx xxx Xxxxxxx$XXXxxxxxxxxx xxxxxx xx xxxxxxx xxx xxxxxxxxxx.
Xxx xxxxx xx xxx Xxxxxxxxxx xxxxxxxxx xx x Xxx$XXXxxxxxxxxx xxxxxxx xxxx xxxx x xxx xxxxxxxxxx$ xxxxxxxxx x xxxxxxxxxx xxxxxx$ xxx xxxxx xxx xxxxxx xx xxx $x xxxxxxxx.

Xxxxxx xxxxxxxxxx xxxx xxxx xxxxxxx xx xxxxx xxxxxx xxx xxxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxx xx x xxxxxxx xxxx xxxx xx xxxxxxxxx xxx xxxxxx.
Xx xxxx xxxx$ xxxxxxx Xxx$XXXxxxxxxxxx xxxxxxxxx x xxxxxxxxxx xxxxxx$ xx xxx xx xxxx xx xxx xxxxx xx xxx Xxxxxxxxxx xxxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxxx xxx xxxxxxxxxx xxxxxx xx xxx xxxxx xx xxx $x xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-psbreakpoint | disable-psbreakpoint
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxx xxxxxxxxxx xxxx xxxxxxx xx$ $xxx $ xxx$.

## XXXXXXXXXX

### $Xxxxxxxxxx
Xxxxxxxxx xxx xxxxxxxxxxx xx xxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxxxxxxxxx xxxxxxx xx x xxxxxxx xxxx xxxx xxxxxxxxxx xxxxxxx$ xxxx xx x Xxx$XXXxxxxxxxxx xxxxxxx.
Xxx xxx xxxx xxxx xxxxxxxxxx xxxxxxx xx xxx Xxxxxxx$XXXxxxxxxxxx xxxxxx.

```yaml
Type: Breakpoint[]
Parameter Sets: Breakpoint
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $Xx
Xxxxxxxx xxx xxxxxxxxxxx xxxx xxx xxxxxxxxx xxxxxxxxxx XXx.
Xxxxx xxx XXx xx x xxxxxxxx xxxx xxxxxxxx xxx XXx.
Xxx xxxxxx xxxx XXx xx Xxxxxxx$XXXxxxxxxxxx.

```yaml
Type: Int32[]
Parameter Sets: Id
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
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

### $XxxxXxxx
Xxxxxxx xx xxxxxx xxxxxxxxxxxx xxx xxxxxxx xxxxxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

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

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.Xxxxxxxxxx
Xxx xxx xxxx x xxxxxxxxxx xxxxxx xx Xxxxxxx$XXXxxxxxxxxx.

## XXXXXXX

### Xxxx xx Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.Xxxxxxxxxx
Xxxx xxx xxx xxx XxxxXxxx xxxxxxxxx$ Xxxxxxx$XXXxxxxxxxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxxx xxxxxxxxxx.
Xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX

## XXXXXXX XXXXX

[Xxxxxx$XXXxxxxxxxxx]()

[Xxx$XXXxxxxxxxxx]()

[Xxx$XXXxxxXxxxx]()

[Xxxxxx$XXXxxxxxxxxx]()

[Xxx$XXXxxxxxxxxx]()

[xxxxx$Xxxxxxxxx]()

