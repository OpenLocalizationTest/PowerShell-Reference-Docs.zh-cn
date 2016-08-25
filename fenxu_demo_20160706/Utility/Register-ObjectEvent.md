---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294002
schema: 2.0.0
---

# Register-ObjectEvent
## XXXXXXXX
Xxxxxxxxxx xx xxx xxxxxx xxxx xxx xxxxxxxxx xx x Xxxxxxxxx .XXX Xxxxxxxxx xxxxxx.

## XXXXXX

```
Register-ObjectEvent [-InputObject] <PSObject> [-EventName] <String> [[-SourceIdentifier] <String>]
 [[-Action] <ScriptBlock>] [-MessageData <PSObject>] [-SupportEvent] [-Forward] [-MaxTriggerCount <Int32>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxxxx$XxxxxxXxxxx xxxxxx xxxxxxxxxx xx xxxxxx xxxx xxx xxxxxxxxx xx .XXX Xxxxxxxxx xxxxxxx xx xxx xxxxx xxxxxxxx xx xx x xxxxxx xxxxxxxx.

Xxxx xxx xxxxxxxxxx xxxxx xx xxxxxx$ xx xx xxxxx xx xxx xxxxx xxxxx xx xxxx xxxxxxx.
Xx xxx xxxxxx xx xxx xxxxx xxxxx$ xxx xxx Xxx$Xxxxx xxxxxx.

Xxx xxx xxx xxx xxxxxxxxxx xx Xxxxxxxx$XxxxxxXxxxx xx xxxxxxx xxxxxxxx xxxxxx xx xxx xxxxxx xxxx xxx xxxx xxx xx xxxxxxxx xxx xxxxx xx xxx xxxxx.
Xxx xxx xxxx xxx xxx Xxxxxx xxxxxxxxx xx xxxxxxx xxxxxxx xx xxxx xxxx x xxxxxxxxxx xxxxx xx xxxxxx xxx xxx Xxxxxxx xxxxxxxxx xx xxxx xxxxxx xxxxxx xx xxx xxxxx xxxxx xx xxx xxxxx xxxxxxx.

Xxxx xxx xxxxxxxxx xx xx xxxxx$ xx xxxxx xxxxxxxxx xx xxxxx xx xxxx xxxxxxx.
Xx xxx xxx xxxxx xxxxxxxxxxx xx xxx xxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxxxx xxxxxx.
Xx xxxxxx xxx xxxxxxxxxxxx$ xxx xxx Xxxxxxxxxx$Xxxxx xxxxxx$ xxxxx xxxxxxx xxx xxxxx xxxxxxxxxx xxxx xxx xxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$query = New-Object System.Management.WqlEventQuery "__InstanceCreationEvent", (New-Object TimeSpan 0,0,1), "TargetInstance isa 'Win32_Process'"
PS C:\>$processWatcher = New-Object System.Management.ManagementEventWatcher $query
PS C:\>register-objectEvent -inputObject $processWatcher -eventName "EventArrived"
```

Xxxx xxxxxxx xxxxxxxxxx xx xxxxxx xxxxxxxxx xxxx x xxx xxxxxxx xxxxxx.

Xxx xxxxxxx xxxx xxx XxxxxxxxxxXxxxxXxxxxxx xxxxxx xx xxx XxxxxXxxxxxx xxxxxx.
X xxxxx xxxxxx xxxxxxxxx xxxx xxx xxxxxx xxx xxxxxxxx xxxxxxxx xxxxxx xxx xxx Xxx00$Xxxxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$query = New-Object System.Management.WqlEventQuery "__InstanceCreationEvent", (New-Object TimeSpan 0,0,1), "TargetInstance isa 'Win32_Process'"
PS C:\>$processWatcher = New-Object System.Management.ManagementEventWatcher $query
PS C:\>$action = { New-Event "PowerShell.ProcessCreated" -Sender $sender -EventArguments $EventArgs.NewEvent.TargetInstance }
PS C:\>register-objectEvent -inputObject $processWatcher -eventName "EventArrived" -action $action

Id    Name            State      HasMoreData     Location             Command
--    ----            -----      -----------     --------             -------
2     422cfe5a-65e... Running    True                                 New-Event "PowerShe...
```

Xxxx xxxxxxx xxxxx xxx xx xxxxxxx xx xxxxxx xx xxxxxxx xx xx xxxxx.
Xxxx xxx xxxxxxx xx xxxxxx$ xxxxxx xxxx xxx xxxxxx xxx xxx xxxxx xx xxx xxxxx xxxxx.
Xxxxxxx$ xxx xxxxxx xxxxxxxx xx xxx xxxxx.

Xx xxxx xxxxxxx$ xxxx xx xxxxxxxx xxxxxxxx xxxxx xx xxxxxx xxxxxxxxxx xxxx x xxx xxxxxxx xx xxxxxxx$ x xxx XxxxxxxXxxxxxx xxxxx xx xxxxxx.

Xxx xxxxxx xxxx xxx $Xxxxxx xxx $XxxxxXxxx xxxxxxxxx xxxxxxxxx xxxxx xxx xxxxxxxxx xxxx xxx xxxxx xxxxxxx.

Xxx Xxxxxxxx$XxxxxxXxxxx xxxxxxx xxxxxxx x xxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx$ xxxxx xxxx xx x xxxxxxxxxx xxx.
Xxx xxx xxx xxx Xxx xxxxxxx$ xxxx xx Xxx$Xxx xxx Xxxxxxx$Xxx$ xx xxxxxx xxx xxxxxxxxxx xxx.

Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$s = new-pssession -computername Server01, Server02
PS C:\>invoke-command -session $s -filepath ProcessCreationEvent.ps1
PS C:\>invoke-command -session $s { get-event }# ProcessCreationEvent.ps1function Enable-ProcessCreationEvent{   $query = New-Object System.Management.WqlEventQuery "__InstanceCreationEvent", `
   (New-Object TimeSpan 0,0,1), `
   "TargetInstance isa 'Win32_Process'"   $processWatcher = New-Object System.Management.ManagementEventWatcher $query   $identifier = "WMI.ProcessCreated"   Register-ObjectEvent -input $processWatcher -eventName "EventArrived" `
   -sourceIdentifier $identifier -messageData "Test" -forward}EnableProcessCreationEvent
```

Xxxx xxxxxxx xxxxx xxx xx xxxxxxxxx xx xxxxxx xxxxxx xx xxxxxx xxxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx XXXxxxxxxx xx xxx xxxxxx xxxxxxxxx xxx xxxxx xxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx XxxxXxxx xxxxxxxxx xx xxx Xxxxxx$Xxxxxxx xxxxxx xx xxx xxx XxxxxxxXxxxxxxxXxxxx.xx0 xxxxxx xx xxx xxxx xx xxx XXXxxxxxxx xx $x.

Xxx xxxxxx xxxxxxxx x Xxxxxxxx$XxxxxxXxxxx xxxxxxx xxxx xxxxxxxxxx xx xxxxxxxx xxxxxxxx xxxxxx xx xxx Xxx00$Xxxxxxx xxxxxx xxxxxxx xxx XxxxxxxxxxXxxxxXxxxxxx xxxxxx xxx xxx XxxxxXxxxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$timer  = New-Object Timers.Timer
PS C:\>$timer.Interval = 500
PS C:\>$job = Register-ObjectEvent -inputObject $timer -eventName Elapsed -sourceIdentifier Timer.Random -Action {$random = Get-Random -Min 0 -Max 100}
PS C:\>$job.gettype().fullnameSystem.Management.Automation.PSEventJob
PS C:\>$job | format-list -property *

State         : 
RunningModule        : __DynamicModule_6b5cbe82-d634-41d1-ae5e-ad7fe8d57fe0
StatusMessage :
HasMoreData   : True
Location      :
Command       : $random = Get-Random -Min 0 -Max 100
JobStateInfo  : Running
Finished      : System.Threading.ManualResetEvent
InstanceId    : 88944290-133d-4b44-8752-f901bd8012e2
Id            : 1
Name          : Timer.Random
ChildJobs     : {}...

PS C:\>$timer.Enabled = $true
PS C:\>& $job.module {$random}60
PS C:\>& $job.module {$random}47
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx xxxxxxx xxxxxx xx xxx XXXxxxxXxx xxxxxx xxxx xx xxxxxxx xxxx xxx xxxxxxx xx Xxxxxx xx x xxxxx xxxxxxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxxxxx x xxxxx xxxxxx.
Xxx xxxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxx xx 000 $xxxxxxxxxxxx$.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxxxx$XxxxxxXxxxx xxxxxx xx xxxxxxxx xxx Xxxxxxx xxxxx xx xxx xxxxx xxxxxx.
Xxx xxxxxxx xxxxxxxx xx xxxxxx xxxx xxxxxxx xxx xxxxx.
Xxxxxxxx xxx xxxxx xxxxxxxx xxxxxxx$ xx xxxxx xx xxxxxx xxx xxx xxxxxxxx xx xxx xxxxxx xxx.
Xx xxxx xxxx$ xxx Xxx$Xxxxxx xxxxxx xxxxxxxxx x xxxxxx xxxxxx xxxxxxx 0 xxx 000 xxx xxxxx xx xx xxx $xxxxxx xxxxxxxx.

Xxxx xxx xxx xx Xxxxxx xxxxxxxxx xx x Xxxxxxxx$XxxxxxXxxxx xxxxxxx$ xxx xxxxxxx xxxxxxx x XXXxxxxXxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx.
Xxx xxxxxxx xxxxx xxx xxx xxxxxx xx xxx $xxx xxxxxxxx.

Xxx XXXxxxxXxx xxxxxx xxxx xxx Xxxxxxxx$XxxxxxXxxxx xxxxxx xxxxxxx xx xxxx xxxxxxxxx xx xxx Xxxxxx xxxxxxxx xx xxx xxxxx xxxxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx Xxx$XxxxxXxxxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxx xxxx xxx $xxx xxxxxxxx xxxxxxxx x XXXxxxxXxx xxxxxx.
Xxx xxxxx xxxxxxx xxxx xxx Xxxxxx$Xxxx xxxxxx xx xxxxxxx xxx xx xxx xxxxxxxxxx xx xxx XXXxxxxXxx xxxxxx xx x xxxx.

Xxx XXXxxxxXxx xxx x Xxxxxx xxxxxxxx xxxx xxxxxxxx x xxxxxxx xxxxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx xxx xxxxx.

Xxx xxxxxxxxx xxxxxxxx xxx xxx xxxx xxxxxxxx $$$ xx xxxxxx xxx xxxxxxx xx xxx xxxxxx xxx xxxxxxx xxx xxxxx xx xxx $xxxxxx xxxxxxxx.
Xxx xxx xxx xxx xxxx xxxxxxxx xx xxxxxx xxx xxxxxxx xx x xxxxxx$ xxxxxxxxx xxxxxxxx xxxx xxx xxx xxxxxxxx.
Xx xxxx xxxx$ xxx xxxxxxxx xxxx xxx xxxxxx xxxxxx xxxx xx xxxxx xxxxxxxxx xxxx xxx Xxxxxxx xxxxx xxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxxxxxx$ xxx xxxxx$Xxxxxxx.

## XXXXXXXXXX

### -Action
Xxxxxxxxx xxxxxxxx xx xxxxxx xxx xxxxxx.
Xxx xxxxxxxx xx xxx Xxxxxx xxx xxxx xx xxxxx xx xxxxxx$ xxxxxxx xx xxxxxxx xxx xxxxx xx xxx xxxxx xxxxx.
Xxxxxxx xxx xxxxxxxx xx xxxxxx $ $ $ $ xx xxxxxx x xxxxxx xxxxx.

Xxx xxxxx xx xxx Xxxxxx xxxxxxxxx xxx xxxxxxx xxx $Xxxxx$ $XxxxxXxxxxxxxxx$ $Xxxxxx$ $XxxxxXxxx$ xxx $Xxxx xxxxxxxxx xxxxxxxxx$ xxxxx xxxxxxx xxxxxxxxxxx xxxxx xxx xxxxx xx xxx Xxxxxx xxxxxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxxx.

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

### -EventName
Xxxxxxxxx xxx xxxxx xx xxxxx xxx xxx xxxxxxxxxxx.
Xxxxx xxx xxxxx xxxx.
Xxxx xxxxxxxxx xx xxxxxxxx.

Xxx xxxxx xx xxxx xxxxxxxxx xx xxx x xxxx xxxx xxx xxxxxx xxx xxx xxxxx xxxxxxxxxxxx.
Xx xx xxx xxxx xx xx xxxxx xxxx xxx .XXX Xxxxxxxxx xxxxxx xxxxxxx.
Xxx xxxxxxx$ xxx XxxxxxxxxxXxxxxXxxxxxx xxxxx xxx xxxxxx xxxxx $XxxxxXxxxxxx$ xxx $Xxxxxxx.$ Xx xxxx xxx xxxxx xxxx xx xx xxxxx$ xxx xxx Xxx$Xxxxxx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Forward
Xxxxx xxxxxx xxx xxxx xxxxxxxxxxxx xx x xxxxxx xxxxxxx.
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
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxxx.

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
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxxx.

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

### -InputObject
Xxxxxxxxx xxx .XXX Xxxxxxxxx xxxxxx xxxx xxxxxxxxx xxx xxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxx$ xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxTriggerCount
Xxx xxxxx xx xxx Xxxxxx xxxxxxxxx xxx xxxxxxx xxx $Xxxxx$ $XxxxxXxxxxxxxxx$ $Xxxxxx$ $XxxxxXxxx$ xxx $Xxxx xxxxxxxxx xxxxxxxxx$ xxxxx xxxxxxx xxxxxxxxxxx xxxxx xxx xxxxx xx xxx Xxxxxx xxxxxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxxx.

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
Xxxxxxxxx xxx xxxxxxxxxx xxxx xx xx xxxxxxxxxx xxxx xxxx xxxxx xxxxxxxxxxxx.
Xxx xxxxx xx xxxx xxxxxxxxx xxxxxxx xx xxx XxxxxxxXxxx xxxxxxxx xx xxx xxxxxx xxxxxxxxxx xxxx xxxx xxxxxxxxxxxx.

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
Xxxxxxxxx x xxxx xxxx xxx xxxxxx xxx xxx xxxxxxxxxxxx.
Xxx xxxx xxxx xxx xxxxxx xxxx xx xxxxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxxx xx xxx XXXX xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.

Xxx xxxxx xx xxxx xxxxxxxxx xxxxxxx xx xxx xxxxx xx xxx XxxxxxXxxxxxxxxx xxxxxxxx xx xxx xxxxxxxxx xxxxxx xxx xx xxx xxxxx xxxxxxx xxxxxxxxxx xxxx xxxx xxxxxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 101
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SupportEvent
Xxxxx xxx xxxxx xxxxxxxxxxxx.
Xxx xxxx xxxxxxxxx xxxx xxx xxxxxxx xxxxxxxxxxxx xx xxxx xx x xxxx xxxxxxx xxxxx xxxxxxxxxxxx xxxxxxxxx xxx xx xxxxxx xxx xx xxxxxxxxxx xxxxxxxxxxxxx.

Xx xxxx xx xxxxxx x xxxxxxxxxxxx xxxx xxx xxxxxxx xxxx xxx XxxxxxxXxxxx xxxxxxxxx$ xxx xxx Xxxxx xxxxxxxxx xx xxx Xxx$XxxxxXxxxxxxxxx xxx Xxxxxxxxxx$Xxxxx xxxxxxx.

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
Xxx xxxxxx xxxx xxxxxxx xx Xxxxxxxx$XxxxxxXxxxx.

## XXXXXXX

### System.Management.Automation.PSEventJob
Xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xxxxxx$ xxxxx xxxxxxxxxxxxx$ xxx xxx xxxxx xxxxx xxxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxx xxxxx xxx xxxxxxx xxxxxxx$ xxx xxxxx xxxxx xx xxxxxxxxx xxx xxx xxxxx xxxxxxxxxxxx xx xxxxxxxx.

## XXXXXXX XXXXX

[Get-Event]()

[New-Event]()

[Register-EngineEvent]()

[Register-WmiEvent]()

[Remove-Event]()

[Unregister-Event]()

[Wait-Event]()

