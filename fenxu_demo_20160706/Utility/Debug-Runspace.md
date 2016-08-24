---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=403731
schema: 2.0.0
---

# Xxxxx$Xxxxxxxx
## XXXXXXXX
Xxxxxx xx xxxxxxxxxxx xxxxxxxxx xxxxxxx xxxx x xxxxxxxx.

## XXXXXX

### XxxxxxxxXxxxxxxxxXxx $Xxxxxxx$
```
Debug-Runspace [-Runspace] <Runspace> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

### XxxxXxxxxxxxxXxx
```
Debug-Runspace [-Name] <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

### XxXxxxxxxxxXxx
```
Debug-Runspace [-Id] <Int32> [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf]
 [-Confirm]
```

### XxxxxxxxXxXxxxxxxxxXxx
```
Debug-Runspace [-InstanceId] <Guid> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxxxx$Xxxxxxxx xxxxxx xx xxxxxxxxxxx xxxxxxxxx xxxxxxx xxxx x xxxxx xx xxxxxx xxxxxx xxxxxxxx.
Xxx xxx xxxx x xxxxxxxx xxxx xxx xxxx xx xxxxx xx xxxxx xxxxxxx Xxx$Xxxxxxx xx xxxx xxxxxxxxx xxxxxxxxxx xxxx Xxxxxxx XxxxxXxxxx$ xxxx Xxxxx$XXXxxxXxxxxxx xxxx xxx xxxxxxx XX xxxxxxxxx xx xxx Xx xxxxxxxxx xx xxxxxx xx xxx xxxxxxx$ xxx xxxx Xxx$Xxxxxxxx xx xxxx xxxxxxxxx xxxxxx xxx Xxxxxxx XxxxxXxxxx xxxx xxxxxxx.

Xxxxx xxx xxxx xxxxxxxx x xxxxxxxx xx xxxxx$ xx xxx xxxxxxxx xx xxxxxxxxx xxxxxxx x xxxxxxx xx xxxxxx$ xx xx xxx xxxxxx xxx xxxxxxx xx x xxxxxxxxxx$ Xxxxxxx XxxxxXxxxx xxxxx x xxxxxx xxxxxxxx xxxxxxx xxx xxx xxxxxxxx.
Xxx xxx xxxxx xxx xxxxxxxx xxxxxx xx xxx xxxx xxx xxxxxx xxxxxxx xxxxxxx xxx xxxxxxxx.

Xxx xxx xxxx xxxxxx xx x Xxxxxxx XxxxxXxxxx xxxx xxxxxxx xx xxx xxx xx xxxxxxxxxxxxx xx xxx xxxxxxxx xxxx xx xxxxxxx xxx xxxxxxx$ xx xxx xxx xxxxxxx xxx xxxxxx xxxx xxx xxxx xx xxxxx.
Xxxx$ xxx xxxxxx xxxxx xxx xxxx xxxxxxx xxxx xx xxxxxxx xxx xxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx$ xxx xxx xxxx xxxxx x xxxx xxxxxxx xxxx xx xxxxxxx x xxxxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxx xxxxxxx$ xx xxx xxx xxxxxxx xx x XxxxxXxxxx.xxx xxxxxxx$ xxx xxx$x xxxxx xxx xxxx xxxxxxx xxx xxxx xxxxxxx$ xxx xxx xxx xxxxx xxx xxxx xxxxxxx xx x xxxxxxx Xxxxxxx XxxxxXxxxx XXX xxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxx x xxxxxx xxxxxxxx
```
PS C:\>Get-Process -ComputerName WS10TestServer -Name *powershell*

Handles      WS(K)   VM(M)      CPU(s)    Id  ProcessName
-------      -----   -----      ------    --  -----------
    377      69912     63     2.09      2420  powershell
    399     123396    829     4.48      1152  powershell_ise

PS C:\> Enter-PSSession -ComputerName WS10TestServer

[WS10TestServer]:PS C:\> Enter-PSHostProcess -Id 1152

[WS10TestServer:][Process:1152]: PS C:\Users\Test\Documents> Get-Runspace

Id Name            ComputerName    Type          State         Availability
-- ----            ------------    ----          -----         ------------
 1 Runspace1       WS10TestServer  Remote        Opened        Available
 2 RemoteHost      WS10TestServer  Remote        Opened        Busy

[WS10TestServer][Process:1152]: PS C:\Users\Test\Documents> Debug-Runspace -Id 2

Hit Line breakpoint on 'C:\TestWFVar1.ps1:83'

At C:\TestWFVar1.ps1:83 char:1
+ $scriptVar = "Script Variable"
+ ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

[Process:1152]: [RSDBG: 2]: PS C:\>>
```

Xx xxxx xxxxxxx$ xxx xxxxx x xxxxxxxx xxxx xx xxxx xx x xxxxxx xxxxxxxx$ XX00XxxxXxxxxx.
Xx xxx xxxxx xxxx xx xxx xxxxxxx$ xxx xxx Xxx$Xxxxxxx xx xxx xxxxxx xxxxxxxx$ xxx xxxxxx xxx Xxxxxxx XxxxxXxxxx xxxx xxxxxxxxx.
Xx xxxx xxxxxxx$ xxx xxxx xx xxxxx xxxxxxx XX 0000$ xxx Xxxxxxx XxxxxXxxxx XXX xxxx xxxxxxx.

Xx xxx xxxxxx xxxxxxx$ xxx xxx Xxxxx$XXXxxxxxx xx xxxx x xxxxxx xxxxxxx xx XX00XxxxXxxxxx.
Xx xxx xxxxx xxxxxxx$ xxx xxxxxx xx xxx Xxxxxxx XxxxxXxxxx XXX xxxx xxxxxxx xxxxxxx xx xxx xxxxxx xxxxxx xx xxxxxxx Xxxxx$XXXxxxXxxxxxx$ xxx xxxxxxxxxx xxx XX xx xxx xxxx xxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxx xxxxxxx$ 0000.

Xx xxx xxxxxx xxxxxxx$ xxx xxxx xxxxxxxxx xxxxxxxxx xxx xxxxxxx XX 0000 xx xxxxxxx Xxx$Xxxxxxxx.
Xxx xxxx xxx XX xxxxxx xx xxx Xxxx xxxxxxxx$ xx xx xxxxxxx x xxxxxx xxxx xxx xxxx xx xxxxx.

Xx xxx xxxx xxxxxxx$ xxx xxxxx xxxxxxxxx xx xxxxxx xxxxxxxx xxxx xx xxxxxxx x xxxxxx$ XxxxXXXxx0.xx0$ xx xxxxxxx Xxxxx$Xxxxxxxx$ xxx xxxxxxxxxxx xxx xxxxxxxx xx xxx XX$ 0$ xx xxxxxx xxx Xx xxxxxxxxx.
Xxxxxxx xxxxx$x x xxxxxxxxxx xx xxx xxxxxx$ xxx xxxxxxxx xxxxx.

## XXXXXXXXXX

### $Xx
Xxxxxxxxx xxx XX xxxxxx xx x xxxxxxxx.
Xxx xxx xxx Xxx$Xxxxxxxx xx xxxx xxxxxxxx XXx.

```yaml
Type: Int32
Parameter Sets: IdParameterSet
Aliases: 

Required: True
Position: 1
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

### $XxxxxxxxXx
Xxxxxxxxx x xxxxxxxx xx xxx xxxxxxxx XX$ x XXXX xxxx xxx xxx xxxx xx xxxxxxx Xxx$Xxxxxxxx.

```yaml
Type: Guid
Parameter Sets: InstanceIdParameterSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx x xxxxxxxx xx xxx xxxx.
Xxx xxx xxx Xxx$Xxxxxxxx xx xxxx xxx xxxxx xx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: NameParameterSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxxxxxxx x xxxxxxxx xxxxxx.
Xxx xxxxxxxx xxx xx xxxxxxx x xxxxx xxx xxxx xxxxxxxxx xx xx xxxxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx x xxxxxxxx Xxx$Xxxxxxxx xxxxxxx.

```yaml
Type: Runspace
Parameter Sets: RunspaceParameterSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
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

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.Xxxxxxxxx.Xxxxxxxx
Xxx xxx xxxx xxx xxxxxxx xx x Xxx$Xxxxxxxx xxxxxxx xx Xxxxx$Xxxxxxxx.

## XXXXXXX

## XXXXX
Xxxxx$Xxxxxxxx xxxxx xx xxxxxxxxx xxxx xxx xx xxx Xxxxxx xxxxx.
Xx x xxxxxxxx xxxxx xxxxxxx xxxx Xxxxxx xx xxxxxxx xxxxx$ xxxx xxxxxxxx xx xxxxxxxxxxxxx xxxxxxx xxxx xxx xxxxxxx xxxx.
X xxxxxxxx xx xxxxx xx xxx xxxxxxx xxxx xxxx xx xx xxxxx xxx xxxxxxxxx xxxxxxxx.

$$ Xx xx xx xxxxxx xxxx Xxxxxx$Xxxxxxx$ xxxx xx$ xx xxx xx Xxxxxx$Xxxxxxx XXXX Xx.
$$ Xx xx xx xxxxxx xxxx Xxxxx$Xxxxxxxx$ xxxx xx$ xx xxx x Xxxxx$Xxxxxxxx XXXX Xx.
$$ Xx xx xx xxxxxx xxxx x Xxxxxxx XxxxxXxxxx xxxxxxxx$ xxx xxx xxxxxxxx xxx XX xx xxx xxxx xx xxx xxxxxxx xxxxxx xxxxxxxx xxxxxxxx xxx XX.

## XXXXXXX XXXXX

[xxxxx$Xxxxxxxxx]()

[Xxx$Xxxxxxx]()

[Xxxxx$XXXxxxXxxxxxx]()

[Xxx$Xxxxxxxx]()

[Xxxxx$Xxx]()

