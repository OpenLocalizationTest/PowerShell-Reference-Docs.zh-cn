---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293978
schema: 2.0.0
---

# Xxx$Xxxxxx
## XXXXXXXX
Xxxxxxx xxxxxx xxxxx xxxx x xxxxxx xxxx.

## XXXXXX

### XxXxxxxx $Xxxxxxx$
```
Get-Unique [-InputObject <PSObject>] [-AsString] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### XxxxxxXxXxxx
```
Get-Unique [-InputObject <PSObject>] [-OnType] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxx xxxxxx xxxxxxxx xxxx xxxx xx x xxxxxx xxxx xx xxx xxxx xxxx$ xxxxxxxxxx xxxxxxxxxx$ xxx xxxxxxx xxxx xxx xxxxxxxx xx xxxx xxxx.
Xxx xxxx xxxx xx xxxxxx xxx xxx xxxxxx xx xxxx xxxxxxxx.

Xxx$Xxxxxx xx xxxx$xxxxxxxxx.
Xx x xxxxxx$ xxxxxxx xxxx xxxxxx xxxx xx xxxxxxxxx xxxxxx xxx xxxxxxxxxx xx xx xxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = $(foreach ($line in get-content C:\Test1\File1.txt) {$line.tolower().split(" ")}) | sort | get-unique
PS C:\>$a.count
```

Xxxxx xxxxxxxx xxxx xxx xxxxxx xx xxxxxx xxxxx xx x xxxx xxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxx xx xxx Xxxx.xxx xxxx.
Xx xxxxxxxx xxxx xxxx xx xxxx xx xxxxxxxxx xxxxxxx xxx xxxx xxxxxx xxxx xxxx xxxx x xxxxxxxx xxxx xx xxx xxxxx $$ $$.
Xxxx$ xx xxxxx xxx xxxxxxxxx xxxx xxxxxxxxxxxxxx $xxx xxxxxxx$ xxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxxxxxxxx xxx xxxxxxxxx xxxxx.
Xxx xxxxxxx xxx xxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxx xxxxxxxx xx xxx xxxxxxxxxx xx xxxxxxx xx $x xx xxxxxxxxx xxx xxxx xxxxx xxx xx $x.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>1,1,1,1,12,23,4,5,4643,5,3,3,3,3,3,3,3 | sort-object | Get-Unique
```

Xxxx xxxxxxx xxxxx xxx xxxxxx xxxxxxx xx xxx xxx xx xxxxxxxx.
Xxx xxxxx xxxxxxx xxxxx xx xxxxx xx xxxxxxxx xxxxx xx xxx xxxxxxx xxxx$ xxxxx xxxx xx xxx Xxxx$Xxxxxx xxxxxx xx xx xxxxxx$ xxx xxxx xxxxx xxxx xx Xxx$Xxxxxx$ xxxxx xxxxxxxxxx xxxxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem | sort-object {$_.GetType()} |  unique -OnType
```

Xxxx xxxxxxx xxxx xxx Xxx$XxxxxXxxx xxxxxx xx xxxxxxxx xxx xxxxxxxx xx xxx xxxxx xxxxxxxxx$ xxxxx xxxxxxxx xxxxx xxx xxxxxxxxxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxx xxx xxxxxxx xx xxx Xxxx$Xxxxxx xxxxxx.
Xxx $$$.XxxXxxx$$$ xxxxxxxxx xxxxxxx xxx XxxXxxx xxxxxx xx xxxx xxxx xx xxxxxxxxx.
Xxxx$ Xxxx$Xxxxxx xxxxx xxx xxxxx xx xxxx.
Xxxxxxx xxxxxxxx xxxxxxxx xxxxx xxx xxxxxxx xx Xxx$Xxxxxx.
Xxx XxXxxx xxxxxxxxx xxxxxxx Xxx$Xxxxxx xx xxxxxx xxxx xxx xxxxxx xx xxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | sort-object | select processname | get-unique -asstring
```

Xxxx xxxxxxx xxxx xxx xxxxx xx xxxxxxxxx xxxxxxx xx xxx xxxxxxxx xxxx xxxxxxxxxx xxxxxxxxxx.

Xxx Xxx$Xxxxxxx xxxxxxx xxxx xxx xx xxx xxxxxxxxx xx xxx xxxxxxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxxx xxx xxxxxx xx Xxxx$Xxxxxx$ xxxxx$ xx xxxxxxx$ xxxxx xxx xxxxxxxxx xxxxxxxxxxxxxx xx XxxxxxxXxxx.
Xxx xxxxxxx xxx xxxxx xx xxx Xxxxxx$Xxxxxx xxxxxx$ xxxxx xxxxxxx xxxx xxx xxxxxx xx xxx XxxxxxxXxxx xxxxxxxx xx xxxx xxxxxx.
Xxx xxxxxxx xxx xxxx xxxxx xx Xxx$Xxxxxx xx xxxxxxxxx xxxxxxxxxx.

Xxx XxXxxxxx xxxxxxxxx xxxxx Xxx$Xxxxxx xx xxxxx xxx XxxxxxxXxxx xxxxxx xx xxxxxxx.
Xxxxxxx xxxx xxxxxxxxx$ Xxx$Xxxxxx xxxxxx xxx XxxxxxxXxxx xxxxxx xx xxxxxxx xxx xxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxxx$ xxxx xx$ xxx xxxxx xxxxxxx xxxx xx xxx xxxx.

## XXXXXXXXXX

### $XxXxxxxx
Xxxxxx xxx xxxx xx x xxxxxx.
Xxxxxxx xxxx xxxxxxxxx$ xxxx xx xxxxxxx xx xx xxxxxx$ xx xxxx xxx xxxxxx x xxxxxxxxxx xx xxxxxxx xx xxx xxxx xxxx xx Xxx$Xxxxxx$ xxxx xx x xxxxxxxxxx xx xxxxx$ xx xxxxxxx xxxx xxx $xxx xxxxx$.
Xxx xxx xxx xxxx xxxxxxxxx xx xxxx xxx xxxxxx xxxxxx xx xxxxxx xxxxxxxxxx$ xxxx xx xxx xxxx xxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: AsString
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
Xxxxxxx xxxxx xxx Xxx$Xxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.

Xxx$Xxxxxx xxxxxx xxx xxxxx xxxxxxxxx xx xxxxx XxxxxXxxxxx xx x xxxxxxxxxx$ xx xxxx xxx xxxxxxxxx xxxxxxxxxx xxxxx xx xxx xxxxxxxxxx.
Xxxxxxx xxx xxxxxxxxxx xx x xxxxxx xxxx$ xxxxx xxxxxxxxx xx xxxxx XxxxxXxxxxx xx xxxxxx xxxxxxxx xxxxxxxxx.

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

### $XxXxxx
Xxxxxxx xxxx xxx xxxxxx xx xxxx xxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UniqueByType
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxx xxxx xxx xxxx xx xxxxxx xx Xxx$Xxxxxx.

## XXXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxxx xx xxxxxx xxxx Xxx$Xxxxxx xxxxxxx xx xxxxxxxxxx xx xxx xxxxx.

## XXXXX
Xxx xxx xxxx xxxxx xx Xxx$Xxxxxx xx xxx xxxxx$xx xxxxx$ $xx$.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx.

Xx xxxx x xxxx$ xxx Xxxx$Xxxxxx.
Xxx xxx xxxx xxx xxx Xxxxxx xxxxxxxxx xx Xxxx$Xxxxxx xx xxxx xxx xxxxxx xxxxx xx x xxxx.

## XXXXXXX XXXXX

[Xxxxxx$Xxxxxx]()

[Xxxx$Xxxxxx]()

