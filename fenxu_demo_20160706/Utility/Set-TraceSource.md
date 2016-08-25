---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294014
schema: 2.0.0
---

# Set-TraceSource
## XXXXXXXX
Xxxxxxxxxx$ xxxxxx$ xxx xxxxx x xxxxx xx Xxxxxxx XxxxxXxxxx xxxxxxxxxx.

## XXXXXX

### optionsSet (Default)
```
Set-TraceSource [-Name] <String[]> [[-Option] <PSTraceSourceOptions>] [-ListenerOption <TraceOptions>]
 [-FilePath <String>] [-Force] [-Debugger] [-PSHost] [-PassThru] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### removeAllListenersSet
```
Set-TraceSource [-Name] <String[]> [-RemoveListener <String[]>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### removeFileListenersSet
```
Set-TraceSource [-Name] <String[]> [-RemoveFileListener <String[]>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$XxxxxXxxxxx xxxxxx xxxxxxxxxx$ xxxxxx$ xxx xxxxx x xxxxx xx x Xxxxxxx XxxxxXxxxx xxxxxxxxx.
Xxx xxx xxx xx xx xxxxxxx xxxxx xxxxxxxxxx xxxx xx xxxxxx xxx xxxxx xxx xxxxxxx xxxxxx xx xxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Set-TraceSource -Name Parameterbinding -Option ExecutionFlow -PSHost -ListenerOption "ProcessID,TimeStamp"
```

Xxxx xxxxxxx xxxxxx xxxxxxx xxx xxx XxxxxxxxxXxxxxxx xxxxxxxxx xx Xxxxxxx XxxxxXxxxx.
Xx xxxx xxx Xxxx xxxxxxxxx xx xxxxxxx xxx xxxxx xxxxxx$ xxx Xxxxxx xxxxxxxxx xx xxxxxx xxx XxxxxxxxxXxxx xxxxx xxxxxx$ xxx xxx XXXxxx xxxxxxxxx xx xxxxxx xxx Xxxxxxx XxxxxXxxxx xxxx xxxxxxxx$ xxxxx xxxxx xxx xxxxxx xx xxx xxxxxxx.
Xxx XxxxxxxxXxxxxx xxxxxxxxx xxxx xxx $XxxxxxxXX$ xxx $XxxxXxxxx$ xxxxxx xx xxx xxxxx xxxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-tracesource -name ParameterBinding -RemoveListener Host
```

Xxxx xxxxxxx xxxxx xxx xxxxx xx xxx XxxxxxxxxXxxxxxx xxxxxxxxx xx Xxxxxxx XxxxxXxxxx.
Xx xxxx xxx Xxxx xxxxxxxxx xx xxxxxxxx xxx xxxxxxxxx xxxx xxx xxxxx xxxxxx xxx xxx XxxxxxXxxxxxxx xxxxxxxxx xx xxxxxxxx xxx xxxxx xxxxxxxx.

## XXXXXXXXXX

### -Debugger
Xxxxx xxx xxxxx xxxxxx xx xxx xxxxxxxx.
Xxx xxx xxxx xxx xxxxxx xx xxx xxxx$xxxx xx xxxxxx xxxx xxxxxxxx xx xx Xxxxxxxxx Xxxxxx Xxxxxx.
Xxxx xxxxxxxxx xxxx xxxxxxx xxx xxxxxxx xxxxx xxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: optionsSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FilePath
Xxxxx xxx xxxxx xxxxxx xx xxx xxxxxxxxx xxxx.
Xxxx xxxxxxxxx xxxx xxxxxxx xxx xxxx xxxxx xxxxxxxx.
Xx xxx xxx xxxx xxxxxxxxx xx xxxxx xxx xxxxx$ xxx xxx XxxxxxXxxxXxxxxxxx xxxxxxxxx xx xxxx xxx xxxxx.

```yaml
Type: String
Parameter Sets: optionsSet
Aliases: PSPath

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Xxxxxx xxx xxxxxx xx xxxxxxxxx x xxxx$xxxx xxxx.
Xxx xxxx xxx XxxxXxxx xxxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: optionsSet
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

### -ListenerOption
Xxxx xxxxxxxx xxxx xx xxx xxxxxx xx xxxx xxxxx xxxxxxx xx xxx xxxxxx.
Xxx xxxxx xxxxxx xxx $Xxxx$$ $XxxxxxxXxxxxxxxxXxxxx$$ $XxxxXxxx$$ $Xxxxxxxxx$$ $XxxxxxxXx$$ $XxxxxxXx$$ xxx $Xxxxxxxxx$.
$Xxxx$ xx xxx xxxxxxx.

Xx xxxxxxx xxxxxxxx xxxxxxx$ xxxxxxxx xxxx xxxx xxxxxx$ xxx xxxx xx xxxxxx$ xxx xxxxxxx xxxx xx xxxxxxxxx xxxxx$ xxxx xx $XxxxxxxXX$XxxxxxXX$.

```yaml
Type: TraceOptions
Parameter Sets: optionsSet
Aliases: 
Accepted values: None, Constructor, Dispose, Finalizer, Method, Property, Delegates, Events, Exception, Lock, Error, Errors, Warning, Verbose, WriteLine, Data, Scope, ExecutionFlow, Assert, All

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Xxxxxxxxxx xxxxx xxxxxxxxxx xxx xxxxxx.
Xxxxx xxx xxxx xx xxx xxxxx xxxxxx xx xxxx xxxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Option
Xxxxxxxxxx xxx xxxx xx xxxxxx xxxx xxx xxxxxx.

Xxx xxxxx xxxxxx xxx$ Xxxx$ Xxxxxxxxxxx$ Xxxxxxx$ Xxxxxxxxx$ Xxxxxx$ Xxxxxxxx$ Xxxxxxxxx$ Xxxxxx$ Xxxxxxxxx$ Xxxx$ Xxxxx$ Xxxxxx$ Xxxxxxx$ Xxxxxxx$ XxxxxXxxx$ Xxxx$ Xxxxx$ XxxxxxxxxXxxx$ Xxxxxx$ xxx Xxx.
Xxx xx xxx xxxxxxx.

Xxx xxxxxxxxx xxxxxx xxx xxxxxxxxxxxx xx xxxxx xxxxxx$

$$ XxxxxxxxxXxxx$ $Xxxxxxxxxxx$ Xxxxxxx$ Xxxxxxxxx$ Xxxxxx$ Xxxxxxxxx$ Xxxxxx$ xxx Xxxxx$ $$ Xxxx$ $Xxxxxxxxxxx$ Xxxxxxx$ Xxxxxxxxx$ Xxxxxxxx$ Xxxxxxx$ xxx XxxxxXxxx$ $$ Xxxxxx$ $Xxxxx xxx Xxxxxxxxx$.

Xx xxxxxxx xxxxxxxx xxxxxxx$ xxxxxxxx xxxx xxxx xxxxxx$ xxx xxxx xx xxxxxx$ xxx xxxxxxx xxxx xx xxxxxxxxx xxxxx$ xxxx xx $Xxxxxxxxxxx$Xxxxxxx$.

```yaml
Type: PSTraceSourceOptions
Parameter Sets: optionsSet
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PSHost
Xxxxx xxx xxxxx xxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxx.
Xxxx xxxxxxxxx xxxx xxxxxxx xxx XXXxxx xxxxx xxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: optionsSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Xxxxxxx xx xxxxxx xxxxxxxxxxxx xxx xxxxx xxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: optionsSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoveFileListener
Xxxxx xxx xxxxx xx xxxxxxxx xxx xxxx xxxxx xxxxxxxx xxxxxxxxxx xxxx xxx xxxxxxxxx xxxx.
Xxxxx xxx xxxx xxx xxxx xxxx xx xxx xxxxx xxxxxx xxxx.

```yaml
Type: String[]
Parameter Sets: removeFileListenersSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoveListener
Xxxxx xxx xxxxx xx xxxxxxxx xxx xxxxx xxxxxxxx.

Xxx xxx xxxxxxxxx xxxxxx xxxx XxxxxxXxxxxxxx$

$$Xx xxxxxx XXXxxx $xxxxxxx$$ xxxx $Xxxx$.
$$Xx xxxxxx Xxxxxxxx$ xxxx $Xxxxx$.
$$Xx xxxxxx xxx xxxxx xxxxxxxxx$ xxxx $$$.

Xx xxxxxx xxx xxxx xxxxx xxxxxxxx$ xxx xxx XxxxxxXxxxXxxxxxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: removeAllListenersSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.String
Xxx xxx xxxx x xxxxxx xxxx xxxxxxxx x xxxx xx Xxx$XxxxxXxxxxx.

## XXXXXXX

### None or System.Management.Automation.PSTraceSource
Xxxx xxx xxx xxx XxxxXxxx xxxxxxxxx$ Xxx$XxxxxXxxxxx xxxxxxxxx x Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxXxxxxx xxxxxx xxxxxxxxxxxx xxx xxxxx xxxxxxx.
Xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xxxxxxx xx x xxxxxx xxxx xxxxxxxxxx xxx xx xxxxx xxx xxxxxx xxxxxxxx.
Xxxx xxxxxxx$ xxx xxxxxxx xxxxxxxxx xxxxxxxx xxxxxxxx xxxxx xxxx xxxx xx xxx xxxxxxxx xxxxxxxxxx.

Xxx Xxxxxxx XxxxxXxxxx xxxxxxx xxxxxxx xxx xxxxxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxxxxx$ xxx xxxx xxx xxxxxxxxx xx xxx xxxxx.
Xxxx xxx xxx xxxxxxx xxxxxx xxxxx xxxxxx xx xxx xxxxxxxxxxxxx xx Xxxxxxx XxxxxXxxxx.

X $xxxxx xxxxxx$ xx xxx xxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxxxx xxxx xxxxxxx xxxxxxx xxx xxxxxxxxx xxxxx xxxxxxxx xxx xxx xxxxxxxxx.
Xx xxxxx x xxxxxxxxx$ xxx xxxxxxxx xxx xxxxx xxxxxx.

X $xxxxx xxxxxxxx$ xxxxxxxx xxx xxxxxx xx xxx xxxxx xxx xxxxxxxx xx xx xxx xxxx.
Xxx xxx xxxxx xx xxxx xxx xxxxx xxxx xx x xxxx$xxxx xx xxxxxx$xxxx xxxxxxxx$ xx xxx xxxxxxx$ xx x xxxx$ xx xx x xxxxxx xxxxxxxx xxxxxxx xxxx xxx Xxxxxx.Xxxxxxxxxxx.XxxxxXxxxxxxx xxxxx.

Xx xxxxx x xxxxx$ xxx xxx Xxxx xxxxxxxxx xx xxxxxxx x xxxxx xxxxxx $xxx xxxxxxxxx xx xx xxxxxx$ xxx xxx XxxxXxxx$ Xxxxxxxx$ xx XXXxxx xxxxxxxxxx xx xxxxxxx x xxxxxxxx $x xxxxxxxxxxx xxx xxx xxxxxx$.
Xxx xxx Xxxxxxx xxxxxxxxx xx xxxxxxxxx xxx xxxxx xx xxxxxx xxxx xxx xxxxxx xxx xxx XxxxxxxxXxxxxxx xxxxxxxxx xx xxxxxxxxx xxx xxxxx xxxxxx.

Xx xxxxxx xxx xxxxxxxxxxxxx xx x xxxxx$ xxxxx x Xxx$XxxxxXxxxxx xxxxxxx xx xxx xxxxx xx xxxxx x xxxxx.
Xxxxxxx XxxxxXxxxx xxxxxxxxxx xxxx xxx xxxxx xxxxxx xx xxxxxxx xxxxx xxxxxx.
Xx xxxxx xxx xxxxx$ xxxx xxx xxx xxxxxxxxxxxxx$ xxx xxxxxx xx xxxxxxxx xxx xxxxx.

Xx xxxx x xxxxx$ xxx xxx XxxxxxXxxxxxxx xxxxxxxxx.
Xx xxxx x xxxxx xxxx xxxx xxx xxxx xxxxxxxx $x xxxxx xxxxxxx xx xxxxx xxx $XxxxXxxx xxxxxxxxx$$ xxx xxx XxxxxxXxxxXxxxxxxx xxxxxxxxx.
Xxxx xxx xxxxxx xxx xxxxxxxx$ xxx xxxxx xxxxx.

Xx xxxxxxxxx xxxxx xxxxxxxxxx xxx xx xxxxxx$ xxx Xxx$XxxxxXxxxxx.
Xxx xxxxx xxxxxxx xxx xxxx xxxxxx xxx xxxxxx xxxxxxxxxxxxx xxxx xxx xxxxxxxxx xx xx xxx$ xxx xxxx xxxxxx xx xxx xxxxxx xx Xxx$XxxxxXxxxxx.

## XXXXXXX XXXXX

[Get-TraceSource]()

[Set-PSDebug]()

[Trace-Command]()

