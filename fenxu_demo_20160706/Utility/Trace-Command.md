---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294020
schema: 2.0.0
---

# Trace-Command
## XXXXXXXX
Xxxxxxxxxx xxx xxxxxx x xxxxx xx xxx xxxxxxxxx xxxxxxxxxx xx xxxxxxx.

## XXXXXX

### expressionSet (Default)
```
Trace-Command [-InputObject <PSObject>] [-Name] <String[]> [[-Option] <PSTraceSourceOptions>]
 [-Expression] <ScriptBlock> [-ListenerOption <TraceOptions>] [-FilePath <String>] [-Force] [-Debugger]
 [-PSHost] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### commandSet
```
Trace-Command [-InputObject <PSObject>] [-Name] <String[]> [[-Option] <PSTraceSourceOptions>]
 [-Command] <String> [-ArgumentList <Object[]>] [-ListenerOption <TraceOptions>] [-FilePath <String>] [-Force]
 [-Debugger] [-PSHost] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxx$Xxxxxxx xxxxxx xxxxxxxxxx xxx xxxxxx x xxxxx xx xxx xxxxxxxxx xxxxxxxxxx xx xxxxxxx.
Xx xxxxx xxxx Xxx$XxxxxXxxxxx$ xxxxxx xxxx xx xxxxxxx xxxx xx xxx xxxxxxxxx xxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>trace-command -name metadata,parameterbinding,cmdlet -expression {get-process notepad} -pshost
```

Xxxx xxxxxxx xxxxxx x xxxxx xx xxxxxxxx xxxxxxxxxx$ xxxxxxxxx xxxxxxx$ xxx xxxxxx xxxxxxxx xxx xxxxxxxxxxx xx xxx $xxx$xxxxxxx xxxxxxx$ xxxxxxxxxx.
Xx xxxx xxx Xxxx xxxxxxxxx xx xxxxxxx xxx xxxxx xxxxxxx$ xxx Xxxxxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxxx$ xxx xxx XXXxxx xxxxxxxxx xx xxxx xxx xxxxxx xx xxx xxxxxxx.
Xxxxxxx xx xxxx xxx xxxxxxx xxx xxxxxxx xxxxxxx xx xxxxxxxx xxxxxxx$ xxx xxxxxxx xxxx xxx xxxxxxxx$ $Xxx$ xxx xxx xxxxxxx xxxxxxx$ xxx $Xxxx$ xxx xxx xxxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = "i*"
PS C:\>trace-command parameterbinding {get-alias $input} -pshost -inputobject $a
```

Xxxxx xxxxxxxx xxxxx xxx xxxxxxx xx xxx XxxxxxxxxXxxxxxx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx xxxxx xx xxxxxxxxx x Xxx$Xxxxx xxxxxxxxxx xxxx xxxxx xxxxx xxxx xxx xxxxxxxx.

Xx Xxxxx$Xxxxxxx$ xxx XxxxxXxxxxx xxxxxxxxx xxxxxx xx xxxxxx xx xxx xxxxxxxxxx xxxx xx xxxxx xxxxxxxxx xxxxxx xxx xxxxx.

Xxx xxxxx xxxxxxx xxxxxx xxx xxxxxx $x$$ xx xxx $x xxxxxxxx.
Xxx xxxxxx xxxxxxx xxxx xxx Xxxxx$Xxxxxxx xxxxxx xxxx xxx XxxxxxxxxXxxxxxx xxxxx xxxxxx.
Xxx XXXxxx xxxxxxxxx xxxxx xxx xxxxxx xx xxx xxxxxxx.

Xxx xxxxxxxxxx xxxxx xxxxxxxxx xx $xxx$xxxxx $xxxxx$$ xxxxx xxx $xxxxx xxxxxxxx xx xxxxxxxxxx xxxx xxx XxxxxXxxxxx xxxxxxxxx.
Xxx XxxxxXxxxxx xxxxxxxxx xxxxxx xxx xxxxxxxx $x xx xxx xxxxxxxxxx.
Xx xxxxxx$ xxx xxxxxxx xxxxx xxxxxxxxx xxxxxx xxx xxxxx xx $xxx$xxxxx $xxxxxxxxxxx $x$ xx $$x $ xxx$xxxxx$.

## XXXXXXXXXX

### -ArgumentList
Xxxxxxxxx xxx xxxxxxxxxx xxx xxxxxxxxx xxxxxx xxx xxx xxxxxxx xxxxx xxxxxx.
Xxx xxxxx xxx XxxxxxxxXxxx xx Xxxx.
Xxxx xxxxxxx xx xxxxxxxxxx xxxxxx xxx xxxxxxxxx xxxxxxx xxxxxxxxxx.

```yaml
Type: Object[]
Parameter Sets: commandSet
Aliases: Args

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Command
Xxxxxxxxx x xxxxxxx xxxx xx xxxxx xxxxxxxxx xxxxxx xxx xxxxx.

```yaml
Type: String
Parameter Sets: commandSet
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Debugger
Xxxxx xxx xxxxx xxxxxx xx xxx xxxxxxxx.
Xxx xxx xxxx xxx xxxxxx xx xxx xxxx$xxxx xx xxxxxx xxxx xxxxxxxx xx xx Xxxxxx Xxxxxx.
Xxxx xxxxxxxxx xxxx xxxxxxx xxx xxxxxxx xxxxx xxxxxxxx.

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

### -Expression
Xxxxxxxxx xxx xxxxxxxxxx xxxx xx xxxxx xxxxxxxxx xxxxxx xxx xxxxx.
Xxxxxxx xxx xxxxxxxxxx xx xxxxxx $$$$.

```yaml
Type: ScriptBlock
Parameter Sets: expressionSet
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FilePath
Xxxxx xxx xxxxx xxxxxx xx xxx xxxxxxxxx xxxx.
Xxxx xxxxxxxxx xxxx xxxxxxx xxx xxxx xxxxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: PSPath

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Xxxxxx xxx xxxxxx xx xxxxxx xxxxx xxxxxxxxxxx xx x xxxx$xxxx xxxx.
Xxxx xxxx xxx XxxxXxxx xxxxxxxxx.
Xxxx xxxxx xxx Xxxxx xxxxxxxxx$ xxx xxxxxx xxxxxx xxxxxxxx xxxxxxxx xxxxxxxxxxxx.

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

### -InputObject
Xxxxxxxx xxxxx xx xxx xxxxxxxxxx xxxx xx xxxxx xxxxxxxxx xxxxxx xxx xxxxx.

Xxx xxx xxxxx x xxxxxxxx xxxx xxxxxxxxxx xxx xxxxx xxxx xxx xxxxxxxxxx xxxxxxx$ xx xxxx xx xxxxxx xxxxxxx xxx xxxxxxxx.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ListenerOption
Xxxx xxxxxxxx xxxx xx xxx xxxxxx xx xxxx xxxxx xxxxxxx xx xxx xxxxxx.
Xxx xxxxx xxxxxx xxx Xxxx$ XxxxxxxXxxxxxxxxXxxxx$ XxxxXxxx$ Xxxxxxxxx$ XxxxxxxXx$ XxxxxxXx$ xxx Xxxxxxxxx.
$Xxxx$ xx xxx xxxxxxx.

Xx xxxxxxx xxxxxxxx xxxxxxx$ xxxxxxxx xxxx xxxx xxxxxx$ xxx xxxx xx xxxxxx$ xxx xxxxxxx xxxx xx xxxxxxxxx xxxxx$ xxxx xx $XxxxxxxXX$XxxxxxXX$.

```yaml
Type: TraceOptions
Parameter Sets: (All)
Aliases: 
Accepted values: None, Constructor, Dispose, Finalizer, Method, Property, Delegates, Events, Exception, Lock, Error, Errors, Warning, Verbose, WriteLine, Data, Scope, ExecutionFlow, Assert, All

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Xxxxxxxxxx xxxxx Xxxxxxx XxxxxXxxxx xxxxxxxxxx xxx xxxxxx.
Xxxxx xxx xxxx xx xxx xxxxx xxxxxx xx xxxx xxxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.
Xx xxxx xxx xxxxx xxxxxxx xx xxxx xxxxxxxx$ xxxx $Xxx$XxxxxXxxxxx$.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Option
Xxxxxxxxxx xxx xxxx xx xxxxxx xxxx xxx xxxxxx.

Xxx xxxxx xxxxxx xxx Xxxx$ Xxxxxxxxxxx$ Xxxxxxx$ Xxxxxxxxx$ Xxxxxx$ Xxxxxxxx$ Xxxxxxxxx$ Xxxxxx$ Xxxxxxxxx$ Xxxx$ Xxxxx$ Xxxxxx$ Xxxxxxx$ Xxxxxxx$ XxxxxXxxx$ Xxxx$ Xxxxx$ XxxxxxxxxXxxx$ Xxxxxx$ xxx Xxx.
$Xxx$ xx xxx xxxxxxx.

Xxx xxxxxxxxx xxxxxx xxx xxxxxxxxxxxx xx xxxxx xxxxxx$

$$ XxxxxxxxxXxxx$ $Xxxxxxxxxxx$ Xxxxxxx$ Xxxxxxxxx$ Xxxxxx$ Xxxxxxxxx$ Xxxxxx$ xxx Xxxxx$ $$ Xxxx$ $Xxxxxxxxxxx$ Xxxxxxx$ Xxxxxxxxx$ Xxxxxxxx$ Xxxxxxx$ xxx XxxxxXxxx$ $$ Xxxxxx$ $Xxxxx xxx Xxxxxxxxx$.

Xx xxxxxxx xxxxxxxx xxxxxxx$ xxxxxxxx xxxx xxxx xxxxxx$ xxx xxxx xx xxxxxx$ xxx xxxxxxx xxxx xx xxxxxxxxx xxxxx$ xxxx xx $Xxxxxxxxxxx$Xxxxxxx$.

```yaml
Type: PSTraceSourceOptions
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PSHost
Xxxxx xxx xxxxx xxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxx.
Xxxx xxxxxxxxx xxxx xxxxxxx xxx XXXxxx xxxxx xxxxxxxx.

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

### System.Management.Automation.PSObject
Xxx xxx xxxx xxxxxxx xxxx xxxxxxxxx xxxxx xx xxx xxxxxxxxxx xx Xxxxx$Xxxxxxx.

## XXXXXXX

### System.Management.Automation.PSObject
Xxxxxxx xxx xxxxxxx xxxxx xx xxx xxxxx xxxxxx.

## XXXXX
Xxxxxxx xx x xxxxxx xxxx xxxxxxxxxx xxx xx xxxxx xxx xxxxxx xxxxxxxx.
Xxxx xxxxxxx$ xxx xxxxxxx xxxxxxxxx xxxxxxxx xxxxxxxx xxxxx xxxx xxxx xx xxx xxxxxxxx xxxxxxxxxx.

Xxx Xxxxxxx XxxxxXxxxx xxxxxxx xxxxxxx xxx xxxxxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxxxxx$ xxx xxxx xxx xxxxxxxxx xx xxx xxxxx.
Xxxx xxx xxx xxxxxxx xxxxxx xxxxx xxxxxx xx xxx xxxxxxxxxxxxx xx xxx xxxxx.

Xx xxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxxx xxxx xxx xxxxxxx xxx xxxxxxx$ xxxx $Xxx$Xxxx Xxx$XxxxxXxxxxx.$

X $xxxxx xxxxxx$ xx xxx xxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxxxx xxxx xxxxxxx xxxxxxx xxx xxxxxxxxx xxxxx xxxxxxxx xxx xxx xxxxxxxxx.
Xx xxxxx x xxxxxxxxx$ xxx xxxxxxxx xxx xxxxx xxxxxx.

X $xxxxx xxxxxxxx$ xxxxxxxx xxx xxxxxx xx xxx xxxxx xxx xxxxxxxx xx xx xxx xxxx.
Xxx xxx xxxxx xx xxxx xxx xxxxx xxxx xx x xxxx$xxxx xx xxxxxx$xxxx xxxxxxxx$ xx xxx xxxx xx xxxxxxx$ xx x xxxx$ xx xx x xxxxxx xxxxxxxx xxxxxxx xxxx xxx Xxxxxx.Xxxxxxxxxxx.XxxxxXxxxxxxx xxxxx.

Xxxx xxx xxx xxx Xxxxxxx xxxxxxxxx xxx$ Xxxxxxx XxxxxXxxxx xxxxxxxxx xxx xxxxxxx xxxx xx xx xxxxx xx xxxxxxxxx xx x xxxxxxxx.
Xxx xxxxxxx$ xxxxxxx xxxxxxxxx xx xxx xxxxxxxx xxx xxxx xxxxxxxx xxxxxx.

Xxx xxxxx xx xxx Xxxx$ Xxxxxxxxxx$ Xxxxxx$ xxx Xxxxxxx xxxxxxxxxx xxx xxxxxxxx.
Xx xxx xxxx xxx xxxxxxxxx xxxxx$ xxx xxxxxxx xxxxxxxxx xxxxxx xxxx xxxxxx xx xxxx xxxxx$ Xxxx$ Xxxxxxxxxx$ Xxxxxx xx Xxxx$ Xxxxxxx$$Xxxxxx .
Xx xxx xxxxxxx xxx xxxxxxxxx xxxxx$ xxx xxxxxxxxxx xxx xxxxxx xx xxx xxxxx.

## XXXXXXX XXXXX

[Get-TraceSource]()

[Set-TraceSource]()

