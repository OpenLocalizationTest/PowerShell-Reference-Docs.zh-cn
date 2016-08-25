---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294001
schema: 2.0.0
---

# Register-EngineEvent
## XXXXXXXX
Xxxxxxxxxx xx xxxxxx xxxx xxx xxxxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxx xxx xx xxx Xxx$Xxxxx xxxxxx.

## XXXXXX

```
Register-EngineEvent [-SourceIdentifier] <String> [[-Action] <ScriptBlock>] [-MessageData <PSObject>]
 [-SupportEvent] [-Forward] [-MaxTriggerCount <Int32>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxxxx$XxxxxxXxxxx xxxxxx xxxxxxxxxx xx xxxxxx xxxx xxx xxxxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxx xxx xxx Xxx$Xxxxx xxxxxx.
Xxx xxx XxxxxxXxxxxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxx.

Xxx xxx xxx xxxx xxxxxx xx xxxxxxxxx xx xxx $Xxxxxxx$ xxxxxx xxxxx xxx xxxxxx xxxxxxxxx xx xxx Xxx$Xxxxx xxxxxx.
Xxxxx xxxxxx xxx xxxxxxxxxxxxx xxxxx xx xxxx xxxxx xxxxx xx xxxx xxxxxxx xxxxxxx xxxxxxxxxxx.
Xxxxxxx$ xxxxxxxxxxx xxxx xxx xxxxxxx xxx xxxxxx$ xxxxxxx xx xxxxxx xx xxxxxxx xx xxx xxxxxx$ xxx xxxxxx xxx xxxxxxxxxxxx.

Xxxx xxx xxxxxxxxxx xxxxx xx xxxxxx$ xx xx xxxxx xx xxx xxxxx xxxxx xx xxxx xxxxxxx.
Xx xxx xxxxxx xx xxx xxxxx xxxxx$ xxx xxx Xxx$Xxxxx xxxxxx.

Xxxx xxx xxxxxxxxx xx x xxxxx$ xx xxxxx xxxxxxxxx xx xxxxx xx xxxx xxxxxxx.
Xx xxx xxx xxxxx xxxxxxxxxxx xx xxx xxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxxxx xxxxxx.
Xx xxxxxx xxx xxxxxxxxxxxx$ xxx xxx Xxxxxxxxxx$Xxxxx xxxxxx$ xxxxx xxxxxxx xxx xxxxx xxxxxxxxxx xxxx xxx xxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$s = New-PSSession -ComputerName Server01, Server02
PS C:\>Invoke-Command -Session $s { Register-EngineEvent -SourceIdentifier ([System.Management.Automation.PsEngineEvent]::Exiting) -Forward }
```

Xxxx xxxxxxx xxxxxxxxx xxx x Xxxxxxx XxxxxXxxxx xxxxxx xxxxx xx xxx xxxxxx xxxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxx$xxxxxxx xxxxxxx $$XXXxxxxxx$$ xx xxxx xx xxx xxxxxx xxxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx$Xxxxxxx xxxxxx xx xxx xxx Xxxxxxxx$XxxxxxXxxxx xxxxxxx xx xxx xxxxxx xxxxxxxx.

Xxx Xxxxxxxx$XxxxxxXxxxx xxxxxxx xxxx xxx XxxxxxXxxxxxxxxx xxxxxxxxx xx xxxxxxxx xxx xxxxx.
Xx xxxx xxx Xxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxx xxxx xxx xxxxxx xxxxxxx xx xxx xxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Register-EngineEvent -SourceIdentifier PowerShell.Exiting -SupportEvent -Action {
     Get-History | Export-Clixml $home\history.clixml
}
```

Xxxx xxxxxxx xxxxx xxx xx xxx Xxxxxxxx$XxxxxxXxxxx xx xxxx x xxxxxxxx xxxxxx xxxx xxx XxxxxXxxxx.Xxxxxxx xxxxx xxxxxx.
Xxx XxxxxxxXxxxx xxxxxxxxx xx xxxxx xx xxxx xxx xxxxx xxxxxxxxxxxx.
Xxxx Xxxxxxx XxxxxXxxxx xxxxx$ xx xxxx xxxx$ xxx xxxxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxx xx xxxxxxxx xx XXX xxxxxx xx x xxxx xxxx xxx xxxx xx xxx xxxx$x $xxxx xxxxxxxxx.

## XXXXXXXXXX

### -Action
Xxxxxxxxx xxxxxxxx xx xxxxxx xxx xxxxxx.
Xxx xxxxxxxx xx xxx Xxxxxx xxx xxxx xx xxxxx xx xxxxxx$ xxxxxxx xx xxxxxxx xxx xxxxx xx xxx xxxxx xxxxx.
Xxxxxxx xxx xxxxxxxx xx xxxxxx $ $ $ $ xx xxxxxx x xxxxxx xxxxx.

Xxx xxxxx xx xxx Xxxxxx xxxxxxxxx xxx xxxxxxx xxx $Xxxxx$ $XxxxxXxxxxxxxxx$ $Xxxxxx$ $XxxxxXxxx$ xxx $Xxxx xxxxxxxxx xxxxxxxxx$ xxxxx xxxxxxx xxxxxxxxxxx xxxxx xxx xxxxx xx xxx Xxxxxx xxxxxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

Xxxx xxx xxxxxxx xx xxxxxx$ Xxxxxxxx$XxxxxxXxxxx xxxxxxx xx xxxxx xxx xxxxxx xxxx xxxxxxxxxx xxxx xxxxxx.
Xxx xxx xxx xxx Xxx xxxxxxx xx xxxxxx xxx xxxxx xxx.

```yaml
Type: ScriptBlock
Parameter Sets: (All)
Aliases: 

Required: False
Position: 102
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Forward
Xxxxx xxxxxx xxx xxxx xxxxxxxxxxxx xx xxx xxxxxxx xx xxx xxxxx xxxxxxxx.
Xxx xxxx xxxxxxxxx xxxx xxx xxx xxxxxxxxxxx xxx xxxxxx xx x xxxxxx xxxxxxxx xx xx x xxxxxx xxxxxxx.

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

### -InformationAction
Xxx xxxxx xx xxx Xxxxxx xxxxxxxxx xxx xxxxxxx xxx $Xxxxx$ $XxxxxXxxxxxxxxx$ $Xxxxxx$ $XxxxxXxxx$ xxx $Xxxx xxxxxxxxx xxxxxxxxx$ xxxxx xxxxxxx xxxxxxxxxxx xxxxx xxx xxxxx xx xxx Xxxxxx xxxxxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

Xxxx xxx xxxxxxx xx xxxxxx$ Xxxxxxxx$XxxxxxXxxxx xxxxxxx xx xxxxx xxx xxxxxx xxxx xxxxxxxxxx xxxx xxxxxx.
Xxx xxx xxx xxx Xxx xxxxxxx xx xxxxxx xxx xxxxx xxx.

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
Xxx xxxxx xx xxx Xxxxxx xxxxxxxxx xxx xxxxxxx xxx $Xxxxx$ $XxxxxXxxxxxxxxx$ $Xxxxxx$ $XxxxxXxxx$ xxx $Xxxx xxxxxxxxx xxxxxxxxx$ xxxxx xxxxxxx xxxxxxxxxxx xxxxx xxx xxxxx xx xxx Xxxxxx xxxxxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

Xxxx xxx xxxxxxx xx xxxxxx$ Xxxxxxxx$XxxxxxXxxxx xxxxxxx xx xxxxx xxx xxxxxx xxxx xxxxxxxxxx xxxx xxxxxx.
Xxx xxx xxx xxx Xxx xxxxxxx xx xxxxxx xxx xxxxx xxx.

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

### -MaxTriggerCount
Xxx xxxxx xx xxx Xxxxxx xxxxxxxxx xxx xxxxxxx xxx $Xxxxx$ $XxxxxXxxxxxxxxx$ $Xxxxxx$ $XxxxxXxxx$ xxx $Xxxx xxxxxxxxx xxxxxxxxx$ xxxxx xxxxxxx xxxxxxxxxxx xxxxx xxx xxxxx xx xxx Xxxxxx xxxxxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

Xxxx xxx xxxxxxx xx xxxxxx$ Xxxxxxxx$XxxxxxXxxxx xxxxxxx xx xxxxx xxx xxxxxx xxxx xxxxxxxxxx xxxx xxxxxx.
Xxx xxx xxx xxx Xxx xxxxxxx xx xxxxxx xxx xxxxx xxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MessageData
Xxxxxxxxx xxxxxxxxxx xxxx xxxxxxxxxx xxxx xxx xxxxx.
Xxx xxxxx xx xxxx xxxxxxxxx xxxxxxx xx xxx XxxxxxxXxxx xxxxxxxx xx xxx xxxxx xxxxxx.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SourceIdentifier
Xxxxxxxxx xxx xxxxxx xxxxxxxxxx xx xxx xxxxx xx xxxxx xxx xxx xxxxxxxxxxx.
Xxx xxxxxx xxxxxxxxxx xxxx xx xxxxxx xx xxx xxxxxxx xxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx.

Xxx xxxxx xx xxxx xxxxxxxxx xxxxxxx xx xxx xxxxx xx xxx XxxxxxXxxxxxxxxx xxxxxxxx xx xxx xxxxxxxxxx xxxxxx xxx xx xxx xxxxx xxxxxxx xxxxxxxxxx xxxx xxxx xxxxxxxxxxxx.

Xxxxxxxxx XxxxxxXxxxx xxxxxx xxxxxxx XxxxxXxxxx.Xxxxxxx$ XxxxxXxxxx.XxXxxx$ xxx XxxxxXxxxx.XxXxxxxxXxxxxXxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 101
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SupportEvent
Xxxxx xxx xxxxx xxxxxxxxxxxx.
Xxx xxxx xxxxxxxxx xxxx xxx xxxxxxx xxxxxxxxxxxx xx xxxx xx x xxxx xxxxxxx xxxxx xxxxxxxxxxxx xxxxxxxxx xxx xx xxxxxx xxx xx xxxxxxxxxx xxxxxxxxxxxxx.

Xx xxxx xx xxxxxx x xxxxxxxxxxxx xxxx xxx xxxxxxx xxxx xxx XxxxxxxXxxxx xxxxxxxxx$ xxx xxx Xxxxx xxxxxxxxx xx xxx Xxx$XxxxxXxxxxxxxxx xx Xxxxxxxxxx$Xxxxx xxxxxxx.

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

## XXXXXX

### None
Xxx xxxxxx xxxx xxxxx xx Xxxxxxxx$XxxxxxXxxxx.

## XXXXXXX

### None or System.Management.Automation.PSEventJob
Xx xxx xxx xxx Xxxxxx xxxxxxxxx$ Xxxxxxxx$XxxxxxXxxxx xxxxxxx x Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxXxx xxxxxx.
Xxxxxxxxx$ xx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xxxxxx$ xxxxx xxxxxxxxxxxxx$ xxx xxx xxxxx xxxxx xxxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxx xxxxx xxx xxxxxxx xxxxxxx$ xxx xxxxx xxxxx xx xxxxxxxxx xxx xxx xxxxx xxxxxxxxxxxx xx xxxxxxxx.

## XXXXXXX XXXXX

[Get-Event]()

[Get-Job]()

[New-Event]()

[Receive-Job]()

[Register-ObjectEvent]()

[Register-WmiEvent]()

[Remove-Event]()

[Remove-Job]()

[Unregister-Event]()

[Wait-Event]()

[Wait-Job]()

