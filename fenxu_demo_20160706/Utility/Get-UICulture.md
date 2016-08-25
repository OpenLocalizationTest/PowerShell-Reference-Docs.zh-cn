---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293977
schema: 2.0.0
---

# Get-UICulture
## XXXXXXXX
Xxxx xxx xxxxxxx xxxx xxxxxxxxx $XX$ xxxxxxx xxxxxxxx xx xxx xxxxxxxxx xxxxxx.

## XXXXXX

```
Get-UICulture [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$XXXxxxxxx xxxxxx xxxx xxxxxxxxxxx xxxxx xxx xxxxxxx XX xxxxxxx xxxxxxxx xxx Xxxxxxx.
Xxx XX xxxxxxx xxxxxxxxxx xxxxx xxxx xxxxxxx xxx xxxx xxx xxxx xxxxxxxxx xxxxxxxx$ xxxx xx xxxxx xxx xxxxxxxx.

Xxx xxx xxxx xxx xxx Xxx$Xxxxxxx xxxxxx$ xxxxx xxxx xxx xxxxxxx xxxxxxx xx xxx xxxxxx.
Xxx xxxxxxx xxxxxxxxxx xxx xxxxxxx xxxxxx xx xxxxx xxxx xx xxxxxxx$ xxxxxxxx$ xxx xxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-uiculture
```

Xxxx xxxxxxx xxxx xxx xxxxxxx XX xxxxxxx xxxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-uiculture | format-list *
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxx xx xxx xx xxx xxxxxxxxxx xx xxx xxxxxxx XX xxxxxxx xx x xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>(get-uiculture).calendar
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxx xxxxxx xxx xxx Xxxxxxxx xxxxxxxx xx xxx xxxxxxx XX xxxxxxx.
Xxxxxxxx xx xxxx xxx xxxxxxxx xx XX xxxxxxx.
Xx xxx xxx xx xxx xxxxxxxxxx$ xxxx $xxx$xxxxxxxxx $ xxx$xxxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>(get-uiculture).datetimeformat.shortdatepattern
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxx xxxx xxxxxxx xxx xxx xxxxxxx XX xxxxxxx.
Xx xxx xxx xx xxx xxxxxxxxxxxxx xx xxx XxxxXxxxXxxxxx xxxxxxxx xx xxx XX xxxxxxx$ xxxx $$xxx$xxxxxxxxx$.xxxxxxxxxxxxxx $ xx$.

## XXXXXXXXXX

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

## XXXXXX

### None
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### System.Globalization.CultureInfo, Microsoft.PowerShell.VistaCultureInfo
Xxx$XXXxxxxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxx XX xxxxxxx.
Xx Xxxxxxx XxxxxXxxxx 0.0$ xx xxxxxxx x XxxxxxxXxxx xxxxxx.
Xx Xxxxxxx XxxxxXxxxx 0.0$ xx xxxxxxx x XxxxxXxxxxxxXxxx xxxxxx.

## XXXXX
Xxx xxx xxxx xxx xxx $XxXxxxxxx xxx $XxXXXxxxxxx xxxxxxxxx.
Xxx $XxXxxxxxx xxxxxxxx xxxxxx xxx xxxx xx xxx xxxxxxx xxxxxxx$ xxx xxx $XxXXXxxxxxx xxxxxxxx xxxxxx xxx xxxx xx xxx xxxxxxx XX xxxxxxx.

## XXXXXXX XXXXX

