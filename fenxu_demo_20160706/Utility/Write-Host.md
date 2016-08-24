---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294029
schema: 2.0.0
---

# Xxxxx$Xxxx
## XXXXXXXX
Xxxxxx xxxxxxxxxx xxxxxx xx x xxxx.

## XXXXXX

```
Write-Host [[-Object] <Object>] [-NoNewline] [-Separator <Object>] [-ForegroundColor <ConsoleColor>]
 [-BackgroundColor <ConsoleColor>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxx$Xxxx xxxxxx xxxxxxxxxx xxxxxx.
Xxx xxx xxxxxxx xxx xxxxx xx xxxx xx xxxxx xxx XxxxxxxxxxXxxxx xxxxxxxxx$ xxx xxx xxx xxxxxxx xxx xxxxxxxxxx xxxxx xx xxxxx xxx XxxxxxxxxxXxxxx xxxxxxxxx.
Xxx Xxxxxxxxx xxxxxxxxx xxxx xxx xxxxxxx x xxxxxx xx xxx xx xxxxxxxx xxxxxxxxx xxxxxxx.
Xxx xxxxxxxxxx xxxxxx xxxxxxx xx xxx xxxxxxx xxxx xx xxxxxxx Xxxxxxx XxxxxXxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>write-host "no newline test " -nonewline
no newline test PS C:\>
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxx xx xxx xxxxxxx$ xxx xxxxxxx xx xxx XxXxxxxxx xxxxxxxxx$ xxx xxxxxx xx xxxxxxxx xxxxxxxx xx xxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>write-host (2,4,6,8,10,12) -Separator ", +2= "
2, +2= 4, +2= 6, +2= 8, +2= 10, +2= 12
```

Xxxx xxxxxxx xxxxxxxx xxx xxxx xxxxxxx xxxx 0 xxxxxxx 00.
Xxx Xxxxxxxxx xxxxxxxxx xx xxxx xx xxx xxx xxxxxx $ $0$ $xxxxx$ xxxxx$ $$ 0$ $$ xxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>write-host (2,4,6,8,10,12) -Separator ", -> " -foregroundcolor DarkGreen -backgroundcolor white
```

Xxxx xxxxxxx xxxxxxxx xxx xxxx xxxxxxx xxxx 0 xxxxxxx 00.
Xx xxxx xxx XxxxxxxxxxXxxxx xxxxxxxxx xx xxxxxx xxxx xxxxx xxxx xxx xxx XxxxxxxxxxXxxxx xxxxxxxxx xx xxxxxxx x xxxxx xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>write-host "Red on white text." -ForegroundColor red -BackgroundColor white
Red on white text.
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxx $Xxx xx xxxxx xxxx.$ Xxx xxxx xx xxx$ xx xxxxxxx xx xxx XxxxxxxxxxXxxxx xxxxxxxxx.
Xxx xxxxxxxxxx xx xxxxx$ xx xxxxxxx xx xxx XxxxxxxxxxXxxxx xxxxxxxxx.

## XXXXXXXXXX

### $XxxxxxxxxxXxxxx
Xxxxxxxxx xxx xxxxxxxxxx xxxxx.
Xxxxx xx xx xxxxxxx.

```yaml
Type: ConsoleColor
Parameter Sets: (All)
Aliases: 
Accepted values: Black, DarkBlue, DarkGreen, DarkCyan, DarkRed, DarkMagenta, DarkYellow, Gray, DarkGray, Blue, Green, Cyan, Red, Magenta, Yellow, White

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxxXxxxx
Xxxxxxxxx xxx xxxx xxxxx.
Xxxxx xx xx xxxxxxx.

```yaml
Type: ConsoleColor
Parameter Sets: (All)
Aliases: 
Accepted values: Black, DarkBlue, DarkGreen, DarkCyan, DarkRed, DarkMagenta, DarkYellow, Gray, DarkGray, Blue, Green, Cyan, Red, Magenta, Yellow, White

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

### $XxXxxxxxx
Xxxxxxxxx xxxx xxx xxxxxxx xxxxxxxxx xx xxx xxxxxxx xxxx xxx xxx xxxx x xxxxxxx xxxxxxxxx.

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
Xxxxxxx xx xxxxxxx xx xxx xxxxxxx.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $Xxxxxxxxx
Xxxxxx xx xxx xxxxxx xxxxxxx xxxxxxx xxxxxxxxx xx xxx xxxxxxx.

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

## XXXXXX

### Xxxxxx.Xxxxxx
Xxx xxx xxxx xxxxxxx xx xx xxxxxxx xx xxx xxxx.

## XXXXXXX

### Xxxx
Xxxxx$Xxxx xxxxx xxx xxxxxxx xx xxx xxxx.
Xx xxxx xxx xxxxxx xxx xxxxxxx.
Xxxxxxx$ xxx xxxx xxxxx xxxxxxx xxx xxxxxxx xxxx Xxxxx$Xxxx xxxxx xx xx.

## XXXXX

## XXXXXXX XXXXX

[Xxxxx$Xxxx]()

[Xxx$Xxxx]()

[Xxxxx$Xxxxx]()

[Xxxxx$Xxxxx]()

[Xxxxx$Xxxxxx]()

[Xxxxx$Xxxxxxxx]()

[Xxxxx$Xxxxxxx]()

[Xxxxx$Xxxxxxx]()

