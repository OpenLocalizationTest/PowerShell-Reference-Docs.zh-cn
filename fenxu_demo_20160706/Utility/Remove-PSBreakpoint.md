---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294004
schema: 2.0.0
---

# Remove-PSBreakpoint
## XXXXXXXX
Xxxxxxx xxxxxxxxxxx xxxx xxx xxxxxxx xxxxxxx.

## XXXXXX

### Breakpoint (Default)
```
Remove-PSBreakpoint [-Breakpoint] <Breakpoint[]> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### Id
```
Remove-PSBreakpoint [-Id] <Int32[]> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XXXxxxxxxxxx xxxxxx xxxxxxx x xxxxxxxxxx.
Xxxxx x xxxxxxxxxx xxxxxx xx x xxxxxxxxxx XX.

Xxxx xxx xxxxxx x xxxxxxxxxx$ xxx xxxxxxxxxx xxxxxx xx xx xxxxxx xxxxxxxxx xx xxxxxxxxxx.
Xx xxx xxxx xxxxx x xxxxxxxxxx xxxxxx xx x xxxxxxxx$ xxx xxxxxxxxx xxxxx xxxxxx$ xxx xxx xxxxxxxxxx xxxx xxx xxxxxxxx.

Xxxxxx$XXXxxxxxxxxx xx xxx xx xxxxxxx xxxxxxx xxxxxxxx xxx xxxxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx$ xxx xxxxx$Xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-breakpoint | remove-breakpoint
```

Xxxx xxxxxxx xxxxxxx xxx xx xxx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$b = set-psbreakpoint -script sample.ps1 -variable Name
PS C:\>$b | remove-psbreakpoint
```

Xxxx xxxxxxx xxxxxxx x xxxxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XXXxxxxxxxxx xxxxxx xx xxxxxx x xxxxxxxxxx xx xxx Xxxx xxxxxxxx xx xxx Xxxxxx.xx0 xxxxxx.
Xxxx$ xx xxxxx xxx xxxxxxxxxx xxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx$XXXxxxxxxxxx xxxxxx xx xxxxxx xxx xxx xxxxxxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxxxxx xxxxxx xx xxx $x xxxxxxxx xx xxx Xxxxxx$XXXxxxxxxxxx xxxxxx.

Xx x xxxxxx xx xxxx xxxxxxx$ xx xxx xxx xxx xxxxxx$ xx xxxx xx xxxxxxxxxx xxxxxxx xxxxxxxx.
Xxxx$ xxx Xxx$XXXxxxxxxxxx xxxxxx xxxx xxx xxxxxx xxxx xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>remove-psbreakpoint -id 2
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxxxxxx xxxx xxxxxxxxxx XX 0.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>function del-psb { get-psbreakpoint | remove-psbreakpoint }
```

Xxxx xxxxxx xxxxxxxx xxxxxxx xxx xx xxx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xx xxxx xxx Xxx$XXXxxxxxxxxx xxxxxx xx xxx xxx xxxxxxxxxxx.
Xxxx$ xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxxxxxx xx xxx Xxxxxx$XXXxxxxxxxxx xxxxxx$ xxxxx xxxxxxx xxxx.

Xx x xxxxxx$ xxx xxx xxxx $xxx$xxx$ xxxxxxx xx xxx xxxxxx xxxxxxx.

Xx xxxx xxx xxxxxxxx$ xxx xx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.

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
Xxxxxxx xxxxxxxxxxx xxxx xxx xxxxxxxxx xxxxxxxxxx XXx.

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

### System.Management.Automation.Breakpoint
Xxx xxx xxxx xxxxxxxxxx xxxxxxx xx Xxxxxx$XXXxxxxxxxxx.

## XXXXXXX

### None
Xxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX

## XXXXXXX XXXXX

[Disable-PSBreakpoint]()

[Enable-PSBreakpoint]()

[Get-PSBreakpoint]()

[Get-PSCallStack]()

[Set-PSBreakpoint]()

[about_Debuggers]()

