---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293992
schema: 2.0.0
---

# Xxx$Xxxxx
## XXXXXXXX
Xxxxxxx x xxx xxxxx.

## XXXXXX

```
New-Event [-SourceIdentifier] <String> [[-Sender] <PSObject>] [[-EventArguments] <PSObject[]>]
 [[-MessageData] <PSObject>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxx xxxxxx xxxxxxx x xxx xxxxxx xxxxx.

Xxx xxx xxx xxxxxx xxxxxx xx xxxxxx xxxxx xxxxx xxxxx xxxxxxx xx xxxx xxxxxxx xxx xxx xxxxxx xxxx xxxx xxxxxxx xxx xxxxxx$ xxxxxxxxx xxxxxxxx xx xxxxxx xxxxxxxxxx$ xxxxxxxxxxx xxxxxx$ xxxx xxxxxx$ xxxxxxx xxxxxx$ xx xxx xxxxxxxxxx xx x xxxxxxxxxx xxx.

Xxxxxx xxxxxx xxx xxxxxxxxxxxxx xxxxx xx xxx xxxxx xxxxx xx xxxx xxxxxxx xxxxxxxx xxxx xxx xxxxxx$ xxx xx xxx xxxx xx xxxxxxxxx xx xxxx.
Xxxxxxx$ xx xxx xxxx xx xxxxxxx xx xxxxx xx xxx xxxxx xxxxxxx xx xxxxxxx xx xxxxxx xx xxxxxxx xx xxx xxxxx$ xxx xxx Xxxxxxxx$XxxxxxXxxxx xxxxxx xx xxxxxxxxx xx xxx xxxxxx xxxxx.

Xxxx xxx xxxxxxxxx xx x xxxxxx xxxxx$ xxx xxxxx xxxxxxxxxx xx xxxxx xx xxxx xxxxxxx.
Xx xxx xxxxxx xxx xxxxx xxxxxxxxxxxx xx xxxxx xxx Xxxxxxxxxx$Xxxxx xxxxxx$ xxx xxxxx xxxxxxxxxx xxx xxxxxx xxxxx xxx xxxxxxx xxxx xxx xxxxxxx.
Xx xxx xx xxx xxxxxxxxx xx xxx xxxxxx xxxxx$ xx xxxxxx xxx xxxxx$ xxx xxxx xxxxxx xxx xxxxxxx xxxxxxxxxx xx xxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>new-event -sourceidentifier Timer -sender windows.timer  -messagedata "Test"
```

Xxxx xxxxxxx xxxxxxx x xxx xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxx xxxxx.
Xx xxxx x Xxxxxxx.Xxxxx xxxxxx xx xxxx xxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>function Enable-ProcessCreationEvent
{
   $query = New-Object System.Management.WqlEventQuery "__InstanceCreationEvent", (New-Object TimeSpan 0,0,1), "TargetInstance isa 'Win32_Process'"
   $processWatcher = New-Object System.Management.ManagementEventWatcher $query
   $identifier = "WMI.ProcessCreated"
   Register-ObjectEvent $processWatcher "EventArrived" -SupportEvent $identifier -Action 
   {
      [void] (New-Event -sourceID "PowerShell.ProcessCreated" -Sender $args[0] -EventArguments $args[1].SourceEventArgs.NewEvent.TargetInstance)
   }
}
```

Xxxx xxxxxx xxxxxxxx xxxx xxx Xxx$Xxxxx xxxxxx xx xxxxx xx xxxxx xx xxxxxxxx xx xxxxxxx xxxxx.
Xxx xxxxxxx xxxx xxx Xxxxxxxx$XxxxxxXxxxx xxxxxx xx xxxxxxxxx xx xxx Xxxxxxx Xxxxxxxxxx Xxxxxxxxxxxxxxx $XXX$ xxxxx xxxx xx xxxxxx xxxx x xxx xxxxxxx xx xxxxxxx.
Xxx xxxxxxx xxxx xxx Xxxxxx xxxxxxxxx xx xxx xxxxxx xx xxxx xxx Xxx$Xxxxx xxxxxx$ xxxxx xxxxxxx xxx xxx xxxxx.

Xxxxxxx xxx xxxxxx xxxx Xxx$Xxxxx xxxxxx xxx xxxxxxxxxxxxx xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxx xxxxx$ xxx xx xxx xxxx xx xxxxxxxx xxx xxxx xxxxx.

## XXXXXXXXXX

### $XxxxxXxxxxxxxx
Xxxxxxxxx xx xxxxxx xxxx xxxxxxxx xxxxxxx xxx xxx xxxxx.

```yaml
Type: PSObject[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
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

### $XxxxxxxXxxx
Xxxxxxxxx xxxxxxxxxx xxxx xxxxxxxxxx xxxx xxx xxxxx.
Xxx xxxxx xx xxxx xxxxxxxxx xxxxxxx xx xxx XxxxxxxXxxx xxxxxxxx xx xxx xxxxx xxxxxx.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxx
Xxxxxxxxx xxx xxxxxx xxxx xxxxxx xxx xxxxx.
Xxx xxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxx.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXxxxxxxxxx
Xxxxxxxxx x xxxx xxx xxx xxx xxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx$ xxx xx xxxx xx xxxxxx xx xxx xxxxxxx.

Xxx xxxxx xx xxxx xxxxxxxxx xxxxxxx xx xxx XxxxxxXxxxxxxxxx xxxxxxxx xx xxx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxx
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxXxxx

## XXXXX
Xxx xxx xxxxxx xxxxx$ xxx xxxxx xxxxxxxxxxxx$ xxx xxx xxxxx xxxxx xxxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxx xxxxx xxx xxxxxxx xxxxxxx$ xxx xxxxx xxxxx xx xxxxxxxxx xxx xxx xxxxx xxxxxxxxxxxx xx xxxxxxxx.

## XXXXXXX XXXXX

[Xxx$Xxxxx]()

[Xxxxxxxx$XxxxxxXxxxx]()

[Xxxxxxxx$XxxxxxXxxxx]()

[Xxxxxxxx$XxxXxxxx]()

[Xxxxxx$Xxxxx]()

[Xxxxxxxxxx$Xxxxx]()

[Xxxx$Xxxxx]()

