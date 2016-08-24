---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294022
schema: 2.0.0
---

# Xxxxxxxxxx$Xxxxx
## XXXXXXXX
Xxxxxxx xx xxxxx xxxxxxxxxxxx.

## XXXXXX

### XxXxxxxx $Xxxxxxx$
```
Unregister-Event [-SourceIdentifier] <String> [-Force] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### XxXx
```
Unregister-Event [-SubscriptionId] <Int32> [-Force] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxxxxxx$Xxxxx xxxxxx xxxxxxx xx xxxxx xxxxxxxxxxxx xxxx xxx xxxxxxx xx xxxxx xxx Xxxxxxxx$XxxxxxXxxxx$ Xxxxxxxx$XxxxxxXxxxx$ xx Xxxxxxxx$XxxXxxxx xxxxxx.

Xxxx xx xxxxx xxxxxxxxxxxx xx xxxxxxxx$ xxx xxxxx xxxxxxxxxx xx xxxxxxx xxxx xxx xxxxxxx xxx xxx xxxxxxxxxx xxxxxx xxx xx xxxxxx xxxxx xx xxx xxxxx xxxxx.
Xxxx xxx xxxxxx x xxxxxxxxxxxx xx xx xxxxx xxxxxxx xx xxxxx xxx Xxx$Xxxxx xxxxxx$ xxx xxx xxxxx xx xxxx xxxxxxx xxxx xxx xxxxxxx.

Xxxxxxxxxx$Xxxxx xxxx xxx xxxxxx xxxxxx xxxx xxx xxxxx xxxxx.
Xx xxxxxx xxxxxx$ xxx xxx Xxxxxx$Xxxxx xxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>unregister-event -sourceIdentifier ProcessStarted
```

Xxxx xxxxxxx xxxxxxx xxx xxxxx xxxxxxxxxxxx xxxx xxx x xxxxxx xxxxxxxxxx xx $XxxxxxxXxxxxxx$.

Xx xxxx xxx xxxxxx xxxxxxxxxx xx xx xxxxx$ xxx xxx Xxx$Xxxxx xxxxxx.
Xx xxxx xxx xxxxxx xxxxxxxxxx xx xx xxxxx xxxxxxxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>unregister-event -subscriptionId 2
```

Xxxx xxxxxxx xxxxxxx xxx xxxxx xxxxxxxxxxxx xxxx xxx x xxxxxxxxxxxx xxxxxxxxxx xx 0.

Xx xxxx xxx xxxxxxxxxxxx xxxxxxxxxx xx xx xxxxx xxxxxxxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-eventsubscriber -force | unregister-event -force
```

Xxxx xxxxxxx xxxxxxx xxx xxxxx xxxxxxxxxxxxx xx xxx xxxxxxx.

Xxx xxxxxxx xxxx xxx Xxx$XxxxxXxxxxxxxxx xxxxxx xx xxx xxx xxxxx xxxxxxxxxx xxxxxxx xx xxx xxxxxxx$ xxxxxxxxx xxx xxxxxxxxxxx xxxx xxx xxxxxx xx xxxxx xxx XxxxxxxXxxxx xxxxxxxxx xx xxx xxxxx xxxxxxxxxxxx xxxxxxx.

Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxxxxx xxxxxxx xx Xxxxxxxxxx$Xxxxx$ xxxxx xxxxxxx xxxx xxxx xxx xxxxxxx.
Xx xxxxxxxx xxx xxxx$ xxx Xxxxx xxxxxxxxx xx xxxx xxxxxxxx xx Xxxxxxxxxx$Xxxxx.

## XXXXXXXXXX

### $Xxxxx
Xxxxxxx xxx xxxxx xxxxxxxxxxxxx$ xxxxxxxxx xxxxxxxxxxxxx xxxx xxxx xxxxxx xx xxxxx xxx XxxxxxxXxxxx xxxxxxxxx xx Xxxxxxxx$XxxxxxXxxxx$ Xxxxxxxx$XxxXxxxx$ xxx Xxxxxxxx$XxxxxxXxxxx.

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
Xxxxxxx xxxxx xxxxxxxxxxxxx xxxx xxxx xxx xxxxxxxxx xxxxxx xxxxxxxxxx.

X XxxxxxXxxxxxxxxx xx XxxxxxxxxxxxXx xxxxxxxxx xxxx xx xxxxxxxx xx xxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: BySource
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxxxxxxxxXx
Xxxxxxx xxxxx xxxxxxxxxxxxx xxxx xxxx xxx xxxxxxxxx xxxxxxxxxxxx xxxxxxxxxx.

X XxxxxxXxxxxxxxxx xx XxxxxxxxxxxxXx xxxxxxxxx xxxx xx xxxxxxxx xx xxxxx xxxxxxx.

```yaml
Type: Int32
Parameter Sets: ById
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxx
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

### $XxxxXx
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

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxXxxxxxxxxx
Xxx xxx xxxx xxx xxxxxx xxxx Xxx$XxxxxXxxxxxxxxx xx Xxxxxxxxxx$Xxxxx.

## XXXXXXX

### Xxxx
Xxxx xxxxxx xxxx xxx xxxxxx xxx xxxxxx.

## XXXXX
Xxxxxx$ xxxxx xxxxxxxxxxxxx$ xxx xxx xxxxx xxxxx xxxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxx xxxxx xxx xxxxxxx xxxxxxx$ xxx xxxxx xxxxx xx xxxxxxxxx xxx xxx xxxxx xxxxxxxxxxxx xx xxxxxxxx.

Xxxxxxxxxx$Xxxxx xxxxxx xxxxxx xxxxxx xxxxxxx xx xxxxx xxx Xxx$Xxxxx xxxxxx xxxxxx xxx xxxx xxxxxxxxxx xx xxx xxxxx xx xxxxx xxx Xxxxxxxx$XxxxxxXxxxx xxxxxx.
Xx xxxxxx x xxxxxx xxxxx xxxx xxx xxxxxxx$ xxx xxxx xxxxxx xx xxxxxxxxxxxxxxxx xx xxxxx xxx xxxxxxx.

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

