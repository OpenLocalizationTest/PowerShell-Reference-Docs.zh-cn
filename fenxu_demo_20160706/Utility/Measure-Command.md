---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293989
schema: 2.0.0
---

# Measure-Command
## XXXXXXXX
Xxxxxxxx xxx xxxx xx xxxxx xx xxx xxxxxx xxxxxx xxx xxxxxxx.

## XXXXXX

```
Measure-Command [-InputObject <PSObject>] [-Expression] <ScriptBlock> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxxx$Xxxxxxx xxxxxx xxxx x xxxxxx xxxxx xx xxxxxx xxxxxxxxxx$ xxxxx xxx xxxxxxxxx xx xxx xxxxxxxxx$ xxx xxxxxxx xxx xxxxxxxxx xxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Measure-Command { Get-EventLog "windows powershell" }
```

Xxxx xxxxxxx xxxxxxxx xxx xxxx xx xxxxx xx xxx x Xxx$XxxxxXxx xxxxxxx xxxx xxxx xxx xxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxx xxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command measures the time it takes to process a recursive Get-ChildItem command that uses the Path parameter to get only .txt files in the C:\Windows directory and its subdirectories.
PS C:\>Measure-Command {Get-ChildItem -Path C:\Windows\*.txt -Recurse}

Days              : 0
Hours             : 0
Minutes           : 0
Seconds           : 8
Milliseconds      : 618
Ticks             : 86182763
TotalDays         : 9.9748568287037E-05
TotalHours        : 0.00239396563888889
TotalMinutes      : 0.143637938333333
TotalSeconds      : 8.6182763
TotalMilliseconds : 8618.2763

The second command measures the time it takes to process a recursive Get-ChildItem command that uses the provider-specific Filter parameter.
PS C:\>Measure-Command {Get-ChildItem C:\Windows -Filter "*.txt" -Recurse}

PS C:\>
Days              : 0
Hours             : 0
Minutes           : 0
Seconds           : 1
Milliseconds      : 140
Ticks             : 11409189
TotalDays         : 1.32050798611111E-05
TotalHours        : 0.000316921916666667
TotalMinutes      : 0.019015315
TotalSeconds      : 1.1409189
TotalMilliseconds : 1140.9189
```

Xxxxx xxxxxxxx xxxx xxx xxxxx xx xxxxx x xxxxxxxx$xxxxxxxx xxxxxx xx Xxxxxxx XxxxxXxxxx xxxxxxxx.

## XXXXXXXXXX

### -Expression
Xxxxxxxxx xxx xxxxxxxxxx xxxx xx xxxxx xxxxx.
Xxxxxxx xxx xxxxxxxxxx xx xxxxxx $$$$.
Xxx xxxxxxxxx xxxx $$Xxxxxxxxxx$$ xx xxxxxxxx.

```yaml
Type: ScriptBlock
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
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
Xxxxxxxxx xxxxxxx xxxxxxxxxxxx xxx xxxxxxxxxxx xx xx xxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.

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

## XXXXXX

### System.Management.Automation.PSObject
Xxx xxx xxxx xx xxxxxx xx Xxxxxxx$Xxxxxxx.

## XXXXXXX

### System.TimeSpan
Xxxxxxx$Xxxxxxx xxxxxxx x xxxx xxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx.

## XXXXX
Xxx xxxx xxxxxxxxxxx$ xxxx $Xxx$Xxxx Xxxxxxx$Xxxxxxx $xxxxxxxx$.
Xxx xxxxxxxxx xxxxxxxxxxx$ xxxx $Xxx$Xxxx Xxxxxxx$Xxxxxxx $xxxx$.

Xxxx xxxxxxxxxx xxxxxxxx xxxxxx xxx x xxxxxxxxx$ xxx xxxxxx xx xxxxxxxx xxx xxxxxx.
Xxx xxxxxxx$ $$$xxxxxxxxx$xxxx$$ $$xxxxx0$$$ $$xxxxx0$$$.

## XXXXXXX XXXXX

[Invoke-Command]()

[Trace-Command]()

