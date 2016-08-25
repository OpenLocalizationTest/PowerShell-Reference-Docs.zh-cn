---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294003
schema: 2.0.0
---

# Remove-Event
## XXXXXXXX
Xxxxxxx xxxxxx xxxx xxx xxxxx xxxxx.

## XXXXXX

### BySource (Default)
```
Remove-Event [-SourceIdentifier] <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### ByIdentifier
```
Remove-Event [-EventIdentifier] <Int32> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxxxx xxxxxx xxxxxxx xxxxxx xxxx xxx xxxxx xxxxx xx xxx xxxxxxx xxxxxxx.

Xxxx xxxxxx xxxxxxx xxxx xxx xxxxxx xxxxxxxxx xx xxx xxxxx.
Xx xxxxxx xxxxx xxxxxxxxxxxxx xx xxxxxxxxxxx$ xxx xxx Xxxxxxxxxx$Xxxxx xxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>remove-event -sourceIdentifier "ProcessStarted"
```

Xxxx xxxxxxx xxxxxxx xxxxxx xxxx x xxxxxx xxxxxxxxxx xx $Xxxxxxx Xxxxxxx$ xxxx xxx xxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>remove-event -eventIdentifier 30
```

Xxxx xxxxxxx xxxxxxx xxx xxxxx xxxx xx xxxxx XX xx 00 xxxx xxx xxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-event | remove-event
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxx xxxx xxx xxxxx xxxxx.

## XXXXXXXXXX

### -EventIdentifier
Xxxxxxx xxxx xxx xxxxx xxxx xxx xxxxxxxxx xxxxx xxxxxxxxxx.
Xx XxxxxXxxxxxxxxx xx XxxxxxXxxxxxxxxx xxxxxxxxx xx xxxxxxxx xx xxxxx xxxxxxx.

```yaml
Type: Int32
Parameter Sets: ByIdentifier
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
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

### -SourceIdentifier
Xxxxxxx xxxx xxx xxxxxx xxxx xxx xxxxxxxxx xxxxxx xxxxxxxxxx.
Xxxxxxxxx xxx xxx xxxxxxxxx.
Xx XxxxxXxxxxxxxxx xx XxxxxxXxxxxxxxxx xxxxxxxxx xx xxxxxxxx xx xxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: BySource
Aliases: 

Required: True
Position: 1
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

### System.Management.Automation.PSEventArgs
Xxx xxx xxxx xxxxxx xxxx Xxx$Xxxxx xx Xxxxxx$Xxxxx.

## XXXXXXX

### None
Xxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xxxxxx$ xxxxx xxxxxxxxxxxxx$ xxx xxx xxxxx xxxxx xxxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxx xxxxx xxx xxxxxxx xxxxxxx$ xxx xxxxx xxxxx xx xxxxxxxxx xxx xxx xxxxx xxxxxxxxxxxx xx xxxxxxxx.

## XXXXXXX XXXXX

[Get-Event]()

[New-Event]()

[Register-EngineEvent]()

[Register-ObjectEvent]()

[Register-WmiEvent]()

[Remove-Event]()

[Unregister-Event]()

[Wait-Event]()

