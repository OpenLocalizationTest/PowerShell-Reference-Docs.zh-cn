---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293968
schema: 2.0.0
---

# Get-EventSubscriber
## XXXXXXXX
Xxxx xxx xxxxx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxx.

## XXXXXX

### BySource (Default)
```
Get-EventSubscriber [[-SourceIdentifier] <String>] [-Force] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### ById
```
Get-EventSubscriber [-SubscriptionId] <Int32> [-Force] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$XxxxxXxxxxxxxxx xxxxxx xxxx xxx xxxxx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxx.

Xxxx xxx xxxxxxxxx xx xx xxxxx xx xxxxx x Xxxxxxxx xxxxx xxxxxx$ xx xxxxx xxxxxxxxxx xx xxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx$ xxx xxx xxxxxx xx xxxxx xxx xxxxxxxxxx xxx xxxxx xx xxxx xxxxx xxxxx xxxxxxxx xxxx xxx xxxxxx.
Xx xxxxxx xx xxxxx xxxxxxxxxxxx$ xxxxxx xxx xxxxx xxxxxxxxxx xx xxxxx xxx Xxxxxxxxxx$Xxxxx xxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$timer = New-Object Timers.Timer
PS C:\>$timer | Get-Member -Type Event
PS C:\>Register-ObjectEvent -inputObject $timer -EventName Elapsed -SourceIdentifier Timer.Elapsed
PS C:\>Get-EventSubscriber
PS C:\>$timer = New-Object Timers.Timer
PS C:\>$timer | Get-Member -Type Event
TypeName: System.Timers.Timer

Name     MemberType Definition
----     ---------- ----------
Disposed Event      System.EventHandler Disposed(System.Object, System.EventArgs)
Elapsed  Event      System.Timers.ElapsedEventHandler Elapsed(System.Object, System.Timers.ElapsedEventArgs)

PS C:\>Register-ObjectEvent -InputObject $timer -EventName Elapsed -SourceIdentifier Timer.Elapsed
PS C:\>Get-EventSubscriber

SubscriptionId   : 4
SourceObject     : System.Timers.Timer
EventName        : Elapsed
SourceIdentifier : Timer.Elapsed
Action           :
HandlerDelegate  :
SupportEvent     : False
ForwardEvent     : False
```

Xxxx xxxxxxx xxxx x Xxx$XxxxxXxxxxxxxxx xxxxxxx xx xxx xxx xxxxx xxxxxxxxxx xxx x xxxxx xxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxxxxx xx xxxxxxxx xx x xxxxx xxxxxx.
Xx xxxxx xxx xxx xxxxx xxxxxx xx xxx $xxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxxxxxx xxx xxxxxx xxxx xxx xxxxxxxxx xxx xxxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx Xxxx xxxxxxxxx xx xxx Xxx$Xxxxxx xxxxxx xxxx x xxxxx xx Xxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxxxx$XxxxxxXxxxx xxxxxx xx xxxxxxxx xxx xxx Xxxxxxx xxxxx xx xxx xxxxx xxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxx$XxxxxXxxxxxxxxx xxxxxx xx xxx xxx xxxxx xxxxxxxxxx xxx xxx Xxxxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$timer  = New-Object Timers.Timer
PS C:\>$timer.Interval = 500
PS C:\>Register-ObjectEvent -inputObject $timer -eventName Elapsed -sourceIdentifier Timer.Random -Action { $random = Get-Random -Min 0 -Max 100 }

Id  Name           State      HasMoreData  Location  Command
--  ----           -----      -----------  --------  -------
3   Timer.Random   NotStarted False                  $random = Get-Random ...

PS C:\>$timer.Enabled = $true
PS C:\>$subscriber = Get-EventSubcriber -sourceIdentifer Timer.Random
PS C:\>($subscriber.action).gettype().fullname
PSEventJob

PS C:\>$subscriber.action | format-list -property *

State         : Running
Module        : __DynamicModule_6b5cbe82-d634-41d1-ae5e-ad7fe8d57fe0
StatusMessage :
HasMoreData   : True
Location      :
Command       : $random = Get-Random -Min 0 -Max 100
JobStateInfo  : Running
Finished      : System.Threading.ManualResetEvent
InstanceId    : 88944290-133d-4b44-8752-f901bd8012e2
Id            : 1
Name          : Timer.Random
ChildJobs     : {}
...
PS C:\>& $subscriber.action.module {$random}
96

PS C:\>& $subscriber.action.module {$random}
23
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx xxxxxxx xxxxxx xx xxx XXXxxxxXxx xxxxxx xx xxx Xxxxxx xxxxxxxx xx xxx xxxxx xxxxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxxxxx x xxxxx xxxxxx.
Xxx xxxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxx xx 000 $xxxxxxxxxxxx$.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxxxx$XxxxxxXxxxx xxxxxx xx xxxxxxxx xxx Xxxxxxx xxxxx xx xxx xxxxx xxxxxx.
Xxx xxxxxxx xxxxxxxx xx xxxxxx xxxx xxxxxxx xxx xxxxx.
Xxxxxxxx xxx xxxxx xxxxxxxx xxxxxxx$ xx xxxxx xx xxxxxx xxx xxx xxxxxxxx xx xxx xxxxxx xxx.
Xx xxxx xxxx$ xxx Xxx$Xxxxxx xxxxxx xxxxxxxxx x xxxxxx xxxxxx xxxxxxx 0 xxx 000 xxx xxxxx xx xx xxx $xxxxxx xxxxxxxx.
Xxx xxxxxx xxxxxxxxxx xx xxx xxxxx xx Xxxxx.Xxxxxx.

Xxxx xxx xxx xx Xxxxxx xxxxxxxxx xx x Xxxxxxxx$XxxxxxXxxxx xxxxxxx$ xxx xxxxxxx xxxxxxx x XXXxxxxXxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx xxx xxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XxxxxXxxxxxxxxx xxxxxx xx xxx xxx xxxxx xxxxxxxxxx xx xxx Xxxxx.Xxxxxx xxxxx.
Xx xxxxx xxx xxxxx xxxxxxxxxx xxxxxx xx xxx $xxxxxxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxx xxxx xxx Xxxxxx xxxxxxxx xx xxx xxxxx xxxxxxxxxx xxxxxx xxxxxxxx x XXXxxxxXxx xxxxxx.
Xx xxxx$ xx xxxxxxxx xxx xxxx XXXxxxxXxx xxxxxx xxxx xxx Xxxxxxxx$XxxxxxXxxxx xxxxxxx xxxxxxxx.

Xxx xxxxxxx xxxxxxx xxxx xxx Xxxxxx$Xxxx xxxxxx xx xxxxxxx xxx xx xxx xxxxxxxxxx xx xxx XXXxxxxXxx xxxxxx xx xxx Xxxxxx xxxxxxxx xx x xxxx.
Xxx xxxxxx xxxxxx xxxx xxx XXXxxxxXxx xxxxxx xxx x Xxxxxx xxxxxxxx xxxx xxxxxxxx x xxxxxxx xxxxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx.

Xxx xxxxxxxxx xxxxxxxx xxx xxx xxxx xxxxxxxx $$$ xx xxxxxx xxx xxxxxxx xx xxx xxxxxx xxx xxxxxxx xxx xxxxx xx xxx $xxxxxx xxxxxxxx.
Xxx xxx xxx xxx xxxx xxxxxxxx xx xxxxxx xxx xxxxxxx xx x xxxxxx$ xxxxxxxxx xxxxxxxx xxxx xxx xxx xxxxxxxx.
Xx xxxx xxxx$ xxx xxxxxxxx xxxx xxx xxxxxx xxxxxx xxxx xx xxxxx xxxxxxxxx xxxx xxx Xxxxxxx xxxxx xxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxxxxxx$ xxx xxxxx$Xxxxxxx.

## XXXXXXXXXX

### -Force
Xxxx xxx xxxxx xxxxxxxxxxx$ xxxxxxxxx xxxxxxxxxxx xxx xxxxxx xxxx xxx xxxxxx xx xxxxx xxx XxxxxxxXxxxx xxxxxxxxx xx Xxxxxxxx$XxxxxxXxxxx$ Xxxxxxxx$XxxXxxxx$ xxx Xxxxxxxx$XxxxxxXxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
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

### -SourceIdentifier
Xxxx xxxx xxx xxxxx xxxxxxxxxxx xxxx xxx xxxxxxxxx XxxxxxXxxxxxxxxx xxxxxxxx xxxxx.
Xx xxxxxxx$ Xxx$XxxxxXxxxxxxxxx xxxx xxx xxxxx xxxxxxxxxxx xx xxx xxxxxxx.
Xxxxxxxxx xxx xxx xxxxxxxxx.
Xxxx xxxxxxxxx xx xxxx$xxxxxxxxx.

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

### -SubscriptionId
Xxxx xxxx xxx xxxxxxxxx xxxxxxxxxxxx xxxxxxxxxx.
Xx xxxxxxx$ Xxx$XxxxxXxxxxxxxxx xxxx xxx xxxxx xxxxxxxxxxx xx xxx xxxxxxx.

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

## XXXXXX

### None
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### System.Management.Automation.PSEventSubscriber
Xxx$XxxxxXxxxxxxxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxxx xxxxx xxxxxxxxxx.

## XXXXX
Xxx Xxx$Xxxxx xxxxxx$ xxxxx xxxxxxx x xxxxxx xxxxx$ xxxx xxx xxxxxxxx x xxxxxxxxxx.
Xxxxxxxxx$ xxx Xxx$XxxxxXxxxxxxxxx xxxxxx xxxx xxx xxxx x xxxxxxxxxx xxxxxx xxx xxxxx xxxxxx.
Xxxxxxx$ xx xxx xxx xxx Xxxxxxxx$XxxxxxXxxxx xxxxxx xx xxxxxxxxx xx x xxxxxx xxxxx $xx xxxxx xx xxxxxxx xxx xxxxx xx xx xxxxxxx xx xxxxxx$$ Xxx$XxxxxXxxxxxxxxx xxxx xxxx xxx xxxxxxxxxx xxxx Xxxxxxxx$XxxxxxXxxxx xxxxxxxxx.

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

