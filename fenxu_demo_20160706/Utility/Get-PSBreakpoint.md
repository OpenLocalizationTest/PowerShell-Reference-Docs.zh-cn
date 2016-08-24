---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293972
schema: 2.0.0
---

# Xxx$XXXxxxxxxxxx
## XXXXXXXX
Xxxx xxx xxxxxxxxxxx xxxx xxx xxx xx xxx xxxxxxx xxxxxxx.

## XXXXXX

### Xxxxxx $Xxxxxxx$
```
Get-PSBreakpoint [[-Script] <String[]>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### Xxxx
```
Get-PSBreakpoint [[-Script] <String[]>] [-Type] <BreakpointType[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### Xxxxxxxx
```
Get-PSBreakpoint [[-Script] <String[]>] -Variable <String[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### Xxxxxxx
```
Get-PSBreakpoint [[-Script] <String[]>] -Command <String[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### Xx
```
Get-PSBreakpoint [-Id] <Int32[]> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$XXXxxxxXxxxx xxxxxx xxxx xxx xxxxxxxxxxx xxxx xxx xxx xx xxx xxxxxxx xxxxxxx.
Xxx xxx xxx xxx xxxxxx xxxxxxxxxx xx xxx xxxxxxxxxx xxxxxxxxxxx.

X xxxxxxxxxx xx x xxxxx xx x xxxxxxx xx xxxxxx xxxxx xxxxxxxxx xxxxx xxxxxxxxxxx xx xxxx xxx xxx xxxxxxx xxx xxxxxxxxxxxx.
Xxx$XXXxxxxxxxxx xx xxx xx xxxxxxx xxxxxxx xxxxxxxx xxx xxxxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx xxx xxxxxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx$ xxx xxxxx$Xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-psbreakpoint
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxx xxx xxxxxxxxxxx xxx xx xxx xxxxxxx xxx xxxxxxxxx xx xxx xxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-psbreakpoint -Id 2

Function   :
IncrementAction     :
Enabled    :
TrueHitCount   : 0
Id         : 2
Script     : C:\ps-test\sample.ps1
ScriptName : C:\ps-test\sample.ps1
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxx xxx xxxxxxxxxx xxxx xxxxxxxxxx XX 0.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$b = set-psbreakpoint -script sample.ps1 -function increment
PS C:\> $b.Id | get-psbreakpoint
```

Xxxxxxxxxxx

-----------

Xxxxx xxxxxxxx xxxx xxx xx xxx x xxxxxxxxxx xx xxxxxx x xxxxxxxxxx XX xx Xxx$XXXxxxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XXXxxxxxxxxx xxxxxx xx xxxxxx x xxxxxxxxxx xx xxx Xxxxxxxxx xxxxxxxx xx xxx Xxxxxx.xx0 xxxxxx.
Xx xxxxx xxx xxxxxxxxxx xxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxx xxxxxxxx $.$ xx xxx xxx Xx xxxxxxxx xx xxx xxxxxxxxxx xxxxxx xx xxx $x xxxxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx XX xx xxx Xxx$XXXxxxxxxxxx xxxxxx.

Xx x xxxxxx$ Xxx$XXXxxxxxxxxx xxxx xxx xxxxxxxxxx xxxx xxx xxxxxxxxx XX.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-psbreakpoint -script Sample.ps1, SupportScript.ps1
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxx xxx xx xxx xxxxxxxxxxx xx xxx Xxxxxx.xx0 xxx XxxxxxxXxxxxx.xx0 xxxxx.

Xxxx xxxxxxx xxxx xxx xxx xxxxx xxxxxxxxxxX xxxx xxxxx xx xxx xx xxxxx xxxxxxx xx xx xxxxxxxxx xx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-psbreakpoint -command Read-Host, Write-Host -script Sample.ps1
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxx xxx Xxxxxxx xxxxxxxxxxx xxxx xxx xxx xx Xxxx$Xxxx xx Xxxxx$Xxxx xxxxxxxx xx xxx Xxxxxx.xx0 xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-psbreakpoint -type Command -script Sample.ps1
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxx xxx Xxxxxxx xxxxxxxxxxx xx xxx Xxxxxx.xx0 xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-psbreakpoint -variable Index, Swap
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxx xxxxxxxxxxx xxxx xxx xxx xx xxx $xxxxx xxx $xxxx xxxxxxxxx xx xxx xxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-psbreakpoint -type line, variable -script Sample.ps1
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxx xxx xxxx xxx xxxxxxxx xxxxxxxxxxx xx xxx Xxxxxx.xx0 xxxxxx.

## XXXXXXXXXX

### $Xxxxxxx
Xxxx xxxxxxx xxxxxxxxxxx xxxx xxx xxx xx xxx xxxxxxxxx xxxxxxx xxxxx.
Xxxxx xxx xxxxxxx xxxxx$ xxxx xx xxx xxxx xx x xxxxxx xx xxxxxxxx.

```yaml
Type: String[]
Parameter Sets: Command
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xx
Xxxx xxx xxxxxxxxxxx xxxx xxx xxxxxxxxx xxxxxxxxxx XXx.
Xxxxx xxx XXx xx x xxxxx$xxxxxxxxx xxxx.
Xxx xxx xxxx xxxx xxxxxxxxxx XXx xx Xxx$XXXxxxxxxxxx.

```yaml
Type: Int32[]
Parameter Sets: Id
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
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

### $Xxxxxx
Xxxx xxxx xxx xxxxxxxxxxx xx xxx xxxxxxxxx xxxxxxx.
Xxxxx xxx  xxxx $xxxxxxxx$ xxx xxxxx xx xxx xx xxxx xxxxxx xxxxx.
Xx xxx xxxx xxx xxxx$ xxx xxxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: Script
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

```yaml
Type: String[]
Parameter Sets: Type, Variable, Command
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $Xxxx
Xxxx xxxx xxxxxxxxxxx xx xxx xxxxxxxxx xxxxx.
Xxxxx xxx xx xxxx xxxxx.
Xxxxx xxxxxx xxx Xxxx$ Xxxxxxx$ xxx Xxxxxxxx.
Xxx xxx xxxx xxxx xxxxxxxxxx xxxxx xx Xxx$XXXxxxxxxxxx.

```yaml
Type: BreakpointType[]
Parameter Sets: Type
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxx xxxxxxxx xxxxxxxxxxx xxxx xxx xxx xx xxx xxxxxxxxx xxxxxxxx xxxxx.
Xxxxx xxx xxxxxxxx xxxxx xxxxxxx xxxxxx xxxxx.

```yaml
Type: String[]
Parameter Sets: Variable
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxx00$ Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.XxxxxxxxxxXxxx
Xxx xxx xxxx xxxxxxxxxx XXx xxx xxxxxxxxxx xxxxx xx Xxx$XXXxxxxxxxxx.

## XXXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.Xxxxxxxxxx
Xxx$XXXxxxxXxxxx xxxxxxx xxxxxxx xxxx xxxxxxxxx xxx xxxxxxxxxxx xx xxx xxxxxxx.

## XXXXX
Xxx xxx xxx Xxx$XXXxxxxxxxxx xx xxx xxxxx$ $xxx$.

## XXXXXXX XXXXX

[Xxxxxxx$XXXxxxxxxxxx]()

[Xxxxxx$XXXxxxxxxxxx]()

[Xxx$XXXxxxXxxxx]()

[Xxxxxx$XXXxxxxxxxxx]()

[Xxx$XXXxxxxxxxxx]()

[xxxxx$Xxxxxxxxx]()

