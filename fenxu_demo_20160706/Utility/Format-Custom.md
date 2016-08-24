---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293960
schema: 2.0.0
---

# Xxxxxx$Xxxxxx
## XXXXXXXX
Xxxx x xxxxxxxxxx xxxx xx xxxxxx xxx xxxxxx.

## XXXXXX

```
Format-Custom [[-Property] <Object[]>] [-Depth <Int32>] [-GroupBy <Object>] [-View <String>] [-ShowError]
 [-DisplayError] [-Force] [-Expand <String>] [-InputObject <PSObject>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxxxxx xxxxxx xxxxxxx xxx xxxxxx xx x xxxxxxx xx xxxxxxx xx xx xxxxxxxxx xxxx.
Xxxxxx$Xxxxxx xx xxxxxxxx xx xxxxxxx xxxxx xxxx xxx xxx xxxx xxxxxx xx xxxx xxxxx.
Xxx xxx xxx xxx xxxxx xxxxxxx xx xxx $xxxxxx.XX0XXX xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxx$ xx xxx xxx xxxxxx xxxx xxx xxxxx xx xxx XX0XXX xxxxx xxx xxx xxx Xxxxxx$XxxxxxXxxx xxxxxx xx xxx xxxx xx Xxxxxxx XxxxxXxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-command start-transcript | format-custom -view MyView
```

Xxxx xxxxxxx xxxxxxx xxxxxxxxxxx xxxxx xxx Xxxxx$Xxxxxxxxxx xxxxxx xx xxx xxxxxx xxxxxxx xx xxx XxXxxx xxxx$ x xxxxxx xxxx xxxxxxx xx xxx xxxx.
Xx xxx xxxx xxxxxxx xxxxxxxxxxxx$ xxx xxxx xxxxx xxxxxx x xxx XX0XXX xxxx$ xxxxxx xxx XxXxxx xxxx$ xxx xxxx xxx xxx Xxxxxx$XxxxxxXxxx xxxxxxx xx xxx xxx XX0XXX xxxx xx Xxxxxxx XxxxxXxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process Winlogon | format-custom
```

Xxxx xxxxxxx xxxxxxx xxxxxxxxxxx xxxxx xxx Xxxxxxxx xxxxxxx xx xx xxxxxxxxx xxxxxxxxxx xxxx.
Xxxxxxx xxx xxxxxxx xxxx xxx xxx xxx Xxxx xxxxxxxxx$ Xxxxxx$Xxxxxx xxxx x xxxxxxx xxxxxx xxxx xx xxxxxx xxx xxxx.

## XXXXXXXXXX

### $Xxxxx
Xxxxxxxxx xxx xxxxxx xx xxxxxxx xx xxx xxxxxxx.

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

### $XxxxxxxXxxxx
Xxxxxxxx xxxxxx xx xxx xxxxxxx xxxx.
Xxxx xxxxxxxxx xx xxxxxx xxxx$ xxx xxx xx xxxx xx x xxxxxxxxx xxx xxxx xxx xxx xxxxxxxxxx xxxxxxxxxxx xx x Xxxxxx$Xxxxxx xxxxxxx$ xxx xxx xxxxxxxxxxx xx xxx xxxxxx xx xx xxxxxxx.
Xxx xxxxxxxxx xxxxx xx xxxxxxx xx xxx xxxxxxx xx xxxxxx xxx XxxxxxxXxxxx xxxxxxxxx xxxx xx xxxxxxxxxx.

XX $$ Xxx$Xxxx $ Xxxxxx$Xxxxxx XxxXxXxxx$$ $$ $ $xxxx $ $XxxxXxxxx XxxXxXxxx  $$ $ $xxxx
--------- ------------
Xxxxxxxxx $XXX

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

### $Xxxxxx
Xxxxxxx xxx xxxxxxxxxx xxxxxx$ xx xxxx xx xxx xxxxxxx xx xxx xxxxxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx xx xxxxxx xxxxxxx xxxx xxxxxxx xxx XXxxxxxxxxx $Xxxxxx.Xxxxxxxxxxx$ xxxxxxxxx.
Xxx xxxxxxx xxxxx xx XxxxXxxx.

Xxxxx xxxxxx xxx$

$$ XxxxXxxx$ Xxxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxx xx xxx xxxxxxxxxx.
$$ XxxxXxxx$ Xxxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxxxxx xxxxxx.
$$ Xxxx$ Xxxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxxxxx xxxxxx xxx xxx xxxxxxxxxx xx xxxxxxx xx xxx xxxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: CoreOnly, EnumOnly, Both

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxx
Xxxxxxx xxx xxxxxx xx xxxxxxx xxx xx xxx xxxxx xxxxxxxxxxx.
Xxx xxxx xxx XxxxxxxXxxxx xx XxxxXxxxx xxxxxxxxxx.
Xx xxxxxxx$ xxxx xx xxxxx xxxxxx xx xxxxxxx xx xxx xxxxx xx xxxxxxx xxxxxxx$ xxxx xxxx xx xxx xxxxx xxxxxxxxxxx xx xxxxxxxxx.

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

### $XxxxxXx
Xxxxxxx xxx xxxxxx xx xxxxxx xxxxx xx x xxxxxx xxxxxxxx xx xxxxx.
Xxxxx xx xxxxxxxxxx xx x xxxxxxxx xx xxx xxxxxx.

Xxx xxxxx xx xxx XxxxxXx xxxxxxxxx xxx xx x xxx xxxxxxxxxx xxxxxxxx.
Xx xxxxxx x xxxxxxxxxx$ xxxxxxxx$ xxx x xxxx xxxxx.
Xxxxx xxxx xxx$

$$ Xxxx $xx Xxxxx$ $$xxxxxx$$$$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxx xxxxx$$$$$ XxxxxxXxxxxx $$xxxxxx\>

```yaml
Type: Object
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
Xxxxxxxxx xxx xxxxxxx xx xx xxxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxxx xxxxxxxxxx xxxx xxxxxx xx xxx xxxxxxx xxx xxx xxxxx xx xxxxx xxxx xxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

Xx xxx xxxx xxxx xxxxxxxxx$ xxx xxxxxxxxxx xxxx xxxxxx xx xxx xxxxxxx xxxxxx xx xxx xxxxxx xxxxx xxxxxxxxx.
Xxx xxxxxxxxx xxxx $$Xxxxxxxx$$ xx xxxxxxxx.
Xxx xxxxxx xxx xxx Xxxxxxxx xxx Xxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

Xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx xxx xx x xxx xxxxxxxxxx xxxxxxxx.
Xx xxxxxx x xxxxxxxxxx xxxxxxxx$ xxx x xxxx xxxxx.
Xxxxx xxxx xxx$

$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxx xxxxx$$$$$ Xxxxx $$xxx00\>

```yaml
Type: Object[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxxx
Xxxxx xxxxxx xxxxxxx xxx xxxxxxxx.
Xxxx xxxxxxxxx xx xxxxxx xxxx$ xxx xxx xx xxxx xx x xxxxxxxxx xxx xxxx xxx xxx xxxxxxxxxx xxxxxxxxxxx xx x Xxxxxx$Xxxxxx xxxxxxx$ xxx xxx xxxxxxxxxxx xx xxx xxxxxx xx xx xxxxxxx.
Xxx xxxxxxxxx xxxxx xx xxxxxxx xx xxx xxxxxxx xx xxxxxx xxx XxxxXxxxx xxxxxxxxx xxxx xx xxxxxxxxxx.

XX $$ Xxx$Xxxx $ Xxxxxx$Xxxxxx XxxXxXxxx$$ $$ $ $xxxx $ $XxxxXxxxx XxxXxXxxx  $$ $ $xxxx
--------- ------------
Xxxxxxxxx

Xxxxxx xx xxxxxxxx xxxxxxxxxx $ $$ $ $xxxx $.
$ XxxxxxxxXxxx          $ XxxxxxxXxxxxxxx$ $00$00$0000 0$00$00 XX$XXXxxxxx$ $$$$$ XxxxxxxXxxxxxxxx $ XxxxxXxxxxxxxxXxxxxXx $ xxxXxxxxxxxxxXxxxx

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

### $Xxxx
Xxxxxxxxx xxx xxxx xx xx xxxxxxxxx xxxxxx xx $xxxx.$ Xx xxx xxxx xxxx xxxxxxxxx$ Xxxxxx$Xxxxxx xxxx x xxxxxxx xxxxxx xxxx.
Xxx xxxxxx xxx xxx Xxxxxxxx xxx Xxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxx xxxx xxx xxxxxx xx Xxxxxx$Xxxxxx

## XXXXXXX

### Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.Xxxxxxxx.Xxxxxx
Xxxxxx$Xxxxxx xxxxxxx xxx xxxxxx xxxxxxx xxxx xxxxxxxxx xxx xxxxxxx.

## XXXXX
Xxxxxx$Xxxxxx xx xxxxxxxx xx xxxxxxx xxxxx xxxx xxx xxx xxxx xxxxxx xx xxxx xxxxx.
Xx xxxxxxx xx xxxxxxxxx xxxxx xxxx$ xxx Xxxxxx$Xxxxx.
Xx xxxxxxx xx xxxxxxxxx xxxx xxxx$ xxx Xxxxxx$Xxxx.

Xxx xxx xxxx xxxxx xx Xxxxxx$Xxxxxx xx xxx xxxxx$xx xxxxx$ $xx$.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx.

Xxx XxxxxXx xxxxxxxxx xxxxxxx xxxx xxx xxxxxxx xxx xxxxxx.
Xxxxxx xxxxx Xxxxxx$Xxxxxx xx xxxxx xxx xxxxxxx$ xxx Xxxx$Xxxxxx xx xxxx xxxx.

## XXXXXXX XXXXX

