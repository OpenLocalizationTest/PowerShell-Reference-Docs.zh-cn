---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294026
schema: 2.0.0
---

# Xxxx$Xxxxx
## XXXXXXXX
Xxxxx xxxxx x xxxxxxxxxx xxxxx xx xxxxxx xxxxxx xxxxxxxxxx xx xxx.

## XXXXXX

```
Wait-Event [[-SourceIdentifier] <String>] [-Timeout <Int32>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxx$Xxxxx xxxxxx xxxxxxxx xxxxxxxxx xx x xxxxxx xx xxxxxxxx xxxxx x xxxxxxxxxx xxxxx xx xxxxxx.
Xxxxxxxxx xxxxxxx xxxx xxx xxxxx xx xxxxxxxx.
Xx xxxxxx xxx xxxx$ xxxxx XXXX$X.

Xxxx xxxxxxx xxxxxxxx xx xxxxxxxxxxx xx xxxxxxx xxx xx xxxxx.
Xx xxxx xxxxxx xxx xx xxxxxxxxx xxx xxxxxxxx xx xx xxxxx xx xxx xxxxxxxxx xxxx$ xx xxxxx xxx Xxxxxx xxxxxxxxx xx xxx xxxxx xxxxxxxxxxxx xxx xx xxxxxxx xxx xx xxxxx xx xxxxxx xxx xxxx xxxxxxx xxxx xx xxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>wait-event
```

Xxxx xxxxxxx xxxxx xxx xxx xxxx xxxxx xxxx xx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>wait-event -sourceIdentifier "ProcessStarted"
```

Xxxx xxxxxxx xxxxx xxx xxx xxxx xxxxx xxxx xx xxxxxx xxx xxxx xxx x xxxxxx xxxxxxxxxx xx $XxxxxxxXxxxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$timer.Interval = 2000
PS C:\>$timer.Autoreset = $false
PS C:\>$timer.Enabled = $true; Wait-Event Timer.Elapsed

# After 2 seconds

EventIdentifier  : 12
Sender           : System.Timers.Timer
SourceEventArgs  : System.Timers.ElapsedEventArgs
SourceArgs       : {System.Timers.Timer, System.Timers.ElapsedEventArgs}
SourceIdentifier : Timer.Elapsed
TimeGenerated    : 6/10/2008 3:24:18 PM
MessageData      :
ForwardEvent     : False
```

Xxxx xxxxxxx xxxx xxx Xxxx$Xxxxx xxxxxx xx xxxx xxx x xxxxx xxxxx xx x xxxxx xxxx xx xxx xxx 0000 xxxxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>wait-event -sourceIdentifier "ProcessStarted" -timeout 90
```

Xxxx xxxxxxx xxxxx xx xx 00 xxxxxxx xxx xxx xxxx xxxxx xxxx xx xxxxxx xxx xxxx xxx x xxxxxx xxxxxxxxxx xx $XxxxxxxXxxxxxx$.
Xx xxx xxxxxxxxx xxxx xxxxxxx$ xxx xxxx xxxx.

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

### $XxxxxxXxxxxxxxxx
Xxxxx xxxx xxx xxxxxx xxxx xxx xxxxxxxxx xxxxxx xxxxxxxxxx.
Xx xxxxxxx$ Xxxx$Xxxxxx xxxxx xxx xxx xxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxx
Xxxxxxxxxx xxx xxxxxxx xxxx$ xx xxxxxxx$ xxxx Xxxx$Xxxxx xxxxx xxx xxx xxxxx xx xxxxx.
Xxx xxxxxxx$ $0$ xxxxx xxxxxxxxxxxx.
Xxx xxxxxx xxxxxx xxxx xxx xxxxxx xxx Xxxx$Xxxxx xxxxxxx.

Xx xxx xxxxxxxxx xxxx xx xxxxxxxx$ xxx xxxx xxxx xxx xxx xxxxxxx xxxxxx xxxxxxx$ xxxx xx xxx xxxxx xxx xxx xxxx xxxxxx.
Xx xxxxx xxxxxxx xx xxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: TimeoutSec

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxx

## XXXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxXxxx

## XXXXX
Xxxxxx$ xxxxx xxxxxxxxxxxxx$ xxx xxx xxxxx xxxxx xxxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxx xxxxx xxx xxxxxxx xxxxxxx$ xxx xxxxx xxxxx xx xxxxxxxxx xxx xxx xxxxx xxxxxxxxxxxx xx xxxxxxxx.

## XXXXXXX XXXXX

[Xxx$Xxxxx]()

[Xxx$XxxxxXxxxxxxxxx]()

[Xxx$Xxxxx]()

[Xxxxxxxx$XxxxxxXxxxx]()

[Xxxxxxxx$XxxxxxXxxxx]()

[Xxxxxxxx$XxxXxxxx]()

[Xxxxxx$Xxxxx]()

[Xxxxxxxxxx$Xxxxx]()

[Xxxx$Xxxxx]()

