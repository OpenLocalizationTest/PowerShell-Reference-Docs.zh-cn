---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293963
schema: 2.0.0
---

# Format-Wide
## XXXXXXXX
Xxxxxxx xxxxxxx xx x xxxx xxxxx xxxx xxxxxxxx xxxx xxx xxxxxxxx xx xxxx xxxxxx.

## XXXXXX

```
Format-Wide [[-Property] <Object>] [-AutoSize] [-Column <Int32>] [-GroupBy <Object>] [-View <String>]
 [-ShowError] [-DisplayError] [-Force] [-Expand <String>] [-InputObject <PSObject>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxxx xxxxxx xxxxxxx xxxxxxx xx x xxxx xxxxx xxxx xxxxxxxx xxxx xxx xxxxxxxx xx xxxx xxxxxx.
Xxx xxx xxx xxx Xxxxxxxx xxxxxxxxx xx xxxxxxxxx xxxxx xxxxxxxx xx xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem | format-wide -column 3
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxx xx xxxxx xx xxx xxxxxxx xxxxxxxxx xx xxxxx xxxxxxx xxxxxx xxx xxxxxx.
Xxx Xxx$XxxxxXxxx xxxxxx xxxx xxxxxxx xxxxxxxxxxxx xxxx xxxx xx xxx xxxxxxxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxxx xxx xxxx xxxxxxx xxxxxxx xxx xxxxxxxx xx Xxxxxx$Xxxx$ xxxxx xxxxxxx xxxx xxx xxxxxx.
Xxx Xxxxxx xxxxxxxxx xxxxxxxxx xxx xxxxxx xx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem HKCU:\software\microsoft | format-wide -property pschildname -autosize
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxx xx xxxxxxxx xxxx xx xxx XXXX$XXXXXXX$XXXX$Xxxxxxxx$Xxxxxxxxx xxx.
Xxx Xxx$XxxxxXxxx xxxxxx xxxx xxxxxxx xxxxxxxxxxxx xxx xxxx.
Xxx xxxx xx xxxxxxxxx xx $XXXX$$$ xxx xx xxx xxxxxx xxxxxxx xx xxx Xxxxxxx XxxxxXxxxx Xxxxxxxx xxxxxxxx$ xxxxxxxx xx xxx xxx xxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxxx xxx xxxxxxxx xxx xxxxxxx xxxxxxx xxx xxxxxxxx xx Xxxxxx$Xxxx$ xxxxx xxxxxxx xxxx xxx xxxxxx.
Xxx Xxxxxxxx xxxxxxxxx xxxxxxxxx xxx xxxx xx xxx xxxxxxxx$ xxx xxx XxxxXxxx xxxxxxxxx xxxxxxx xxx xxxxxxx xxx xxxxxxxxxxx.

## XXXXXXXXXX

### -AutoSize
Xxxxxxx xxx xxxxxx xxxx xxx xxxxxx xx xxxxxxx xxxxx xx xxx xxxxx xx xxx xxxx.
Xx xxxxxxx$ xxx xxxxxx xxxx xxx xxxxxx xxx xxxxxxxxxx xx xxx xxxx.
Xxx xxxxxx xxx xxx XxxxXxxx xxx Xxxxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

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

### -Column
Xxxxxxxxx xxx xxxxxx xx xxxxxxx xx xxx xxxxxxx.
Xxx xxxxxx xxx xxx XxxxXxxx xxx Xxxxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

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

### -DisplayError
Xxxxxxxx xxxxxx xx xxx xxxxxxx xxxx.
Xxxx xxxxxxxxx xx xxxxxx xxxx$ xxx xxx xx xxxx xx x xxxxxxxxx xxx xxxx xxx xxx xxxxxxxxxx xxxxxxxxxxx xx x Xxxxxx$Xxxx xxxxxxx$ xxx xxx xxxxxxxxxxx xx xxx xxxxxx xx xx xxxxxxx.
Xxx xxxxxxxxx xxxxx xx xxxxxxx xx xxx xxxxxxx xx xxxxxx xxx XxxxxxxXxxxx xxxxxxxxx xxxx xx xxxxxxxxxx.

XX $$ Xxx$Xxxx $ Xxxxxx$Xxxx XxxXxXxxx$$ $$ $ $xxxx $ $XxxxXxxxx XxxXxXxxx  $$ $ $xxxx
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

### -Expand
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

### -Force
Xxxxxxxxx xxxxxxxxxxxx xxxx xxxxxxx xxx xxxxxxx xxxx xxxxxxxxxx$ xxxx xx xxx xxxxxxx xx xxx xxxxxxxxxx xxxxxxxx.
Xxx xxxxxxx$ Xxxxx xxxx xxxxxxxx xxx xxxx$xxxx xxxxxxxxx xx xxxxxx xxxxxxxxxxx xx xxxxxxxx x xxxx xxxx$ xxx xx xxxx xxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxxx.

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

### -GroupBy
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

### -InputObject
Xxxxxxxxx xxx xxxxxxx xx xx xxxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx$ xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.

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

### -Property
Xxxxxxxxx xxx xxxxxx xxxxxxxxxx xxxx xxxxxx xx xxx xxxxxxx xxx xxx xxxxx xx xxxxx xxxx xxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

Xx xxx xxxx xxxx xxxxxxxxx$ xxx xxxxxxxxxx xxxx xxxxxx xx xxx xxxxxxx xxxxxx xx xxx xxxxxx xxxxx xxxxxxxxx.
Xxx xxxxxxxxx xxxx $$Xxxxxxxx$$ xx xxxxxxxx.
Xxx xxxxxx xxx xxx Xxxxxxxx xxx Xxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

Xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx xxx xx x xxx xxxxxxxxxx xxxxxxxx.
Xx xxxxxx x xxxxxxxxxx$ xxxxxxxx$ xxx x xxxx xxxxx.
Xxxxx xxxx xxx$

$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxx xxxxx$$$$$ XxxxxxXxxxxx $$xxxxxx\>

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ShowError
Xxxxx xxxxxx xxxxxxx xxx xxxxxxxx.
Xxxx xxxxxxxxx xx xxxxxx xxxx$ xxx xxx xx xxxx xx x xxxxxxxxx xxx xxxx xxx xxx xxxxxxxxxx xxxxxxxxxxx xx x Xxxxxx$Xxxx xxxxxxx$ xxx xxx xxxxxxxxxxx xx xxx xxxxxx xx xx xxxxxxx.
Xxx xxxxxxxxx xxxxx xx xxxxxxx xx xxx xxxxxxx xx xxxxxx xxx XxxxXxxxx xxxxxxxxx xxxx xx xxxxxxxxxx.

XX $$ Xxx$Xxxx $ Xxxxxx$Xxxx XxxXxXxxx$$ $$ $ $xxxx $ $XxxxXxxxx XxxXxXxxx  $$ $ $xxxx
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

### -View
Xxxxxxxxx xxx xxxx xx xx xxxxxxxxx xxxxx xxxxxx xx $xxxx.$ Xxx xxxxxx xxx xxx Xxxxxxxx xxx Xxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

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

### System.Management.Automation.PSObject
Xxx xxx xxxx xxx xxxxxx xx Xxxxxx$Xxxx.

## XXXXXXX

### Microsoft.PowerShell.Commands.Internal.Format
Xxxxxx$Xxxx xxxxxxx xxxxxx xxxxxxx xxxx xxxxxxxxx xxx xxxxx.

## XXXXX
Xxx xxx xxxx xxxxx xx Xxxxxx$Xxxx xx xxx xxxxx$xx xxxxx$ $xx$.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx.
Xxx XxxxxXx xxxxxxxxx xxxxxxx xxxx xxx xxxxxxx xxx xxxxxx.
Xxxxxx xxxxx Xxxxxx$Xxxxxx xx xxxxx xxx xxxxxxx$ xxx Xxxx$Xxxxxx xx xxxx xxxx.
Xxx $Xxxx xxxxxxxxx xxxx xxx xxxxxxx xx xxxxxxxxx xxxxxx xxx xxx xxxxx.
Xxx xxx xxx xxx xxxxx xxxxxxx xx xxx $.xxxxxx.XX0XXX xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxx xx xxx xxx xxxxxx xxxx xxx xxxxx xx xxx XX0XXX xxxxx xxx xxx xxx Xxxxxx$XxxxxxXxxx xxxxxx xx xxxxxxx xxxx xx Xxxxxxx XxxxxXxxxx.
Xxx xxxxxxxxx xxxx xxx xxx Xxxx xxxxxxxxx xxxx xxx xxxxx xxxxxx$ xx xx xxxx xxx$ xxx xxxxxxx xxxxx.
Xx xxx xxxxxxxxx xxxx xx x xxxx$ xxx Xxxxxx$Xxxx.
Xx xxx xxxxxxxxx xxxx xx xxxxxxx x xxxx xxx x xxxxx$ xxx Xxxxxx$Xxxxxx.

## XXXXXXX XXXXX

