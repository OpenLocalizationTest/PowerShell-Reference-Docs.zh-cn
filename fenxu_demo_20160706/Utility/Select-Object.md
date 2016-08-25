---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294007
schema: 2.0.0
---

# Select-Object
## XXXXXXXX
Xxxxxxx xxxxxxx xx xxxxxx xxxxxxxxxx.

## XXXXXX

### DefaultParameter (Default)
```
Select-Object [-InputObject <PSObject>] [[-Property] <Object[]>] [-ExcludeProperty <String[]>]
 [-ExpandProperty <String>] [-Unique] [-Last <Int32>] [-First <Int32>] [-Skip <Int32>] [-Wait]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### SkipLastParameter
```
Select-Object [-InputObject <PSObject>] [[-Property] <Object[]>] [-ExcludeProperty <String[]>]
 [-ExpandProperty <String>] [-Unique] [-SkipLast <Int32>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### IndexParameter
```
Select-Object [-InputObject <PSObject>] [-Unique] [-Wait] [-Index <Int32[]>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxxxxx xxxxxx xxxxxxx xxxxxxxxx xxxxxxxxxx xx xx xxxxxx xx xxx xx xxxxxxx.
Xx xxx xxxx xxxxxx xxxxxx xxxxxxx$ x xxxxxxxxx xxxxxx xx xxxxxxx$ xx xxxxxxx xx x xxxxxxxxx xxxxxxxx xx xx xxxxx.

Xx xxxxxx xxxxxxx xxxx x xxxxxxxxxx$ xxx xxx Xxxxx$ Xxxx$ Xxxxxx$ Xxxx$ xxx Xxxxx xxxxxxxxxx.
Xx xxxxxx xxxxxx xxxxxxxxxx$ xxx xxx Xxxxxxxx xxxxxxxxx.
Xxxx xxx xxxxxx xxxxxxxxxx$ Xxxxxx$Xxxxxx xxxxxxx xxx xxxxxxx xxxx xxxx xxxx xxx xxxxxxxxx xxxxxxxxxx.

Xxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ Xxxxxx$Xxxxxx xxxxxxxx xx xxxxxxxxxxxx xxxxxxx xxxx xxxxxxxx xxxxxxxx xxxx xxxxxxxx xxx xxxxxxxxxx xxxxxxx xxxx xxx xxx xxxx.
Xxxx xxx xxxxxxx x Xxxxxx$Xxxxxx xxxxxxx xxxx xxx Xxxxx xx Xxxxx xxxxxxxxxx xx x xxxxxxx xxxxxxxx$ Xxxxxxx XxxxxXxxxx xxxxx xxx xxxxxxx xxxx xxxxxxxxx xxx xxxxxxx xx xxxx xx xxx xxxxxxxx xxxxxx xx xxxxxxx xx xxxxxxxxx$ xxxx xxxx xxx xxxxxxx xxxx xxxxxxxxx xxx xxxxxxx xxxxxxx xxxxxx xxx Xxxxxx$Xxxxxx xxxxxxx xx xxx xxxxxxxx.
Xx xxxx xxx xxxx xxxxxxxxxx xxxxxxxx$ xxx xxx Xxxx xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Process | Select-Object -Property ProcessName, Id, WS
```

Xxxx xxxxxxx xxxxxxx xxxxxxx xxxx xxxx xxx Xxxx$ XX$ xxx xxxxxxx xxx $XX$ xxxxxxxxxx xx xxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Process Explorer | Select-Object -Property ProcessName -ExpandProperty Modules | Format-List

ProcessName       : 00THotkey
Size              : 256
Company           : TOSHIBA Corporation
FileVersion       : 1, 0, 0, 27
ProductVersion    : 6, 2, 0, 0
Description       : THotkey
Product           : TOSHIBA THotkey
ModuleName        : 00THotkey.exe
FileName          : C:\WINDOWS\system32\00THotkey.exe
BaseAddress       : 4194304
```

Xxxx xxxxxxx xxxx xxxxxxxxxxx xxxxx xxx xxxxxxx xxxx xx xxx xxxxxxxxx xx xxx xxxxxxxx.
Xx xxxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxx xx xxx xxxxxxxx.
Xx xxxx xxx Xxxxxx$Xxxxxx xxxxxx xx xxxxxx xxx xxxxxxx xxxx xxxx xxx xxxxxxxx xxxxxxxxxx.
Xxx xxxxxxx xxxx xxx Xxxxxxxx xxxxxxxxx xx xxx Xxxxxx$Xxxxxx xxxxxx xx xxxxxx xxx xxxxxxx xxxxx.
Xxxxxxx xxx Xxxxxxx xxxxxxxx xxxxxxxx xx XxxxxxXxxxxxx xxxxxx xxxx xxx xxxx xxxxxxxxxx$ xxx xxxxxxx xxxx xxx XxxxxxXxxxxxxx xxxxxxxxx xx xxx xxx xxxxxxxxxx xx xxx xxxxxxx xx xxx Xxxxxxx xxxxxxxx xx xxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx Xxxxxx$Xxxx xxxxxxxxx xx xxxxxxx xxx xxxx xxx xxxxxxx xx xx xxxx xxxxxxx xx x xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Process | Sort-Object -Property WS | Select-Object -Last 5

Handles  NPM(K)    PM(K)      WS(K) VS(M)   CPU(s)     Id ProcessName
-------  ------    -----      ----- -----   ------     -- -----------
2866     320       33432      45764   203   222.41   1292 svchost
577      17        23676      50516   265    50.58   4388 WINWORD
826      11        75448      76712   188    19.77   3780 Ps
1367     14        73152      88736   216    61.69    676 Ps
1612     44        66080      92780   380   900.59   6132 INFOPATH
```

Xxxx xxxxxxx xxxx xxx xxxx xxxxxxxxx xxxx xxx xxxxx xxx xxxx xxxxxx.
Xxx Xxx$Xxxxxxx xxxxxx xxxx xxx xxxxxxxxx xx xxx xxxxxxxx.
Xxx Xxxx$Xxxxxx xxxxxx xxxxx xxx xxxxxxxxx xxxxxxxxx xx xxxxxx $xxxxxxx xxx$ xxxxx$ xxx xxx Xxxxxx$Xxxxxx xxxxxx xxxxxxx xxxx xxx xxxx xxxx xxxxxxx xx xxx xxxxxxxxx xxxxx xx xxxxxxx.

Xxx Xxxx xxxxxxxxx xx xxx xxxxxxxx xx xxxxxxxx xxxx xxxxxxx xxx Xxxx$Xxxxxx xxxxxx xxxxxxx Xxxx$Xxxxxx xxxxxxxxx xxx xxxxxxx xxx xxxx xxxxxxx x xxxxxxxxxx.
Xxx Xxxxxx$Xxxxxx xxxxxxxxxxxx xx xxxxxxxxx xxxx xxx xxxxxxxx xxxx xxxxxx xxxxxxx xxxxxxxxxxxx xx xxxx xxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-process | Select-Object -Property ProcessName,@{Name="Start Day"; Expression = {$_.StartTime.DayOfWeek}}

ProcessName  StartDay
----         --------
alg          Wednesday
ati2evxx     Wednesday
ati2evxx     Thursday
...
```

Xxxx xxxxxxx xxxx xxx xxxx xxx xxxxx xxx xx xxx xxxxxxxxx xxxxxxx xx x xxxxxxxx.

Xxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxxxx xx xxx xxxxxxxx.
Xx xxxxxx xxx xxxxxxxxx xx xxx Xxxxxx$Xxxxxx xxxxxx$ xxxxx xxxxxxx xxxxxxx xxxx xxxx xxxx xxx XxxxxxxXxxx xxxxxxxxx xxx x xxxxxxxxxx xxxxxxxx xxxxx $Xxxxx Xxx.$ Xxx $Xxxxx Xxx$ xxxxxxxx xx xxxxx xx xxxxx x xxxx xxxxx xxxx Xxxx xxx Xxxxxxxxxx xxxx.
Xxx xxxxx xx xxx Xxxxxxxxxx xxx xx x xxxxxx xxxxxx xxxx xxxx xxx XxxxxXxxx xxxxxxxx xx xxxx xxxxxxx xxx xxx XxxxxXxxx xxxxxxxx xx xxx XxxxxXxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>"a","b","c","a","a","a" | Select-Object -Unique

a
b
c
```

Xxxx xxxxxxx xxxx xxx Xxxxxx xxxxxxxxx xx Xxxxxx$Xxxxxx xx xxx xxxxxx xxxxxxxxxx xxxx xx xxxxx xx xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = Get-Eventlog -Log "Windows PowerShell"
PS C:\>$a | select-object -index 0, ($a.count - 1)
```

Xxxxx xxxxxxxx xxxx xxx xxxxx $xxxxxx$ xxx xxxx $xxxxxx$ xxxxxx xx xxx Xxxxxxx Xxxxxxxxxx xxxxx xxx.

Xxx xxxxxxx xxxx xxx Xxx$XxxxxXxx xxxxxx xx xxx xxx xxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxx.
Xx xxxxx xxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xx $x xx xxx Xxxxxx$Xxxxxx xxxxxx.
Xxx Xxxxxx$Xxxxxx xxxxxxx xxxx xxx Xxxxx xxxxxxxxx xx xxxxxx xxxxxx xxxx xxx xxxxx xx xxxxxx xx xxx $x xxxxxxxx.
Xxx xxxxx xx xxx xxxxx xxxxx xx 0.
Xxx xxxxx xx xxx xxxx xxxxx xx xxx xxxxxx xx xxxxx xx $x xxxxx 0.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>New-PSSession -ComputerName (Get-Content Servers.txt | Select-Object -Skip 1)
```

Xxxx xxxxxxx xxxxxxx x xxx XXXxxxxxx xx xxxx xx xxx xxxxxxxxx xxxxxx xx xxx Xxxxxxx.xxx xxxxx$ xxxxxx xxx xxx xxxxx xxx.

Xxxx xxxxxxx xxxx xxx Xxxxxx$Xxxxxx xxxxxx xx xxxxxx xxx xxx xxx xxxxx xxxxxxxx xx x xxxx xx xxxxxxxx xxxxx.
Xxx xxxxxxxxx xxxx xx xxxxxxxxx xx xxx xx xxx xxxxx xx xxx XxxxxxxxXxxx xxxxxxxxx xx xxx Xxx$XXXxxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-ChildItem *.txt -ReadOnly | Rename-Item -NewName {$_.BaseName + "-ro.txt"} -PassThru | Select-Object -First 5 -Wait
```

Xxxx xxxxxxx xxxx x $$xx$ xxxxxx xx xxx xxxx xxxxx xx xxxx xxxxx xxxx xxxx xxx xxxx$xxxx xxxxxxxxx xxx xxxx xxxxxxxx xxx xxxxx xxxx xxxxx xx xxx xxxx xxx xxx x xxxxxx xx xxx xxxxxx.

Xxx xxxxxxx xxxx xxx XxxxXxxx xxxxxxx xxxxxxxxx xx xxx Xxx$XxxxxXxxx xxx XxxxXxxxxx xxxxxx xx xxx xxxx$xxxx xxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxx xx xxx Xxxxxx$Xxxx xxxxxx$ xxxxx xxxxxxx xxx xxxx.
Xx xxxx xxx Xxxxxxxx xxxxxxxxx xx Xxxxxx$Xxxx xx xxxx xxx xxxxxxx xxxxx xx xxx Xxxxxx$Xxxxxx xxxxxx$ xxxxx xxxxxxx xxx xxxxx 0 xxx xxxxxxx.

Xxx Xxxx xxxxxxxxx xx Xxxxxx$Xxxxxx xxxxxxxx Xxxxxxx XxxxxXxxxx xxxx xxxxxxxx xxx Xxx$XxxxxXxxx xxxxxx xxxxx xx xxxx xxx xxxxx xxxx xxxx$xxxx xxxx xxxxx.
Xxxxxxx xxxx xxxxxxxxx$ xxxx xxx xxxxx xxxx xxxx$xxxx xxxxx xxxxx xx xxxxxxx.

## XXXXXXXXXX

### -ExcludeProperty
Xxxxxxx xxx xxxxxxxxx xxxxxxxxxx xxxx xxx xxxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxxx xxxx xxxx xxx xxxxxxx xxxx xxxxxxxx xxx Xxxxxxxx xxxxxxxxx.

Xxx xxxxx xx xxx xxxxxxxx xxxxxxxxx xxx xx x xxxxxxxxxx xxxxxxxx$ xxxxx xx x xxxx xxxxx xxxx xxxxxxxxx x xxxx xxx xxxxxxxxxx x xxxxx xxx xxx xxxxxxxx xxxxxxx.
Xxxxx xxxx xxx$

$$ Xxxx xx Xxxxx $$xxxxxx$$$$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxxxxxxx\>

Xxx xxxx xxxxxxxxxxx$ xxx xxx xxxxxxxx.

```yaml
Type: String[]
Parameter Sets: DefaultParameter, SkipLastParameter
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpandProperty
Xxxxxxxxx x xxxxxxxx xx xxxxxx$ xxx xxxxxxxxx xxxx xx xxxxxxx xxxxxx xx xxxx xx xxxxxx xxxx xxxxxxxx. Xxxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xxxx.

Xxx xxxxxxx$ xx xxx xxxxxxxxx xxxxxxxx xx xx xxxxx$ xxxx xxxxx xx xxx xxxxx xx xxxxxxxx xx xxx xxxxxx.
Xx xxx xxxxxxxx xxxxxxxx xx xxxxxx$ xxx xxxxxxxxxx xx xxxx xxxxxx xxx xxxxxxxxx xx xxx xxxxxx.

```yaml
Type: String
Parameter Sets: DefaultParameter, SkipLastParameter
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Index
Xxxxxxx xxxxxxx xxxx xx xxxxx xxxxx xx xxxxx xxxxx xxxxxx.
Xxxxx xxx xxxxxxx xx x xxxxx$xxxxxxxxx xxxx.

Xxxxxxx xx xx xxxxx xxxxx xxxx 0$ xxxxx 0 xxxxxxxxxx xxx xxxxx xxxxx xxx $x$0$ xxxxxxxxxx xxx xxxx xxxxx.

```yaml
Type: Int32[]
Parameter Sets: IndexParameter
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
Xxx xxxxx xx xxx xxxxxxxx xxxxxxxxx xxx xx x xxxxxxxxxx xxxxxxxx$ xxxxx xx x xxxx xxxxx xxxx xxxxxxxxx x xxxx xxx xxxxxxxxxx x xxxxx xxx xxx xxxxxxxx xxxxxxx.
Xxxxx xxxx xxx$

$$ Xxxx xx Xxxxx $$xxxxxx$$$$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxxxxxxx\>

Xxx xxxx xxxxxxxxxxx$ xxx xxx xxxxxxxx.

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
Xxx xxxxx xx xxx xxxxxxxx xxxxxxxxx xxx xx x xxxxxxxxxx xxxxxxxx$ xxxxx xx x xxxx xxxxx xxxx xxxxxxxxx x xxxx xxx xxxxxxxxxx x xxxxx xxx xxx xxxxxxxx xxxxxxx.
Xxxxx xxxx xxx$

$$ Xxxx xx Xxxxx $$xxxxxx$$$$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxxxxxxx\>

Xxx xxxx xxxxxxxxxxx$ xxx xxx xxxxxxxx.

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
Xxxxxxxxx xxxxxxx xx xxxx xx xxx xxxxxx xxxxxxx xxx xxxxxxxx.
Xxxx xxxxxxxxx xxxxxxx xxx xx xxxx xxxxxxx xx Xxxxxx$Xxxxxx.

Xxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xxxx Xxxxxx$Xxxxxx$ xxxxxxx xx xxxxxx xxxxxxx xxxxxxx xx Xxxxxx$Xxxxxx$ xxx XxxxxXxxxxx xxxxx$xxxx xx xxx xxxxx xx x xxxxxxxxxx xxxx xx xxx xxxxxx xx x xxxxxxx$ xxxx xx $XxxxxXxxxxx $Xxx$Xxxxxxx$$xx xxxxxxx xx x xxxxxx xxxxxx.
Xxxxxxx XxxxxXxxxxx xxxxxx xxxxxx xxxxxxxxxx xxxxxxxxxx xxxx xx xxxxx xx xxxxxxxxxx xx xxxxxxx$ xx xx xxxxxxxxxxx xxxx xx xxx xxx Xxxxxx$Xxxxxx xx xxxxxx x xxxxxxxxxx xx xxxxxxx xxx xxxxx xxxxxxx xxxx xxxx xxxxxxxx xxxxxx xx xxxxxxx xxxxxxxxxx$ xxx xxx Xxxxxx$Xxxxxx xx xxx xxxxxxxx$ xx xxxxx xx xxx xxxxxxxx xx xxxx xxxxx.

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

### -Last
Xxxxxxxxx xxx xxxxxx xx xxxxxxx xx xxxxxx xxxx xxx xxx xx xx xxxxx xx xxxxx xxxxxxx.

```yaml
Type: Int32
Parameter Sets: DefaultParameter
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Property
Xxxxxxxxx xxx xxxxxxxxxx xx xxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

Xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx xxx xx x xxx xxxxxxxxxx xxxxxxxx.
Xx xxxxxx x xxxxxxxxxx$ xxxxxxxx$ xxx x xxxx xxxxx.
Xxxxx xxxx xxx$

$$ Xxxx $xx Xxxxx$ $$xxxxxx$$$$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxx xxxxx\>

```yaml
Type: Object[]
Parameter Sets: DefaultParameter, SkipLastParameter
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SkipLast
Xxx xxxxx xx xxx xxxxxxxx xxxxxxxxx xxx xx x xxxxxxxxxx xxxxxxxx$ xxxxx xx x xxxx xxxxx xxxx xxxxxxxxx x xxxx xxx xxxxxxxxxx x xxxxx xxx xxx xxxxxxxx xxxxxxx.
Xxxxx xxxx xxx$

$$ Xxxx xx Xxxxx $$xxxxxx$$$$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxxxxxxx\>

Xxx xxxx xxxxxxxxxxx$ xxx xxx xxxxxxxx.

```yaml
Type: Int32
Parameter Sets: SkipLastParameter
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Unique
Xxxxxxxxx xxxx xx x xxxxxx xx xxx xxxxx xxxxxxx xxx xxxxxxxxx xxxxxxxxxx xxx xxxxxx$ xxxx x xxxxxx xxxxxx xx xxx xxxxxx xxxx xx xxxxxxxx.

Xxxx xxxxxxxxx xx xxxx$xxxxxxxxx.
Xx x xxxxxx$ xxxxxxx xxxx xxxxxx xxxx xx xxxxxxxxx xxxxxx xxx xxxxxxxxxx xx xx xxxxxx.

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

### -Wait
Xxxxx xxx xxxxxxxxxxxx.
Xxxxxxx XxxxxXxxxx xxxx xxxxxxxx xx xxx xxxxx xxxx xxxx xxxxxx xx xxx xxxxxxx xxxxxxxx xxx xxxx xxxx xxxxxxxx xxx xxxxxxx.
Xx xxxxxxx$ xx xxx xxxxxxx x Xxxxxx$Xxxxxx xxxxxxx xxxx xxx Xxxxx xx Xxxxx xxxxxxxxxx xx x xxxxxxx xxxxxxxx$ Xxxxxxx XxxxxXxxxx xxxxx xxx xxxxxxx xxxx xxxxxxxxx xxx xxxxxxx xx xxxx xx xxx xxxxxxxx xxxxxx xx xxxxxxx xx xxxxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: SwitchParameter
Parameter Sets: DefaultParameter, IndexParameter
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -First
$$Xxxx Xxxxx Xxxxxxxxxxx$$

```yaml
Type: Int32
Parameter Sets: DefaultParameter
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Skip
$$Xxxx Xxxx Xxxxxxxxxxx$$

```yaml
Type: Int32
Parameter Sets: DefaultParameter
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.Management.Automation.PSObject
Xxx xxx xxxx xxx xxxxxx xx Xxxxxx$Xxxxxx.

## XXXXXXX

### System.Management.Automation.PSObject

## XXXXX
Xxx xxx xxxx xxxxx xx xxx Xxxxxx$Xxxxxx xxxxxx xx xxx xxxxx$xx xxxxx$ $xxxxxx$.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx.

Xxx xxxxxxxxxxxx xxxxxxx xx Xxxxxx$Xxxxxx xx xxxxxxxxx xxxx xxx xxxxxxxx xxxx xxxxx xxxxxxx xx xxx xxxxxxxx xx xxxx xxx xxxxxxxxx.
Xx xxx xx xxxxxx xx xxxxxxxx xxxx xxxxxx xxxxxxxxx xxxxxxx xxx xxxxx xxxx xx x xxxxxxxxxx.
Xxxxxxx xxxxxxx xxxxxxxxxxx xx x xxxxxx xxxxxx xxxx xxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx $Xxxxx Xxxxxx Xxxxxxx xx xxx Xxxxxxxx$ xx $Xxxxxxxx Xxxxxxxxxx Xxxxxxxxxxx Xxxxxxxxxx$ xx xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXx$000000

## XXXXXXX XXXXX

[Group-Object]()

[Sort-Object]()

[Where-Object]()

