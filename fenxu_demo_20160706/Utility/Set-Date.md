---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294012
schema: 2.0.0
---

# Set-Date
## XXXXXXXX
Xxxxxxx xxx xxxxxx xxxx xx xxx xxxxxxxx xx x xxxx xxxx xxx xxxxxxx.

## XXXXXX

### Date (Default)
```
Set-Date [-Date] <DateTime> [-DisplayHint <DisplayHintType>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### Adjust
```
Set-Date [-Adjust] <TimeSpan> [-DisplayHint <DisplayHintType>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxx xxxxxx xxxxxxx xxx xxxxxx xxxx xxx xxxx xx xxx xxxxxxxx xx x xxxx xxx xxxx xxxx xxx xxxxxxx.
Xxx xxx xxxxxxx x xxx xxxx xxx$xx xxxx xx xxxxxx x xxxxxx xx xx xxxxxxx x XxxxXxxx xx XxxxXxxx xxxxxx xx Xxx$Xxxx.
Xx xxxxxxx x xxx xxxx xx xxxx$ xxx xxx Xxxx xxxxxxxxx.
Xx xxxxxxx x xxxxxx xxxxxxxx$ xxx xxx Xxxxxx xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Set-Date -Date (Get-Date).AddDays(3)
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxx xxxxx xxxx xx xxx xxxxxxx xxxxxx xxxx.
Xx xxxx xxx xxxxxx xxx xxxx.
Xxx xxxxxxx xxxx xxx Xxxx xxxxxxxxx xx xxxxxxx xxx xxxx.
Xx xxxx xxx Xxx$Xxxx xxxxxx xx xxx xxx xxxxxxx xxxx xxx xxxx xxx xxxxxxx xxx XxxXxxx .XXX xxxxxx xxx XxxxXxxx xxxxxxx xxxx x xxxxx xx 0 $xxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-date -adjust -0:10:0 -displayHint time
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxx xxx xxxxxxx xxxxxx xxxx xxxx xx 00 xxxxxxx.
Xx xxxx xxx Xxxxxx xxxxxxxxx xx xxxxxxx xx xxxxxxxx xx xxxxxx xxx xxx xxxx xxxxxx $xxxxx xxx xxxxxxx$ xx xxxxxxxx xxxx xxxxxx xxx xxx xxxxxx.
Xxx XxxxxxxXxxx xxxxxxxxx xxxxx Xxxxxxx XxxxxXxxxx xx xxxxxxx xxxx xxx xxxx$ xxx xx xxxx xxx xxxxxx xxx XxxxXxxx xxxxxx xxxx Xxx$Xxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$t = get-date
PS C:\>set-date -date $t
```

Xxxxxxxxxxx

-----------

Xxxxx xxxxxxxx xxxxxx xxx xxxxxx xxxx xxx xxxx xx xxx xxxxxxxx xx xxx xxxx xxx xxxx xxxxx xx xxx xxxxxxxx $x.
Xxx xxxxx xxxxxxx xxxx xxx xxxx xxx xxxxxx xx xx $x.
Xxx xxxxxx xxxxxxx xxxx xxx Xxxx xxxxxxxxx xx xxxx xxx XxxxXxxx xxxxxx xx $x xx xxx Xxx$Xxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$90mins = new-timespan -minutes 90
PS C:\>set-date -adjust $90mins
```

Xxxxxxxxxxx

-----------

Xxxxx xxxxxxxx xxxxxxx xxx xxxxxx xxxx xx xxx xxxxx xxxxxxxx xx 00 xxxxxxx.
Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxxx xxxxxx xx xxxxxx x XxxxXxxx xxxxxx xxxx x 00$xxxxxx xxxxxxxx$ xxx xxxx xx xxxxx xxx XxxxXxxx xxxxxx xx xxx $00xxxx xxxxxxxx.
Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx xxxxxxxxx xx Xxx$Xxxx xx xxxxxx xxx xxxx xx xxx xxxxx xx xxx XxxxXxxx xxxxxx xx xxx $00xxxx xxxxxxxx.

## XXXXXXXXXX

### -Adjust
Xxxx xx xxxxxxxxx xxx xxxxxxxxx xxxxx xxxx xxx xxxxxxx xxxx xxx xxxx.
Xxx xxx xxxx xx xxxxxxxxxx xx xxxxxxxx xxxx xxx xxxx xxxxxx xxx xxxx xxxxxx xx xxx xxx Xxxxxx xxxxxxxxx xx xxxx x XxxxXxxx xxxxxx xxxx Xxx$XxxxXxxx xx Xxx$Xxxx.

```yaml
Type: TimeSpan
Parameter Sets: Adjust
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Date
Xxxxxxx xxx xxxx xxx xxxx xx xxx xxxxxxxxx xxxxxx.
Xxx xxx xxxx x xxx xxxx xx xxx xxxxx xxxx xxxxxx xxx x xxxx xx xxx xxxxxxxx xxxx xxxxxx xxx xxxx xxxxxx.
Xx$ xxx xxx xxxx x Xxxx$Xxxx xxxxxx xxxx Xxx$Xxxx.

Xx xxx xxxxxxx x xxxx$ xxx xxx x xxxx$ Xxx$Xxxx xxxxxxx xxx xxxx xx xxxxxxxx xx xxx xxxxxxxxx xxxx.
Xx xxx xxxxxxx xxxx x xxxx$ xx xxxx xxx xxxxxx xxx xxxx.

```yaml
Type: DateTime
Parameter Sets: Date
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -DisplayHint
Xxxxxxxxxx xxxxx xxxxxxxx xx xxx xxxx xxx xxxx xxx xxxxxxxxx.

Xxxxx xxxxxx xxx$

$$ xxxx$ xxxxxxxx xxxx xxx xxxx $$ xxxx$ xxxxxxxx xxxx xxx xxxx $$ xxxxxxxx$ xxxxxxxx xxx xxxx xxx xxxx

Xxxx xxxxxxxxx xxxxxxx xxxx xxx xxxxxxx.
Xx xxxx xxx xxxxxx xxx XxxxXxxx xxxxxx xxxx Xxx$Xxxx xxxxxxxxx.

```yaml
Type: DisplayHintType
Parameter Sets: (All)
Aliases: 
Accepted values: Date, Time, DateTime

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

### System.DateTime
Xxx xxx xxxx x xxxx xx Xxx$Xxxx.

## XXXXXXX

### System.DateTime
Xxx$Xxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxx xxxx xx xxx.

## XXXXX
Xxx xxxx xxxxxx xxxxxxxxxx.
Xxxxxxxx xxx xxxx xxx xxxx xx xxx xxxxxxxx.
Xxx xxxxxx xxxxx xxxxxxx xxx xxxxxxxx xxxx xxxxxxxxx xxxxxx$xxxx xxxxxx xxx xxxxxxx xxxx xxx xxxxxxxxx xx x xxxx xx xxxx.
Xxx xxx $XxxxXx xxx $Xxxxxxx xxxxxxxxxx xx xxxxx xxxxxx.

Xxx xxx xxx xxxxxxxx .XXX xxxxxxx xxxx xxx XxxxXxxx xxx XxxxXxxx xxxxxxx xxxx xxxx Xxx$Xxxx$ xxxx xx XxxXxxx$ XxxXxxxxx xxx XxxxXxxxXxxx.
Xxx xxxx xxxxxxxxxxx$ xxx $XxxxXxxx Xxxxxxx$ xxx $XxxxXxxx Xxxxxxx.$

## XXXXXXX XXXXX

[Get-Date]()

[New-TimeSpan]()

