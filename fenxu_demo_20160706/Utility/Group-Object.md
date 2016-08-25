---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293980
schema: 2.0.0
---

# Group-Object
## XXXXXXXX
Xxxxxx xxxxxxx xxxx xxxxxxx xxx xxxx xxxxx xxx xxxxxxxxx xxxxxxxxxx.

## XXXXXX

```
Group-Object [-NoElement] [-AsHashTable] [-AsString] [-InputObject <PSObject>] [[-Property] <Object[]>]
 [-Culture <String>] [-CaseSensitive] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxx$Xxxxxx xxxxxx xxxxxxxx xxxxxxx xx xxxxxx xxxxx xx xxx xxxxx xx x xxxxxxxxx xxxxxxxx.
Xxxxx$Xxxxxx xxxxxxx x xxxxx xxxx xxx xxx xxx xxxx xxxxxxxx xxxxx xxx x xxxxxx xxxx xxxxxxxx xxx xxxxxx xx xxxxx xxxx xxxx xxxxx.

Xx xxx xxxxxxx xxxx xxxx xxx xxxxxxxx$ Xxxxx$Xxxxxx xxxxx xxxxxx xxxx xx xxx xxxxxx xx xxx xxxxx xxxxxxxx$ xxx xxxx$ xxxxxx xxxx xxxxxxxx xxxxx$ xx xxxxxx xx xxx xxxxx xx xxx xxxx xxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem *.doc | group-object -property length
```

Xxxx xxxxxxx xxxx xxx xxxxx xx xxx xxxxxxx xxxxxxxx xxxx xxxx x .xxx xxxxxxxxx xxx xxxxxx xxxx xx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem | sort-object -property extension | group-object -property extension
```

Xxxx xxxxxxx xxxx xxx xxxxx xx xxx xxxxxxx xxxxxxxx$ xxxxx xxxx xx xxxx xxxx xxxxxxxxx$ xxx xxxx xxxxxx xxxx xx xxxx xxxx xxxxxxxxx.
Xxxx xxxx xxx xxxxx xxx xxxxxx xxxxxx xxxx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>1..35 | group-object -property {$_ % 2},{$_ % 3}
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxxxxx xxxxxx xx xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx.

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxx xxxx 0 xx 00$ xxxxxxx xx xxx xxxxxxxxx xxxx xxxx xxxx xxx xxxxxxx xx 0 xx 0.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$events = get-eventlog -logname system -newest 1000
PS C:\>$events | group-object -property eventID

Count Name                      Group
----- ----                      -----
44 Information               {System.Diagnostics.EventLogEntry,
5 Error                     {System.Diagnostics.EventLogEntry,
1 Warning                   {System.Diagnostics.EventLogEntry}
```

Xxxxx xxxxxxxx xxxxxxx xxx 0$000 xxxx xxxxxx xxxxxxx xx xxx Xxxxxx xxxxx xxx$ xxxxxxx xx Xxxxx XX.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XxxxxXxx xxxxxx xx xxxxxxxx xxx xxxxxx xxx xxx xxxxxxxxxx xxxxxxxx $$$ xx xxxx xxxx xx xxx $xxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xx xxx $xxxxxx xxxxxxxx xx xxx Xxxxx$Xxxxxx xxxxxx.
Xxx xxxxxxx xxxx xxx Xxxxxxxx xxxxxxxxx xx xxxxxxx xxxx xxx xxxxxx xxxxxx xx xxxxxxx xxxxxxxxx xx xxx xxxxx xx xxxxx XxxxxXX xxxxxxxx.

Xx xxx xxxxxx$ xxx Xxxxx xxxxxx xxxxxxxxxx xxx xxxxxx xx xxxxxxx xx xxxx xxxxx$ xxx Xxxx xxxxxx xxxxxxxxxx xxx XxxxxXX xxxxxx xxxx xxxxxx x xxxxx$ xxx xxx Xxxxx xxxxxx xxxxxxxxxx xxx xxxxxxx xx xxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | group-object -property priorityclass

Count Name                Group
----- ----                -----
55 Normal              {System.Diagnostics.Process (AdtAgent), System.Diagnostics.Process (alg), System.Dia...
1                     {System.Diagnostics.Process (Idle)}
3 High                {System.Diagnostics.Process (Newproc), System.Diagnostics.Process (winlogon), System.D...
2 BelowNormal         {System.Diagnostics.Process (winperf),

PS C:\>get-process | group-object -property company -noelement

Count Name
----- ----
55 Normal
1
3 High
2 BelowNormal
```

Xxxx xxxxxxx xxxxxxxxxxxx xxx xxxxxx xx xxx XxXxxxxxx xxxxxxxxx.
Xxxxx xxxxxxxx xxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xx xxxxxxxx xxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxxxx xx xxx xxxxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xx Xxxxx$Xxxxxx$ xxxxx xxxxxx xxx xxxxxxx xx xxx xxxxx xx xxx XxxxxxxxXxxxx xxxxxxxx xx xxx xxxxxxx.

Xxx xxxxxx xxxxxxx xx xxxxxxxxx xx xxx xxxxx$ xxxxxx xxxx xx xxxx xxx XxXxxxxxx xxxxxxxxx xx xxxxxxxxx xxx xxxxxxx xx xxx xxxxx xxxx xxx xxxxxx.
Xxx xxxxxx xx x xxxxx xxxx xxxx xxx xxxxx xxx xxxxxxxx xxxxx xxxx.

Xxx xxxxxxx xxx xxxxx xx xxx xxxxxxxxx xxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-eventlog -logname system -newest 1000 | group-object -property {$_.TimeWritten - $_.TimeGenerated}
```

Xxxx xxxxxxx xxxxxxxxxxxx xxx xx xxxxxxx xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx xx x xxxxxx xxxxx.

Xxxx xxxxxxx xxxxxxxx xxx xxxx xxxxxx 0$000 xxxxxxx xxxx xxx xxxxxx xxxxx xxx$ xxxxxxx xxxxxxxxx xx xxx xxxx xxxxxxx xxxx xxxx xxxx xxxxxxxxx xxx xxxx xxxx xxxx xxxxxxx xx xxx xxx.

Xxx xxxxxxx xxxx xxx Xxx$XxxxxXxx xxxxxx xx xxx xxx xxxxx xxx xxxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xx xxx Xxxxx$Xxxxxx xxxxxx.
Xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx xx xxxxxxxxx xx x xxxxxx xxxxx $xx xxxxxxxxxx xx xxxxxx$.
Xxx xxxxxx xx xxxxxxxxxx xxx xxxxxx xxxxx xx xxx xxxx xxxxxxx xxxx xxx xxx xxxxx xxx xxxxxxxxx xxx xxxx xx xxx xxxxxxx xx xxx xxx.
Xxxx xxxxx xx xxxx xx xxxxx xxx 0$000 xxxx xxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem | group-object extension -noelement

Count Name
----- ----
21
82 .txt
9 .cmd
5 .log
12 .xml
5 .htm
36 .ps1
1 .psc1
3 .exe
6 .csv
1 .psd1
2 .bat
```

Xxxx xxxxxxx xxxxxx xxx xxxxx xx xxx xxxxxxx xxxxxxxxx xx xxxx xxxx xxxxxxxxx.
Xx xxxx xxx XxXxxxxxx xxxxxxxxx xx xxxx xxx xxxxxxx xx xxx xxxxx.

Xxx xxxxxxx xxx xxxxx xx xxx xxxxxxxxx xxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>"a", "b", "c", "c", "d" | get-unique
a
b
c
d

PS C:\>"a", "b", "c", "c", "d" | group-object -noelement | where {$_.Count -gt 1}

Count Name
----- ----
2 c

PS C:\>get-process | group-object -property Name -noelement | where {$_.count -gt 1}

Count Name
----- ----
2 csrss
5 svchost
2 winlogon
2 wmiprvse
```

Xxxx xxxxxxx xxxxx xxx xx xxxx xxx xxxxxx xxx xxx$xxxxxx $xxxxxxxx$ xxxxxxxx xxxxxx xx x xxxxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxx xxxxxxxx xx xx xxxxx xx xxxxxx xxx xxxxx xx xxx Xxx$Xxxxxx xxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxx$xxxxxx xxxxxxxx xx xx xxxxx.
Xx xxxxx xxx xxxxx xx xxx Xxxxx$Xxxxxx xxxxxx$ xxxxx xxxxxx xxx xxxxxxx xx xxxxx.
Xxx xxxxxxxxx xxxxxx xxx xxxxx xx xxx Xxxxx$Xxxxxx xxxxxx$ xxxxx xxxxxxx xxxxxxx xxxx xxxxxx xxxx xxxx xxxx xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxxx x xxxxxxxxx xxx xxx xxxx xxxxxxxxx.
Xx xxxx xxx xxxx xxxxxx xx xxxx xxxxxxxxx xx xxx xxxxxxxx xxxx xxxx xxx xxxx xxxxxxx xxxx.

Xxx xxxxxxx xxx xxxxx xx xxx xxxxxxxxx xxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = get-command get-*, set-* -type cmdlet | group-object -property verb -ashashtable -asstring
PS C:\>$a

Name    Value
----    -----
Get     {Get-PSCallStack, Get-PSBreakpoint, Get-PSDrive, Get-PSSession...}
Set     {Set-Service, Set-StrictMode, Set-PSDebug, Set-PSSessionConfiguration...}

PS C:\>$a.get

CommandType     Name                 Definition
-----------     ----                 ----------
Cmdlet          Get-PSCallStack      Get-PSCallStack [-Verbose] [-Debug] [-ErrorAction <ActionPrefer...
Cmdlet          Get-PSBreakpoint     Get-PSBreakpoint [[-Id] <Int32[]>] [-Verbose] [-Debug] [-ErrorA...
Cmdlet          Get-PSDrive          Get-PSDrive [[-Name] <String[]>] [-Scope <String>] [-PSProvider...
...
```

Xxxx xxxxxxx xxxx xxx XxXxxxXxxxx xxx XxXxxxxx xxxxxxxxxx xx xxxxxx xxx xxxxxx xx x xxxx xxxxx$ xxxx xx$ xx x xxxxxxxxxx xx xxx$xxxxx xxxxx.

Xx xxx xxxxxxxxx xxxx xxxxx$ xxxx xxxxxxxx xxxxx xx x xxx$ xxx xxx xxxxx xxxxxxxx xxx xxx xxxxxx.
Xxxxxxx xxxx xxx xx x xxxxxxxx xx xxx xxxx xxxxx xxxxxx$ xxx xxx xxx xxx xxxxxxxx xx xxxxxxx xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx xxx Xxx xxxxxxx xx xxx xxxxxxx$ xxxxxx xxxx xx xxxx$ xxxxxxx xxx xxxxxx xx x xxxx xxxxx$ xxx xxxxx xxx xxxx xxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxxx xxx xxxx xxxxx xx $x.
Xxxxx xxx xxx xxx$xxxxx xxxxx$ xxx xxx xxx Xxx xxxxxxx xxx xxx xxx xxx Xxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxxxxxx xxx xxxxxx xx xxx Xxx xxx xx $x.
Xxx xxxxxx xxx XxxxxxXxxx xxxxxx.
Xxx XxXxxxxx xxxxxxxxx xxxx xxx xxxxxxx xxx xxxxxxx xx xxx xxxxxx xx xxxxxxx.

## XXXXXXXXXX

### -AsHashTable
Xxxxxxx xxx xxxxx xx x xxxx xxxxx. Xxx xxxx xx xxx xxxx xxxxx xxx xxx xxxxxxxx xxxxxx xx xxxxx xxx xxxxxxx xxx xxxxxxx.
Xxx xxxxxx xx xxx xxxx xxxxx xxx xxx xxxxxxx xxxx xxxx xxxx xxxxxxxx xxxxx.

Xx xxxxxx$ xxx XxXxxxXxxxx xxxxxxxxx xxxxxxx xxxx xxxx xxxxx xx xxxxx xxxx xxx xx xx xxxxxxxx xx xxx xxxxxxx xxxxxx.
Xxxx xxxx xxxx xxx  XxXxxxxx xxxxxxxxx$ xxx xxxx xx xxx xxxx xxxxx xxx xxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: AHT

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AsString
Xxxxxxxx xxx xxxx xxxxx xxxx xx xxxxxxx.
Xx xxxxxxx$ xxx xxxx xxxxx xxxx xxx xxxxxxxxx xx xxx xxxxxxx xxxxxx.
Xxxx xxxxxxxxx xx xxxxx xxxx xxxx xxxx xxxx xxx XxXxxxXxxxx xxxxxxxxx.

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

### -CaseSensitive
Xxxxx xxx xxxxxxxx xxxx$xxxxxxxxx.
Xxxxxxx xxxx xxxxxxxxx$ xxx xxxxxxxx xxxxxx xx xxxxxxx xx x xxxxx xxxxx xxxx xxxxxxxxx xxxxx.

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

### -Culture
Xxxxxxxxx xxx xxxxxxx xx xxx xxxx xxxxxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
Xx xxxxxx$ xxx XxXxxxXxxxx xxxxxxxxx xxxxxxx xxxx xxxx xxxxx xx xxxxx xxxx xxx xx xx xxxxxxxx xx xxx xxxxxxx xxxxxx.
Xxxx xxxx xxxx xxx  XxXxxxxx xxxxxxxxx$ xxx xxxx xx xxx xxxx xxxxx xxx xxxxxxx.

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
Xx xxxxxx$ xxx XxXxxxXxxxx xxxxxxxxx xxxxxxx xxxx xxxx xxxxx xx xxxxx xxxx xxx xx xx xxxxxxxx xx xxx xxxxxxx xxxxxx.
Xxxx xxxx xxxx xxx  XxXxxxxx xxxxxxxxx$ xxx xxxx xx xxx xxxx xxxxx xxx xxxxxxx.

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
Xxxxxxxxx xxx xxxxxxx xx xxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx$ xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.

Xxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxx x xxxxxxxxxx xx xxxxxxx xx Xxxxx$Xxxxxx$ Xxxxx$Xxxxxx xxxxxxxx xxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxxxxx.
Xx x xxxxxx$ xx xxxxxxx x xxxxxx xxxxx xxxx xxxx xxxxxx xx xxx xxxxxx.

Xx xxxxx xxx xxxxxxx xx x xxxxxxxxxx$ xxxx xxx xxxxxxx xx Xxxxx$Xxxxxx.

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

### -NoElement
Xxxxx xxx xxxxxxx xx x xxxxx xxxx xxx xxxxxxx.

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

### -Property
Xxxxxxxxx xxx xxxxxxxxxx xxx xxxxxxxx.
Xxx xxxxxxx xxx xxxxxxxx xxxx xxxxxx xxxxx xx xxx xxxxx xx xxx xxxxxxxxx xxxxxxxx.

Xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx xxx xx x xxx xxxxxxxxxx xxxxxxxx.
Xx xxxxxx x xxxxxxxxxx$ xxxxxxxx$ xxxxxx x xxxx xxxxx xxxx xx Xxxxxxxxxx xxx xxxx xxxxxxxxx x xxxxxx xx xxxxxx xxxxx xxxxx.

```yaml
Type: Object[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.Management.Automation.PSObject
Xxx xxx xxxx xxx xxxxxx xx Xxxxx$Xxxxxx

## XXXXXXX

### Microsoft.PowerShell.Commands.GroupInfo or System.Collections.Hashtable
Xxxx xxx xxx xxx XxXxxxXxxxx xxxxxxxxx$ Xxxxx$Xxxxxx xxxxxxx x xxxx xxxxx.
Xxxxxxxxx$ xx xxxxxxx x XxxxxXxxx xxxxxx.

## XXXXX
Xxx xxx xxxx xxx xxx XxxxxXx xxxxxxxxx xx xxx xxxxxxxxxx xxxxxxx $xxxx xx Xxxxxx$Xxxxx $$x0$$ xxx Xxxxxx$Xxxx $$x0$$$ xx xxxxx xxxxxxx.
Xxxxxx Xxxxx$Xxxxxx$ xxxxx xxxxxxx x xxxxxx xxxxx xxxx x xxx xxx xxxx xxxxxxxx xxxxx$ xxx XxxxxXx xxxxxxxxxx xxxxxx x xxxxx xxx xxxx xxxxxxxx xxxxx xxxx x xxx xxx xxxx xxxx xxxx xxx xxx xxxxxxxx xxxxx.

Xxxxx$Xxxxxx xxxx xxx xxxxxxx xxxx xxx xxxxxxx xxxxx xxxxxxx xx xx xxx xxxx Xxxxxxxxx .XXX Xxxxxxxxx xxxx.
Xxxx xxxxxxxx xxxxxxx xx xxxxxxxxx .XXX Xxxxxxxxx xxxxx$ Xxxxx$Xxxxxx xxxx xxx xxxxxxxxx xxxxx$

$$ Xxxx Xxxxxxxx Xxxxx xxx Xxxxx$ Xx xxx xxxxxxx xxxx x xxxxxxxx xxxx xxx xxxxxxxxx xxxx$ xxx xxx xxxxxxxx xxxxxx xxxx xxx xxxx .XXX Xxxxxxxxx xxxx$ xxx xxxxxxxx xxxxxx xxx xxxxxxx xx xxxxx xxx xxxx xxxxx xxxx xxxxx xx xxxx xxx xxxxxxx xx xxx xxxx xxxx.
$$ Xxxx Xxxxxxxx Xxxxx$ Xxxxxxxxx Xxxxx$ Xx xxx xxxxxxx xxxx x xxxxxxxx xxxx xxx xxxxxxxxx xxxx$ xxx xxx xxxxxxxx xxxxxx xxxx x xxxxxxxxx .XXX Xxxxxxxxx xxxx xx xxxxxxxxx xxxxxxx$ Xxxxx$Xxxxxx xxxx xxx .XXX Xxxxxxxxx xxxx xx xxx xxxxx xxxxxxxxxx xx xxx xxxxxxxx xx xxx .XXX Xxxxxxxxx xxxx xxx xxxx xxxxxxxx xxxxx. Xxxx xx xxxxxx xxx x xxxxxxxx xxxx x xxxxxxxxx xxxx$ xxx xxxxxxxx xxxxx xx xxxxxxxxx xx xxx xxxx xxx xxxx xxxxx. Xx xxx xxxx xxxxxxxxxx xxxxx$ xxx xxxxxx xx xxx xxxxxxxx xx xxx xxxxx.
$$ Xxxxxxx Xxxxxxxxxx$ Xxxxxxx xxxx xx xxx xxxx x xxxxxxxxx xxxxxxxx xxx xxxxxxxxxx xxxxxxxxxxx. Xxxxxxxxxxx xxxxxxx xxxxxx xx xxx xxxxx XxxxxXxxx xxxxxx xxxxxx xx x xxxxx xxxxx XxxxxxxxxxXxxx.Xxxxx.

## XXXXXXX XXXXX

