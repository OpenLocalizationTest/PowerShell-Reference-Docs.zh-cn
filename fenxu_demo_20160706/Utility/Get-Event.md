---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293967
schema: 2.0.0
---

# Xxx$Xxxxx
## XXXXXXXX
Xxxx xxx xxxxxx xx xxx xxxxx xxxxx.

## XXXXXX

### XxXxxxxx $Xxxxxxx$
```
Get-Event [[-SourceIdentifier] <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### XxXx
```
Get-Event [-EventIdentifier] <Int32> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxx xxxxxx xxxx xxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxx xxxxx xxx xxx xxxxxxx xxxxxxx.
Xxx xxx xxx xxx xxxxxx xx xxx xxx XxxxxXxxxxxxxxx xx XxxxxxXxxxxxxxxx xxxxxxxxxx xx xxxxxxx xxx xxxxxx.

Xxxx xx xxxxx xxxxxx$ xx xx xxxxx xx xxx xxxxx xxxxx.
Xxx xxxxx xxxxx xxxxxxxx xxxxxx xxx xxxxx xxx xxxx xxxxxxxxxx$ xxxxxx xxxxxxx xx xxxxx xxx Xxx$Xxxxx xxxxxx$ xxx xxx xxxxx xxxx xx xxxxxx xxxx Xxxxxxx XxxxxXxxxx xxxxx.
Xxx xxx xxx Xxx$Xxxxx xx Xxxx$Xxxxx xx xxx xxx xxxxxx.

Xxxx xxxxxx xxxx xxx xxx xxxxxx xxxx xxx Xxxxx Xxxxxx xxxx.
Xx xxx xxxxx xxxxxx$ xxx Xxx$XxxXxxxx xx Xxx$XxxxxXxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-event
```

Xxxx xxxxxxx xxxx xxx xxxxxx xx xxx xxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-event -sourceIdentifier "PowerShell.ProcessCreated"
```

Xxxx xxxxxxx xxxx xxxxxx xx xxxxx xxx xxxxx xx xxx XxxxxxXxxxxxxxxx xxxxxxxx xx $XxxxxXxxxx.XxxxxxxXxxxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$events = get-event
PS C:\>$events[0] | format-list -property *

ComputerName     :
RunspaceId       : c2153740-256d-46c0-a57c-b805917d1b7b
EventIdentifier  : 1
Sender           : System.Management.ManagementEventWatcher
SourceEventArgs  : System.Management.EventArrivedEventArgs
SourceArgs       : {System.Management.ManagementEventWatcher, System.Management.EventArrivedEventArgs}
SourceIdentifier : ProcessStarted
TimeGenerated    : 11/13/2008 12:09:32 PM
MessageData      :

PS C:\>get-event | where {$_.TimeGenerated -ge "11/13/2008 12:15:00 PM"}

ComputerName     :
RunspaceId       : c2153740-256d-46c0-a57c-b8059325d1a0
EventIdentifier  : 1
Sender           : System.Management.ManagementEventWatcher
SourceEventArgs  : System.Management.EventArrivedEventArgs
SourceArgs       : {System.Management.ManagementEventWatcher, System.Management.EventArrivedEventArgs}
SourceIdentifier : ProcessStarted
TimeGenerated    : 11/13/2008 12:15:00 PM
MessageData      :
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxxxxx xx xxxxx xxxxxxxxxx xxxxx xxxx XxxxxxXxxxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxx xx xxx xxxxx xxxxx xxx xxxxx xxxx xx xxx $xxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxxxx xxxxxxxx xx xxx xxx xxxxx $0$xxxxx$ xxxxx xx xxx xxxxx xx xxx $xxxxxx xxxxxxxx.
Xxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxx xx xxx Xxxxxx$Xxxx xxxxxxx$ xxxxx xxxxxxxx xxx xxxxxxxxxx xx xxx xxxxx xx x xxxx.
Xxxx xxxxxx xxx xx xxxxxxx xxx xxxxxxxxxx xx xxx xxxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxxx xxx xx xxx xxx Xxxxx$Xxxxxx xxxxxx xx xxx xx xxxxx

xxxxx xx xxx xxxx xxxx xx xxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-event -eventIdentifier 2
```

Xxxx xxxxxxx xxxx xxx xxxxx xxxx xx xxxxx xxxxxxxxxx xx 0.

## XXXXXXXXXX

### $XxxxxXxxxxxxxxx
Xxxx xxxx xxx xxxxxx xxxx xxx xxxxxxxxx xxxxx xxxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: ById
Aliases: Id

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

### $XxxxxxXxxxxxxxxx
Xxxx xxxx xxxxxx xxxx xxx xxxxxxxxx xxxxxx xxxxxxxxxx.
Xxx xxxxxxx xx xxx xxxxxx xx xxx xxxxx xxxxx.
Xxxxxxxxx xxx xxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: BySource
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

### Xxxx
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxXxxx
Xxx$Xxxxx xxxxxxx x XXXxxxxXxxx xxxxxx xxx xxxx xxxxx.
Xx xxx x xxxxxxxxxxx xx xxxx xxxxxx$ xxxx $xxx$xxxx xxx$xxxxx $xxxx$ xxx xxx xxx Xxxxx xxxxxxx xx xxx xxxx xxxxx.

## XXXXX
Xxxxxx$ xxxxx xxxxxxxxxxxxx$ xxx xxx xxxxx xxxxx xxxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxx xxxxx xxx xxxxxxx xxxxxxx$ xxx xxxxx xxxxx xx xxxxxxxxx xxx xxx xxxxx xxxxxxxxxxxx xx xxxxxxxx.

Xxx Xxx$Xxxxx xxxxxx xxxxxxx x XXXxxxxXxxx xxxxxx $Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxXxxx$ xxxx xxx xxxxxxxxx xxxxxxxxxx.

$$ XxxxxxxxXxxx$  Xxx xxxx xx xxx xxxxxxxx xx xxxxx xxx xxxxx xxxxxxxx. Xxxx xxxxxxxx xxxxx xx xxxxxxxxx xxxx xxxx xxx xxxxx xx xxxxxxxxx xxxx x xxxxxx xxxxxxxx.
$$ XxxxxxxxXx$  X XXXX xxxx xxxxxxxx xxxxxxxxxx xxx xxxxxxx xx xxxxx xxx xxxxx xxxxxxxx. Xxxx xxxxxxxx xxxxx xx xxxxxxxxx xxxx xxxx xxx xxxxx xx xxxxxxxxx xxxx x xxxxxx xxxxxxxx.
$$ XxxxxXxxxxxxxxx$ Xx xxxxxxx $Xxx00$ xxxx xxxxxxxx xxxxxxxxxx xxx xxxxx xxxxxxxxxxxx xx xxx xxxxxxx xxxxxxx.
$$ Xxxxxx$ Xxx xxxxxx xxxx xxxxxxxxx xxx xxxxx. Xx xxx xxxxx xx xxx Xxxxxx xxxxxxxxx$ xxx $Xxxxxx xxxxxxxxx xxxxxxxx xxxxxxxx xxx xxxxxx xxxxxx.
$$ XxxxxxXxxxxXxxx$ Xxx xxxxx xxxxxxxxx xxxx xxxxxxx xxxx XxxxxXxxx$ xx xx xxxxxx. Xxx xxxxxxx$ xx x xxxxx xxxxxxx xxxxx xx xxxxx xxx xxxxxxxxx xxx xxx xxxx $Xxxxxx xxxxxx$ Xxxxxx.XxxxxxxXxxxxXxxx x$$ xxx XxxxxxXxxxxXxxx xxxxxxxx xxxxx xxxxxxx xxx Xxxxxx.XxxxxxxXxxxxXxxx. Xx xxx xxxxx xx xxx Xxxxxx xxxxxxxxx$ xxx $XxxxxXxxx xxxxxxxxx xxxxxxxx xxxxxxxx xxxx xxxxx.
$$ XxxxxxXxxx$ Xxx xxxxxxxxxx xx xxx xxxxxxxx xxxxx xxxxxxxxx. Xxx x xxxxxxxx xxxxx xxxxxxxxx$ $Xxxx$$0$$ xxxxxxxxxx xxx xxxxxx$ xxx $Xxxx$$0$$ xxxxxxxxxx xxx XxxxxxXxxxxXxxx. Xx xxx xxxxx xx xxx Xxxxxx xxxxxxxxx$ xxx $Xxxx xxxxxxxxx xxxxxxxx xxxxxxxx xxxx xxxxx.
$$ XxxxxxXxxxxxxxxx$  X xxxxxx xxxx xxxxxxxxxx xxx xxxxx xxxxxxxxxxxx. Xx xxx xxxxx xx xxx Xxxxxx xxxxxxxxx$ xxx XxxxxxXxxxxxxxxx xxxxxxxx xx xxx $Xxxxx xxxxxxxxx xxxxxxxx xxxxxxxx xxxx xxxxx.
$$ XxxxXxxxxxxxx$ X XxxxXxxx xxxxxx xxxx xxxxxxxxxx xxx xxxx xx xxxxx xxx xxxxx xxx xxxxxxxxx. Xx xxx xxxxx xx xxx Xxxxxx xxxxxxxxx$ xxx XxxxXxxxxxxxx xxxxxxxx xx xxx $Xxxxx xxxxxxxxx xxxxxxxx xxxxxxxx xxxx xxxxx.
$$XxxxxxxXxxx$ Xxxx xxxxxxxxxx xxxx xxx xxxxx xxxxxxxxxxxx. Xxxxx xxxxxxx xxxx xxxx xxxx xxxx xxxxxxxx xx xxxxx. Xx xxx xxxxx xx xxx Xxxxxx xxxxxxxxx$ xxx XxxxxxxXxxx xxxxxxxx xx xxx $Xxxxx xxxxxxxxx xxxxxxxx xxxxxxxx xxxx xxxxx.

## XXXXXXX XXXXX

[Xxx$Xxxxx]()

[Xxxxxxxx$XxxxxxXxxxx]()

[Xxxxxxxx$XxxxxxXxxxx]()

[Xxxxxxxx$XxxXxxxx]()

[Xxxxxx$Xxxxx]()

[Xxxxxxxxxx$Xxxxx]()

[Xxxx$Xxxxx]()

