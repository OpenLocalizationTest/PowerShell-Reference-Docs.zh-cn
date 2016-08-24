---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293961
schema: 2.0.0
---

# Xxxxxx$Xxxx
## XXXXXXXX
Xxxxxxx xxx xxxxxx xx x xxxx xx xxxxxxxxxx xx xxxxx xxxx xxxxxxxx xxxxxxx xx x xxx xxxx.

## XXXXXX

```
Format-List [[-Property] <Object[]>] [-GroupBy <Object>] [-View <String>] [-ShowError] [-DisplayError] [-Force]
 [-Expand <String>] [-InputObject <PSObject>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxxx xxxxxx xxxxxxx xxx xxxxxx xx x xxxxxxx xx x xxxx xx xxxxxxxxxx xx xxxxx xxxx xxxxxxxx xx xxxxxxxxx xx x xxxxxxxx xxxx.
Xxx xxx xxx Xxxxxx$Xxxx xx xxxxxx xxx xxxxxxx xxx xx xxxxxxxx xxxxxxxxxx xx xx xxxxxx xx x xxxx $xxxxxx$xxxx $$.

Xxxxxxx xxxx xxxxx xx xxxxxxxxx xxx xxxx xxxx xx x xxxx xxxx xx x xxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxxx xxxx xxxxxxxxxx xx xxx xxxxxx xx xxx xxxx$ xxx xxx xxxxxxxx xxxxxx xxx xxxx xxxxxx xx xx xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-service | format-list
```

Xxxx xxxxxxx xxxxxxx xxxxxxxxxxx xxxxx xxxxxxxx xx xxx xxxxxxxx xx x xxxx.
Xx xxxxxxx$ xxx xxxxxxxx xxx xxxxxxxxx xx x xxxxx.
Xxx Xxx$Xxxxxxx xxxxxx xxxx xxxxxxx xxxxxxxxxxxx xxx xxxxxxxx xx xxx xxxxxxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxxx xxx xxxxxxx xxxxxxx xxx xxxxxxxx xx Xxxxxx$Xxxx.
Xxxx$ xxx Xxxxxx$Xxxx xxxxxxx xxxxxxx xxx xxxxxxx xxxxxxxxxxx xx x xxxx xxx xxxxx xx xx xxx xxxxxxx xxxxxx xxxxxx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = get-childitem $pshome\*.ps1xml
PS C:\>format-list -InputObject $a
```

Xxxxx xxxxxxxx xxxxxxx xxxxxxxxxxx xxxxx xxx XX0XXX xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxx xx x xxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxxxxxxx xxx xxxxx xxx xxxxxx xxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx Xxxxxx$Xxxx xx xxxxxx xxxxxxxxxxx xxxxx xxxxxxx xxxxxx xx $x.
Xxxx xxxxxxx xxxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxx xxx xxxxxxxx xx Xxxxxx$Xxxx$ xxxxx xxxx xxxxx xxx xxxxxxxxx xxxxxx xx xxx xxxxxxx xxxxxx xxxxxx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | format-list -property name, basepriority, priorityclass
```

Xxxx xxxxxxx xxxxxxxx xxx xxxx$ xxxx xxxxxxxx$ xxx xxxxxxxx xxxxx xx xxxx xxxxxxx xx xxx xxxxxxxx.
Xx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xx xxxxxx xxxxxxxxxxxx xxxx xxxxxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxxx xxx xxxxxxx xxxxxxx xxxxxxx xxx xxxxxxxx xx Xxxxxx$Xxxx.
Xxxxxx$Xxxx xxxxxxx xxx xxxxxxxxx xx x xxxx xx xxx xxxxxxxxx xxxxxxxxxx.
Xxx $Xxxxxxxx$ xxxxxxxxx xxxx xx xxxxxxxx$ xx xxx xxx xxxx xx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process winlogon | format-list -property *
```

Xxxx xxxxxxx xxxxxxxx xxx xx xxx xxxxxxxxxx xx xxx Xxxxxxxx xxxxxxx.
Xx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xx xxxxxx xxxxxxxxxxxx xxx Xxxxxxxx xxxxxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxxx xxx Xxxxxxxx xxxxxxx xxxxxx xxxxxxx xxx xxxxxxxx xx Xxxxxx$Xxxx.
Xxx xxxxxxx xxxx xxx Xxxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxxxxxx xxx xxx $ xx xxxxxxxx xxx xxxxxxxxxx. Xxxxxxx xxx xxxx xx xxx Xxxxxxxx xxxxxxxxx xx xxxxxxxx$ xxx xxx xxxx xx xxx xxxx xxx xxxxxxx xx$ $xxxxxx$xxxx $$.
Xxxxxx$Xxxx xxxxxxxxxxxxx xxxxx xxx xxxxxxx xx xxx xxxxxxx xxxxxx xxxxxx xxx xxxxxxx.

## XXXXXXXXXX

### $XxxxxxxXxxxx
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
Xx xxxxxx x xxxxxxxxxx xxxxxxxx$ xxx x xxxx xxxxx.
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
XX $$ Xxx$Xxxx $ Xxxxxx$Xxxx XxxXxXxxx$$ $$ $ $xxxx $ $XxxxXxxxx XxxXxXxxx  $$ $ $xxxx
--------- ------------
Xxxxxxxxx $XXX

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
XX $$ Xxx$Xxxx $ Xxxxxx$Xxxx XxxXxXxxx$$ $$ $ $xxxx $ $XxxxXxxxx XxxXxXxxx  $$ $ $xxxx
--------- ------------
Xxxxxxxxx $XXX

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

$$ Xxxx $xx Xxxxx$ $$xxxxxx$$$$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxx xxxxx$$$$$ XxxxxxXxxxxx $$xxxxxx\>

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

### $Xxxx
Xxxxxxxxx xxx xxxx xx xx xxxxxxxxx xxxx xxxxxx xx $xxxx.$ Xxx xxxxxx xxx xxx Xxxxxxxx xxx Xxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

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
Xxx xxx xxxx xxx xxxxxx xx Xxxxxx$Xxxx.

## XXXXXXX

### Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.Xxxxxxxx.Xxxxxx
Xxxxxx$Xxxx xxxxxxx xxx xxxxxx xxxxxxx xxxx xxxxxxxxx xxx xxxx.

## XXXXX
Xxx xxx xxxx xxxxx xx Xxxxxx$Xxxx xx xxx xxxxx$xx xxxxx$ $XX$.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx.

Xxx xxxxxx xxxxxxx$ xxxx xx Xxxxxx$Xxxx$ xxxxxxx xxx xxxx xx xx xxxxxxxxx xxx xx xxx xxxxxxx xx.
Xxx xxxx xx xxxxxxxxx xx xxx xxxxxx xxxxxxxx xx Xxxxxxx XxxxxXxxxx xxx xx xxx xxxxxxx xxxx xxxxxxx xxx Xxx xxxx $xxx Xxx xxxxxxx$$ xxxx xx Xxx$Xxxx$ Xxx$Xxxx$ xxx Xxx$Xxxxxxx.

Xx xxx xx xxx xxx x xxxxxx xxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxx xxxx xxxxxxx xxxxxx xxx xxxx xxxxxx xxxx xx xxxxxxxx.

Xxx XxxxxXx xxxxxxxxx xxxxxxx xxxx xxx xxxxxxx xxx xxxxxx.
Xxxxxx xxxxx Xxxxxx$Xxxxxx xx xxxxx xxx xxxxxxx$ xxx Xxxx$Xxxxxx xx xxxx xxxx.

Xxx Xxxx xxxxxxxxx xxxx xxx xxxxxxx xx xxxxxxxxx xxxxxx xxx xxx xxxxx.
Xxx xxx xxx xxx xxxxx xxxxxxx xx xxx $.xxxxxx.XX0XXX xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxx$ xx xxx xxx xxxxxx xxxx xxx xxxxx xx xxx XX0XXX xxxxx xxx xxx xxx Xxxxxx$XxxxxxXxxx xxxxxx xx xxxxxxx xxxx xx Xxxxxxx XxxxxXxxxx.

Xxx xxxxxxxxx xxxx xxx xxx Xxxx xxxxxxxxx xxxx xxx xxx xxxx xxxxxx$ xx xxx$ xxx xxxxxxx xxxxx.
Xx xxx xxxxxxxxx xxxx xx x xxxxx$ xxx Xxxxxx$Xxxxx.
Xx xxx xxxxxxxxx xxxx xx xxxxxxx x xxxx xxx x xxxxx$ xxx Xxxxxx$Xxxxxx.

## XXXXXXX XXXXX

