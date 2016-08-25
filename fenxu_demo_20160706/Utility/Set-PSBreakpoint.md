---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294013
schema: 2.0.0
---

# Set-PSBreakpoint
## XXXXXXXX
Xxxx x xxxxxxxxxx xx x xxxx$ xxxxxxx$ xx xxxxxxxx.

## XXXXXX

### Line (Default)
```
Set-PSBreakpoint [-Action <ScriptBlock>] [[-Column] <Int32>] [-Line] <Int32[]> [-Script] <String[]>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### Command
```
Set-PSBreakpoint [-Action <ScriptBlock>] -Command <String[]> [[-Script] <String[]>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### Variable
```
Set-PSBreakpoint [-Action <ScriptBlock>] [[-Script] <String[]>] -Variable <String[]>
 [-Mode <VariableAccessMode>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$XXXxxxxxxxxx xxxxxx xxxx x xxxxxxxxxx xx x xxxxxx xx xx xxx xxxxxxx xxx xx xxx xxxxxxx xxxxxxx. Xxx xxx xxx Xxx$XXXxxxxxxxxx xx xxx x xxxxxxxxxx xxxxxx xxxxxxxxx x xxxxxx xx xxxxxxx x xxxxxxx$ xx xxxxxx xxxxxxxxx$ xxxx xxxxxxx xx xxxxxxx xxxxxxxxxx.

Xxxx$ Xxx$XXXxxxxxxxxx xxxxxx xxx x xxxxxxxxxx xx x xxxxxx xxxxxxxx.
Xx xxxxx x xxxxxx xx x xxxxxx xxxxxxxx$ xxxx xxx xxxxxx xx xxx xxxxx xxxxxxxx xxx xxxx xxxxx xx xxxxxxx.

Xxxx Xxx$XXXxxxxxxxxx xxxxxxx xxxxxxx xxx xx xxx xxxxxxxxx xxxxx xxxxx xx xxxxxxxxxxx$

$$ Xxxx xxxxxxxxxx$  Xxxx xxxxxxxxxxx xx xxxxxxxxxx xxxx xxx xxxxxx xxxxxxxxxxx.
$$ Xxxxxxx xxxxxxxxxx$  Xxxx xxxxxxxxxxx xx xxxxxxxx xxx xxxxxxxxx.
$$ Xxxxxxxx xxxxxxxxxx$ Xxxx xxxxxxxxxxx xx xxxxxxxxx.

Xxx xxx xxx x xxxxxxxxxx xx xxxxxxxx xxxxx$ xxxxxxxx$ xx xxxxxxxxx xx x xxxxxx Xxx$XXXxxxxxxxxx xxxxxxx$ xxx xxxx Xxx$XXXxxxxxxxxx xxxxxxx xxxx xxxx xxx xxxx xx xxxxxxxxxx.

Xx x xxxxxxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxxxxxx xxxxx xxxxxxxxx xxx xxxxx xxxxxxx xx xxx xxxxxxxx.
Xxx xxxxxxx xxxxxx xxxxxxx xx $XXX$$$$ xxx x xxx xx xxxxxxxx xxxxxxxx xxxxxx xxxxxxxxx xxx xxx.
Xxxxxxx$ xxx xxx xxx xxx Xxxxxx xxxxxxxxx xx xxxxxxx xx xxxxxxxxx xxxxxxxx$ xxxx xx xxxxxxxxxx xxx xxx xxxxxxxxxx xx xxxxxxxxxxxx xx xxxxxxx xxxxxxxxxx xxxxx xxxx xx xxxxxxx xx xxxxxxxxxxx.

Xxx Xxx$XXXxxxxxxxxx xxxxxx xx xxx xx xxxxxxx xxxxxxx xxxxxxxx xxx xxxxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx$ xxx xxxxx$Xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-psbreakpoint -script sample.ps1 -line 5
Column     : 0
Line       : 5
Action     :
Enabled    : True
HitCount   : 0
Id         : 0
Script     : C:\ps-test\sample.ps1
ScriptName : C:\ps-test\sample.ps1
```

Xxxx xxxxxxx xxxx x xxxxxxxxxx xx xxxx 0 xx xxx Xxxxxx.xx0 xxxxxx.
Xx x xxxxxx$ xxxx xxx xxxxxx xxxx$ xxxxxxxxx xxxxx xxxxxxxxxxx xxxxxx xxxx 0 xxxxx xxxxxxx.

Xxxx xxx xxx x xxx xxxxxxxxxx xx xxxx xxxxxx$ xxx Xxx$XXXxxxxxxxxx xxxxxx xxxxxxxxx x xxxx xxxxxxxxxx xxxxxx $Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XxxxXxxxxxxxxx$ xxxx xxxxxxxx xxx xxxxxxxxxx XX xxx xxx xxxxx$ xx xxxxx xx xxx xxxxxxxxx xxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-psbreakpoint -command Increment -script sample.ps1
Command    : Increment
Action     :
Enabled    : True
HitCount   : 0
Id         : 1
Script     : C:\ps-test\sample.ps1
ScriptName : C:\ps-test\sample.ps1
```

Xxxx xxxxxxx xxxxxxx x xxxxxxx xxxxxxxxxx xx xxx Xxxxxxxxx xxxxxxxx xx xxx Xxxxxx.xx0 xxxxxx.
Xxx xxxxxx xxxxx xxxxxxxxx xxxxxxxxxxx xxxxxx xxxx xxxx xx xxx xxxxxxxxx xxxxxxxx.

Xxx xxxxxx xx x xxxxxxx xxxxxxxxxx xxxxxx.
Xxxxxx xxx xxxxxx xxxx$ xxx xxxxx xx xxx XxxXxxxx xxxxxxxx xx 0.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-psbreakpoint -script sample.ps1 -variable Server -Mode ReadWrite
```

Xxxx xxxxxxx xxxx x xxxxxxxxxx xx xxx Xxxxxx xxxxxxxx xx xxx Xxxxxx.xx0 xxxxxx.
Xx xxxx xxx Xxxx xxxxxxxxx xxxx x xxxxx xx XxxxXxxxx xx xxxx xxxxxxxxx xxxx xxx xxxxx xx xxx xxxxxxxx xx xxxx xxx xxxx xxxxxx xxx xxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-psbreakpoint -script Sample.ps1 -command "write*"
```

Xxxx xxxxxxx xxxx x xxxxxxxxxx xx xxxxx xxxxxxx xx xxx Xxxxxx.xx0 xxxxxx xxxx xxxxxx xxxx $xxxxx$$ xxxx xx $xxxxx$xxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-psbreakpoint -script test.ps1 -command DiskTest `
-action { if ($disk -gt 2) { break } }
```

Xxxx xxxxxxx xxxxx xxxxxxxxx xx xxx XxxxXxxx xxxxxxxx xx xxx Xxxx.xx0 xxxxxx xxxx xxxx xxx xxxxx xx xxx $xxxx xxxxxxxx xx xxxxxxx xxxx 0.

Xx xxxx xxx Xxx$XXXxxxxxxxxx xxxxxx xx xxx x xxxxxxx xxxxxxxxxx xx xxx XxxxXxxx xxxxxxxx.
Xxx xxxxx xx xxx xxxxxx xx x xxxxxx xxxxx xxxx xxxxx xxx xxxxx xx xxx $xxxx xxxxxxxx xx xxx xxxxxxxx.

Xxx xxxxxx xxxx xxx XXXXX xxxxxxx xx xxxx xxxxxxxxx xx xxx xxxxxxxxx xx xxx.
Xxx xxxxxxxxxxx $xxx xxx xxxxxxx$ xx XXXXXXXX.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-psbreakpoint -command checklog

Id       : 0
Command  : checkkog
Enabled  : True
HitCount : 0
Action   :

PS C:\>function CheckLog {
>> get-eventlog -log Application |
>> where {($_.source -like "TestApp") -and ($_.Message -like "*failed*")}
>>}
>>
PS C:\>Checklog
DEBUG: Hit breakpoint(s)
DEBUG:  Function breakpoint on 'prompt:Checklog'
PS C:\>>>
```

Xxxx xxxxxxx xxxx x xxxxxxxxxx xx xxx XxxxxXxx xxxxxxxx.
Xxxxxxx xxx xxxxxxx xxxx xxx xxxxxxx x xxxxxx$ xxx xxxxxxxxxx xx xxx xx xxxxxxxx xxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxxxxxxx xxxxxx xxxx xxx xxxxxxxx xx xxxxxx$ xxx xxxx xx xx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-psbreakpoint -script sample.ps1 -line 1, 14, 19 -column 2 -action {&(log.ps1)}

Column     : 2
Line       : 1
Action     :
Enabled    : True
HitCount   : 0
Id         : 6
Script     : C:\ps-test\sample.ps1
ScriptName : C:\ps-test\sample.ps1

Column     : 2
Line       : 14
Action     :
Enabled    : True
HitCount   : 0
Id         : 7
Script     : C:\ps-test\sample.ps1
ScriptName : C:\ps-test\sample.ps1

Column     : 2
Line       : 19
Action     :
Enabled    : True
HitCount   : 0
Id         : 8
Script     : C:\ps-test\sample.ps1
ScriptName : C:\ps-test\sample.ps1
```

Xxxx xxxxxxx xxxx xxxxx xxxx xxxxxxxxxxx xx xxx Xxxxxx.xx0 xxxxxx.
Xx xxxx xxx xxxxxxxxxx xx xxxxxx 0 xx xxxx xx xxx xxxxx xxxxxxxxx xx xxx xxxxxx.
Xxx xxxxxx xxxxxxxxx xx xxx Xxxxxx xxxxxxxxx xxxxxxx xx xxx xxxxxxxxxxx.

## XXXXXXXXXX

### -Action
Xxxxxxxxx xxxxxxxx xxxx xxx xx xxxx xxxxxxxxxx xxxxxxx xx xxxxxxxx.
Xxxxx x xxxxxx xxxxx xxxx xxxxxxxx xxx xxxxxxxx.
Xxx xxx xxx xxxx xxxxxxxxx xx xxx xxxxxxxxxxx xxxxxxxxxxx xx xx xxxxxxx xxxxx xxxxx$ xxxx xx xxxxxxx xx xxxxxxx.

Xx xxxx xxxxxxxxx xx xxxxxxx$ xx xx xxxxxx xx xxxxxxxxx$ xxxxxxxxx xxxxx xx xxx xxxxxxxxxx$ xxx xxx xxxxxxxx xxxxxx.

Xxxx xxx Xxxxxx xxxxxxxxx xx xxxx$ xxx Xxxxxx xxxxxx xxxxx xxxx xx xxxx xxxxxxxxxx.
Xxxxxxxxx xxxx xxx xxxx xxxxxx xxx xxxxxx xxxxx xxxxxxxx xxx Xxxxx xxxxxxx.
Xx xxx xxx xxx Xxxxxxxx xxxxxxx xx xxx xxxxxx xxxxx$ xxxxxxxxx xxxxxxx xxxxx xxx xxxx xxxxxxxxxx.

Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxx$Xxxxxx$ xxxxx$Xxxxx$ xxx xxxxx$Xxxxxxxx.

```yaml
Type: ScriptBlock
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Column
Xxxxxxxxx xxx xxxxxx xxxxxx xx xxx xxxxxx xx xxx xxxxxx xxxx xx xxxxx xxxxxxxxx xxxxx.
Xxxxx xxxx xxx xxxxxx xxxxxx.
Xxx xxxxxxx xx xxxxxx 0.

Xxx Xxxxxx xxxxx xx xxxx xxxx xxx xxxxx xx xxx Xxxx xxxxxxxxx xx xxxxxxx xxx xxxxxxxxxx.
Xx xxx Xxxx xxxxxxxxx xxxxxxxxx xxxxxxxx xxxxx$ xxx Xxxxxx xxxxxxxxx xxxx x xxxxxxxxxx xx xxx xxxxxxxxx xxxxxx xx xxxx xx xxx xxxxxxxxx xxxxx.
Xxxxxxx XxxxxXxxxx xxxxx xxxxxxxxx xxxxxx xxx xxxxxxxxx xx xxxxxxxxxx xxxx xxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxxx xxxx xxx xxxxxx xxxxxxxx.

Xxxxxxx xxx xxxxxxx xxxx xxx xxx xxxx xxxxxx xxxxxxxxx xxxx xxxxxx xxxxxx 0 $xxx 0$.
Xx xxx xxxxxxx x xxxxxx xxxx xxxx xxx xxxxx xx xxx xxxxxx$ xx xxxxx xx xxx xxxxxxxx$ xxx xxx xxxxxxxxxx xx xxxxx xxxxxxxx.

```yaml
Type: Int32
Parameter Sets: Line
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Command
Xxxx x xxxxxxx xxxxxxxxxx.
Xxxxx xxxxxx xxxxx$ xxxx xx $Xxx$Xxxxxxx$ xx xxxxxxxx xxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

Xxxxxxxxx xxxxx xxxx xxxxxx xxxx xxxxxxxx xx xxxx xxxxxxx xx xxxxxxxx.
Xx xxx xxxxxxx xx x xxxxxxxx$ xxxxxxxxx xxxxx xxxx xxxx xxx xxxxxxxx xx xxxxxx xxx xx xxxx XXXXX$ XXXXXXX$ xxx XXX xxxxxxx.

```yaml
Type: String[]
Parameter Sets: Command
Aliases: C

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
Xx xxxx xxxxxxxxx xx xxxxxxx$ xx xx xxxxxx xx xxxxxxxxx$ xxxxxxxxx xxxxx xx xxx xxxxxxxxxx$ xxx xxx xxxxxxxx xxxxxx.

Xxxx xxx Xxxxxx xxxxxxxxx xx xxxx$ xxx Xxxxxx xxxxxx xxxxx xxxx xx xxxx xxxxxxxxxx.
Xxxxxxxxx xxxx xxx xxxx xxxxxx xxx xxxxxx xxxxx xxxxxxxx xxx Xxxxx xxxxxxx.
Xx xxx xxx xxx Xxxxxxxx xxxxxxx xx xxx xxxxxx xxxxx$ xxxxxxxxx xxxxxxx xxxxx xxx xxxx xxxxxxxxxx.

Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxx$Xxxxxx$ xxxxx$Xxxxx$ xxx xxxxx$Xxxxxxxx.

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
Xx xxxx xxxxxxxxx xx xxxxxxx$ xx xx xxxxxx xx xxxxxxxxx$ xxxxxxxxx xxxxx xx xxx xxxxxxxxxx$ xxx xxx xxxxxxxx xxxxxx.

Xxxx xxx Xxxxxx xxxxxxxxx xx xxxx$ xxx Xxxxxx xxxxxx xxxxx xxxx xx xxxx xxxxxxxxxx.
Xxxxxxxxx xxxx xxx xxxx xxxxxx xxx xxxxxx xxxxx xxxxxxxx xxx Xxxxx xxxxxxx.
Xx xxx xxx xxx Xxxxxxxx xxxxxxx xx xxx xxxxxx xxxxx$ xxxxxxxxx xxxxxxx xxxxx xxx xxxx xxxxxxxxxx.

Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxx$Xxxxxx$ xxxxx$Xxxxx$ xxx xxxxx$Xxxxxxxx.

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

### -Line
Xxxx x xxxx xxxxxxxxxx xx x xxxxxx.
Xxxxx xxx xx xxxx xxxx xxxxxxx$ xxxxxxxxx xx xxxxxx.
Xxxxxxx XxxxxXxxxx xxxxx xxxxxxxxxxx xxxxxx xxxxxxxxx xxx xxxxxxxxx xxxx xxxxxx xx xxxx xx xxx xxxxxxxxx xxxxx.

Xxxxx xxx xxxxxxx xxxx xxx xxx xxxx xxxxxx xx xxx xxxxxx xxxx xxxxxxxxx xxxx xxxx xxxxxx 0 $xxx 0$.
Xx xxx xxxxxxx x xxxxx xxxx$ xxxxxxxxx xxxxx xxxxxx xxx xxxx xxx$xxxxx xxxx.
Xx xxx xxxx xx xxx xx xxxxx$ xxx xxxxxxxxxx xx xxxxx xxx.

```yaml
Type: Int32[]
Parameter Sets: Line
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Mode
Xxxxxxxxxx xxx xxxx xx xxxxxx xxxx xxxxxxxx xxxxxxxx xxxxxxxxxxx.
Xxx xxxxxxx xx Xxxxx.

Xxxx xxxxxxxxx xx xxxxx xxxx xxxx xxx Xxxxxxxx xxxxxxxxx xx xxxx xx xxx xxxxxxx.
Xxx xxxx xxxxxxx xx xxx xxxxxxxxxxx xxx xx xxx xxxxxxx.

Xxxxx xxxxxx xxx$

$$ Xxxxx$ Xxxxx xxxxxxxxx xxxxxxxxxxx xxxxxx x xxx xxxxx xx xxxxxxx xx xxx xxxxxxxx.
$$  Xxxx$ Xxxxx xxxxxxxxx xxxx xxx xxxxxxxx xx xxxx$ xxxx xx$ xxxx xxx xxxxx xx xxxxxxxx$ xxxxxx xx xx xxxxxxxx$ xxxxxxxxx$ xx xxxx. Xx xxxx xxxx$ xxxxxxxxx xxxx xxx xxxx xxxx xxx xxxxx xx xxx xxxxxxxx xxxxxxx.
$$  XxxxXxxxx$ Xxxxx xxxxxxxxx xxxx xxx xxxxxxxx xx xxxx xx xxxxxxx.

```yaml
Type: VariableAccessMode
Parameter Sets: Variable
Aliases: 
Accepted values: Read, Write, ReadWrite

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Script
Xxxx x xxxxxxxxxx xx xxxx xx xxx xxxxxxxxx xxxxxx xxxxx.
Xxxxx xxx xxxxx xxx xxxx xxxxx xx xxx xx xxxx xxxxxx xxxxx.
Xx xxx xxxxx xxx xx xxx xxxxxxx xxxxxxxxx$ xxx xxx xxxx xxx xxxx.
Xxxxxxxxx xxx xxxxxxxxx.

Xx xxxxxxx$ xxxxxxxx xxxxxxxxxxx xxx xxxxxxx xxxxxxxxxxx xxx xxx xx xxx xxxxxxx xxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx xxxx xxxx xxxxxxx x xxxx xxxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: Line
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String[]
Parameter Sets: Command, Variable
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Variable
Xxxx x xxxxxxxx xxxxxxxxxx.
Xxxxx x xxxxx$xxxxxxxxx xxxx xx xxxxxxxxx xxxxxxx xxxxxx xxxxx $$$.

Xxx xxx Xxxx xxxxxxxxxx xx xxxxxxxxx xxx xxxx xx xxxxxx xxxx xxxxxxxx xxx xxxxxxxxxxx.
Xxx xxxxxxx xxxx$ Xxxxx$ xxxxx xxxxxxxxx xxxx xxxxxx x xxx xxxxx xx xxxxxxx xx xxx xxxxxxxx.

```yaml
Type: String[]
Parameter Sets: Variable
Aliases: V

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### None
Xxx xxxxxx xxxx xxxxx xx Xxx$XXXxxxxxxxxx.

## XXXXXXX

### Breakpoint object (System.Management.Automation.LineBreakpoint, System.Management.Automation.VariableBreakpoint, System.Management.Automation.CommandBreakpoint)
Xxx$XXXxxxxxxxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxxx xxxxxxxxxx xxxx xx xxxx.

## XXXXX
Xxx$XXXxxxxxxxxx xxxxxx xxx x xxxxxxxxxx xx x xxxxxx xxxxxxxx.
Xx xxxxx x xxxxxx xx x xxxxxx xxxxxxxx$ xxxx xxx xxxxxx xx xxx xxxxx xxxxxxxx xxx xxxx xxxxx xx xxxxxxx.

Xxxx xxx xxx x xxxxxxxxxx xx xxxx xxxx xxx xxxx$ xxxxxxx$ xx xxxxxxxx$ Xxx$XXXxxxxxxxxx xxxxxxxxx x xxxxxxxxxx xxxxxx xxx xxxx xxxxx.

Xxxx xxxxxxx x xxxxxxxxxx xx x xxxxxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxx$ xxx xxx xxx xxx xxxxxxxxxx xxxxxx xx xxxxx xxx xxxxxx xxx xxxxxxxx xx xxxxxxxx.

## XXXXXXX XXXXX

[Disable-PSBreakpoint]()

[Enable-PSBreakpoint]()

[Get-PSBreakpoint]()

[Get-PSCallStack]()

[Remove-PSBreakpoint]()

[about_Debuggers]()

