---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293954
schema: 2.0.0
---

# Enable-PSBreakpoint
## XXXXXXXX
Xxxxxxx xxx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxx.

## XXXXXX

### Id (Default)
```
Enable-PSBreakpoint [-PassThru] [-Id] <Int32[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### Breakpoint
```
Enable-PSBreakpoint [-PassThru] [-Breakpoint] <Breakpoint[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XXXxxxxxxxxx xxxxxx xx$xxxxxxx xxxxxxxx xxxxxxxxxxx.
Xxx xxx xxx xx xx xxxxxx xxx xxxxxxxxxxx$ xx xxx xxx xxxxxxx xxxxxxxxxxx xx xxxxxxxxxx xxxxxxxxxx xxxxxxx xx xxxxxxxxxx XXx.

X xxxxxxxxxx xx x xxxxx xx x xxxxxx xxxxx xxxxxxxxx xxxxx xxxxxxxxxxx xx xxxx xxx xxx xxxxxxx xxx xxxxxxxxxxxx xx xxx xxxxxx.
Xxxxx xxxxxxx xxxxxxxxxxx xxx xxxxxxxxxxxxx xxxxxxx$ xxx xxx xxx xxxxxxx xxxx xx xxxxx xxx Xxxxxxx$XXXxxxxxxxxx xxxxxx.

Xxxxxxxxxxx$ xxxx xxxxxx xxxxxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx x xxxxxxxxxx xxxxxx xx Xxxx.

Xxxxxx$XXXxxxxxxxxx xx xxx xx xxxxxxx xxxxxxx xxxxxxxx xxx xxxxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx$ xxx xxxxx$Xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-psbreakpoint | enable-psbreakpoint
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxx xxxxxxxxxx xxx xxxxxxx xx $xxx $ xxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>enable-psbreakpoint -id 0, 1, 5
```

Xxxx xxxxxxx xxxxxxx xxxxxxxxxxx xxxx xxxxxxxxxx XXx 0$ 0$ xxx 0.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$b = set-psbreakpoint -script sample.ps1 -variable Name
PS C:\>$b | disable-psbreakpoint -passthru

AccessMode : Write
Variable   : Name
Action     :
Enabled    : False
HitCount   : 0
Id         : 0
Script     : C:\ps-test\sample.ps1
ScriptName : C:\ps-test\sample.ps1

PS C:\>$b | enable-psbreakpoint -passthru

AccessMode : Write
Variable   : Name
Action     :
Enabled    : True
HitCount   : 0
Id         : 0
Script     : C:\ps-test\sample.ps1
ScriptName : C:\ps-test\sample.ps1
```

Xxxxx xxxxxxxx xx$xxxxxx x xxxxxxxxxx xxxx xxx xxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XXXxxxxxxxxx xxxxxx xx xxxxxx x xxxxxxxxxx xx xxx $Xxxx$ xxxxxxxx xx xxx Xxxxxx.xx0 xxxxxx.
Xxxx$ xx xxxxx xxx xxxxxxxxxx xxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxxx$XXXxxxxxxxxx xxxxxx xx xxxxxxx xxx xxx xxxxxxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxxxxx xxxxxx xx $x xx xxx Xxxxxxx$XXXxxxxxxxxx xxxxxx$ xxx xx xxxx xxx XxxxXxxx xxxxxxxxx xx Xxxxxxx$XXXxxxxxxxxx xx xxxxxxx xxx xxxxxxxx xxxxxxxxxx xxxxxx.
Xxxx xxxx xxx xxxxxx xxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxxxxxx xxxxxx xx Xxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxx$XXXxxxxxxxxx xxxxxx xx xx$xxxxxx xxx xxxxxxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxxxxx xxxxxx xx $x xx xxx Xxxxxx$XXXxxxxxxxxx xxxxxx$ xxx xx xxxx xxx XxxxXxxx xxxxxxxxx xx Xxxxxx$XXXxxxxxxxxx xx xxxxxxx xxx xxxxxxxxxx xxxxxx.
Xxxx xxxx xxx xxxxxx xxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxxxxxx xxxxxx xx Xxxx.

Xxx xxxxxxx xxx xxxxx xx xxx xxxxxxxxx xxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$b = get-psbreakpoint -id 3, 5
PS C:\>enable-psbreakpoint -breakpoint $b
```

Xxxxx xxxxxxxx xxxxxx x xxx xx xxxxxxxxxxx xx xxxxxxxxxx xxxxx xxxxxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XXXxxxxxxxxx xxxxxx xx xxx xxx xxxxxxxxxxx xxx xxxxx xxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx$XXXxxxxxxxxx xxxxxx xxx xxx Xxxxxxxxxx xxxxxxxxx xx xxxxxx xxx xxxxxxxxxxx.

Xxxx xxxxxxx xx xxx xxxxxxxxxx xx $xxxxxx$xxxxxxxxxxxx $xx 0$ 0$.

## XXXXXXXXXX

### -Breakpoint
Xxxxxxxxx xxx xxxxxxxxxxx xx xxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxxxxxxxxx xxxxxxx xx x xxxxxxx xxxx xxxx xxxxxxxxxx xxxxxxx$ xxxx xx x Xxx$XXXxxxxxxxxx xxxxxxx.
Xxx xxx xxxx xxxx xxxxxxxxxx xxxxxxx xx Xxxxxx$XXXxxxxxxxxx.

```yaml
Type: Breakpoint[]
Parameter Sets: Breakpoint
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Id
Xxxxxxx xxxxxxxxxxx xxxx xxxx xxx xxxxxxxxx xxxxxxxxxx XXx.
Xxx xxxxxxx xxxxx xx xxx xxxxxxxxxxx.
Xxxxx xxx XXx xx x xxxxxxxx xxxx xxxxxxxx xxx XXx.
$Xxx xxxxxx xxxx XXx xx Xxxxxx$XXXxxxxxxxxx.$ Xx xxxx xxx XX xx x xxxxxxxxxx$ xxx xxx Xxx$XXXxxxxxxxxx xxxxxx.

```yaml
Type: Int32[]
Parameter Sets: Id
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

### -PassThru
Xxxxxxx xx xxxxxx xxxxxxxxxxxx xxx xxxxxxx xxxxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

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

### -Confirm
$$Xxxx Xxxxxxx Xxxxxxxxxxx$$

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
$$Xxxx XxxxXx Xxxxxxxxxxx$$

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.Management.Automation.Breakpoint
Xxx xxx xxxx x xxxxxxxxxx xxxxxx xx Xxxxxx$XXXxxxxxxxxx.

## XXXXXXX

### None or System.Management.Automation.Breakpoint
Xxxx xxx xxx xxx XxxxXxxx xxxxxxxxx$ Xxxxxx$XXXxxxxxxxxx xxxxxxx x xxxxxxxxxx xxxxxx xxxx xxxxxxxxx xxxx xxxxxxxxxx xxxx xxx xxxxxxx.
Xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xxx Xxxxxx$XXXxxxxxxxxx xxxxxx xxxx xxx xxxxxxxx xx xxxxx xx xxx xxx xx xxxxxx x xxxxxxxxxx xxxx xx xxxxxxx xxxxxxx.
Xx xxxx$ xxx xxx xxxxxx xxx xxxxxxxxxxx xxxxxxx xxxxx$ xxxx xxxx xxxx x xxx xxx xxxxxxxx.

Xxxxxxxxxxx xxx xxxxxxx xxxx xxx xxxxxx xxxx xx xxxxx xxx Xxx$XXXxxxxxxxxx xxxxxx.
Xxx xx xxx xxxx xx xxxxxx xxxxx xxxxxxx xxxxxxxxxxx.

## XXXXXXX XXXXX

[Disable-PSBreakpoint]()

[Get-PSBreakpoint]()

[Get-PSCallStack]()

[Remove-PSBreakpoint]()

[Set-PSBreakpoint]()

[about_Debuggers]()

