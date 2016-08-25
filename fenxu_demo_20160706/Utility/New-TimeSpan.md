---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293994
schema: 2.0.0
---

# New-TimeSpan
## XXXXXXXX
Xxxxxxx x XxxxXxxx xxxxxx.

## XXXXXX

### Date (Default)
```
New-TimeSpan [[-Start] <DateTime>] [[-End] <DateTime>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### Time
```
New-TimeSpan [-Days <Int32>] [-Hours <Int32>] [-Minutes <Int32>] [-Seconds <Int32>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$XxxxXxxx xxxxxx xxxxxxx x XxxxXxxx xxxxxx xxxx xxxxxxxxxx x xxxx xxxxxxxx Xxx xxx xxx x XxxxXxxx xxxxxx xx xxx xx xxxxxxxx xxxx xxxx XxxxXxxx xxxxxxx.

Xxxxxxx xxxxxxxxxx$ x $Xxx$Xxxxxxxx$ xxxxxxx xxxxxxx x xxxxxxxx xxxxxx xxxx xxxxxxxxxx x xxxx xxxxxxxx xx xxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$timespan = new-timespan -hour 1 -minute 25
```

Xxxx xxxxxxx xxxxxxx x XxxxXxxx xxxxxx xxxx x xxxxxxxx xx 0 xxxx xxx 00 xxxxxxx xxx xxxxxx xx xx x xxxxxxxx xxxxx $xxxxxxxx.
Xx xxxxxxxx x xxxxxxxxxxxxxx xx xxx XxxxXxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>new-timespan -end (get-date -year 2010 -month 1 -day 1)
```

Xxxx xxxxxxx xxxxxxx x xxx XxxxXxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxxx xxxxxxx xxx xxxx xxxx xxx xxxxxxx xx xxx xxx Xxxxxxx 0$ 0000.

Xxxx xxxxxxx xxxx xxx xxxxxxx xxx Xxxxx xxxxxxxxx$ xxxxxxx xxx xxxxxxx xxxxx xx xxx Xxxxx xxxxxxxxx xx xxx xxxxxxx xxxx xxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$90days = new-timespan -days 90
PS C:\>(get-date) + $90days
```

Xxxxx xxxxxxxx xxxxxx xxx xxxx xxxx xx 00 xxxx xxxxx xxx xxxxxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>dir $pshome\en-us\about_remote.help.txt | new-timespan

Days              : 321
Hours             : 21
Minutes           : 59
Seconds           : 22
Milliseconds      : 312
Ticks             : 278135623127728
TotalDays         : 321.916230471907
TotalHours        : 7725.98953132578
TotalMinutes      : 463559.371879547
TotalSeconds      : 27813562.3127728
TotalMilliseconds : 27813562312.7728

# Equivalent to:

PS C:\>new-timespan -start (dir $pshome\en-us\about_remote.help.txt).lastwritetime
```

Xxxx xxxxxxx xxxxx xxx xxx xxxx xx xxx xxxx xxxxx xxx xxxxx$xxxxxx.xxxx.xxx xxxx xxx xxxx xxxxxxx.
Xxx xxx xxx xxxx xxxxxxx xxxxxx xx xxx xxxx$ xxx xx xxx xxxxx xxxxxx xxxx xxx x XxxxXxxxxXxxx xxxxxxxx.

Xxxx xxxxxxx xxxxx xxxxxxx xxx Xxxxx xxxxxxxxx xx Xxx$XxxxXxxx xxx xx xxxxx xx XxxxXxxxxXxxx.
Xxxx xxx xxxx xx xxxxxx xxxx xxx x XxxxXxxxxXxxx xxxxxxxx xx Xxx$XxxxXxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxx xx xxx XxxxXxxxxXxxx xxxxxxxx xx xxx xxxxx xx xxx Xxxxx xxxxxxxxx.

## XXXXXXXXXX

### -Days
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxx.
Xxx xxxxxxx xx 0.

```yaml
Type: Int32
Parameter Sets: Time
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -End
Xxxxxxxxx xxx xxx xx x xxxx xxxx.
Xxx xxxxxxx xx xxx xxxxxxx xxxx xxx xxxx.

```yaml
Type: DateTime
Parameter Sets: Date
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Hours
Xxxxxxxxx xxx xxxxx xx xxx xxxx xxxx.
Xxx xxxxxxx xx xxxx.

```yaml
Type: Int32
Parameter Sets: Time
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

### -Minutes
Xxxxxxxxx xxx xxxxxxx xx xxx xxxx xxxx.
Xxx xxxxxxx xx 0.

```yaml
Type: Int32
Parameter Sets: Time
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Seconds
Xxxxxxxxx xxx xxxxxx xx xxx xxxx xxxx xx xxxxxxx.
Xxx xxxxxxx xx 0.

```yaml
Type: Int32
Parameter Sets: Time
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Start
Xxxxxxxxx xxx xxxxx xx x xxxx xxxx.
Xxxxx x xxxxxx xxxx xxxxxxxxxx xxx xxxx xxx xxxx$ xxxx xx $0$00$00$ xx x XxxxXxxx xxxxxx$ xxxx xx xxx xxxx x Xxx$Xxxx xxxxxxx. Xxx xxxxxxx xx xxx xxxxxxx xxxx xxx xxxx.

Xxx xxx xxx Xxxxx xx xxx xxxxx$ XxxxXxxxxXxxx.
Xxx XxxxXxxxxXxxx xxxxx xxxx xxx xxxx xxxxxxx xxxx xxxx x XxxxXxxxxXxxx xxxxxxxx$ xxxx xx xxxxx xx xxx xxxx xxxxxx $Xxxxxx.Xx.XxxxXX$$ xx xxx Xxxxx xxxxxxxxx xx Xxx$XxxxXxxx.

```yaml
Type: DateTime
Parameter Sets: Date
Aliases: LastWriteTime

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

## XXXXXX

### System.DateTime
Xxx xxx xxxx x XxxxXxxx xxxxxx xxxx xxxxxxxxxx xxxx xxxxx xxxx xx Xxx$XxxxXxxx.

## XXXXXXX

### System.TimeSpan
Xxx$XxxxXxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxx xxxx.

## XXXXX

## XXXXXXX XXXXX

[Get-Date]()

[Set-Date]()

