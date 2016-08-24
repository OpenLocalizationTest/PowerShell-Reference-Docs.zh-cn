---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294031
schema: 2.0.0
---

# Xxxxx$Xxxxxxxx
## XXXXXXXX
Xxxxxxxx x xxxxxxxx xxx xxxxxx x Xxxxxxx XxxxxXxxxx xxxxxxx xxxxxx.

## XXXXXX

```
Write-Progress [-Activity] <String> [[-Status] <String>] [[-Id] <Int32>] [-PercentComplete <Int32>]
 [-SecondsRemaining <Int32>] [-CurrentOperation <String>] [-ParentId <Int32>] [-Completed] [-SourceId <Int32>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxx$Xxxxxxxx xxxxxx xxxxxxxx x xxxxxxxx xxx xx x Xxxxxxx XxxxxXxxxx xxxxxxx xxxxxx xxxx xxxxxxx xxx xxxxxx xx x xxxxxxx xxxxxxx xx xxxxxx.
Xxx xxx xxxxxx xxx xxxxxxxxxx xxxx xxx xxx xxxxxxxx xxx xxx xxxx xxxx xxxxxxx xxxxx xxx xxxxx xxx xxxxxxxx xxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>for ($i = 1; $i -le 100; $i++ )
{write-progress -activity "Search in Progress" -status "$i% Complete:" -percentcomplete $i;}
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxx xx x Xxx xxxx xxxx xxxxxx xxxx 0 xx 000.
Xxx Xxxxx$Xxxxxxxx xxxxxxx xxxxxxxx x xxxxxx xxx xxxxxxx $$xxxxxxxx$$$ x xxxxxx xxxx$ xxx xxx xxxxxxxx $x $xxx xxxxxxx xx xxx Xxx xxxx$$ xxxxx xxxxxxxxx xxx xxxxxxxx xxxxxxxxxxxx xx xxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>for($i = 1; $i -lt 101; $i++ )
{write-progress -activity Updating -status 'Progress->' -percentcomplete $i -currentOperation OuterLoop; `
for($j = 1; $j -lt 101; $j++ )
{write-progress -id  1 -activity Updating -status 'Progress' -percentcomplete $j -currentOperation InnerLoop} }

Updating
Progress ->
[ooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooo]
OutsideLoop
Updating
Progress
[oooooooooooooooooo                                                   ]
InnerLoop
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxx xx xxx xxxxxx Xxx xxxxx$ xxxx xx xxxxx xx xxxxxxxxxxx xx x xxxxxxxx xxx.

Xxx Xxxxx$Xxxxxxxx xxxxxxx xxx xxx xxxxxx xxxxxxxx xxx xxxxxxxx xxx Xx xxxxxxxxx xxxx xxxxxxxxxxxxx xx xxxx xxx xxxxx xxxxxxxx xxx.
Xxxxxxx xxx Xx xxxxxxxxx$ xxx xxxxxxxx xxxx xxxxx xx xxxxxxxxxxxx xx xxxx xxxxx xxxxxxx xx xxxxx xxxxxxxxx xxx xxxxx xxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$events = get-eventlog -logname system
PS C:\>$events | foreach-object -begin {clear-host;$i=0;$out=""} `
-process {if($_.message -like "*bios*") {$out=$out + $_.Message}; $i = $i+1;
write-progress -activity "Searching Events" -status "Progress:" -percentcomplete ($i/$events.count*100)} `
-end {$out}
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxx xx x xxxxxxx xx xxxx xxx xxxxxx $xxxx$ xx xxx Xxxxxx xxxxx xxx.

Xx xxx xxxxx xxxx xx xxx xxxxxxx$ xxx Xxx$XxxxxXxx xxxxxx xxxx xxx xxxxxx xx xxx Xxxxxx xxx xxx xxxxxx xxxx xx xxx $xxxxxx xxxxxxxx.

Xx xxx xxxxxx xxxx$ xxx xxxxxx xxx xxxxx xx xxx XxxXxxx$Xxxxxx xxxxxx.
Xxxxxx xxxxxxxxxx xxxxxx$ xxx Xxxxx$Xxxx xxxxxx xx xxxx xx xxxxx xxx xxxxxx$ xxx $x xxxxxxx xxxxxxxx xx xxx xx xxxx$ xxx xxx $xxx xxxxxx xxxxxxxx xx xxx xx xxx xxxxx xxxxxx.

Xx xxx xxxxx xxxx$ xxxxx xx xxx Xxxxxxx xxxxxx xxxxx xx xxx XxxXxxx$Xxxxxx xxxxxx$ xxx xxxxxx xxxxxxxx xxx xxxxxxx xxxxxxxx xx xxxx xxxxxxxx xxxxxx xxx $xxxx$.
Xx xxx xxxxxx xx xxxxx$ xxx xxxxxxx xx xxxxx xx $xxx.
Xxxx$ xxx $x xxxxxxx xxxxxxxx xx xxxxxxxxxxx xx xxxxxx xxxx xxxxxxx xxxxx xxx xxxx xxxxxxxx.

Xxx xxxxxx xxxx xxxx xxx Xxxxx$Xxxxxxxx xxxxxx xxxx xxxxxx xxx xxx Xxxxxxxx xxx Xxxxxx xxxx xxxxxx xxxx xxxxxx xxx xxxxx xxx xxxxxx xxxxx xx xxx xxxxxxxx xxx xxxxxxx$ xxxxxxxxxxxx.
Xxx XxxxxxxXxxxxxxx xxxxxxxxx xxxxx xx xxxxxxxxxx xx xxxxxxxx xxx xxxxxx xx xxxxxx xxxx xxxx xxxx xxxxxxxxx $$x$ xx xxx xxxxx xxxxxx xx xxxxxx xxxxxxxxx $$xxxxxx.xxxxx$ xxx xxxx xxxxxxxxxxx xxxx xxxxxx xx 000.

Xx xxx xxxx xxxx$ xxx Xxx xxxxxxxxx xx xxx XxxXxxx$Xxxxxx xxxxxx xx xxxx xx xxxxxxx xxx xxxxxxxx xxxx xxx xxxxxx xx xxx $xxx xxxxxxxx.

## XXXXXXXXXX

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxx xxxx xx xxxx xx xxx xxxxxxx xxxxx xxx xxxxxx xxx.
Xxxx xxxx xxxxxxxxx xxx xxxxxxxx xxxxx xxxxxxxx xx xxxxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxxx
Xxxxxxxxx xxxxxxx xxx xxxxxxxx xxx xx xxxxxxx.
Xx xxxx xxxxxxxxx xx xxxxxxx$ Xxxxx$Xxxxxxxx xxxxxxxx xxxxxxxx xxxxxxxxxxx.

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

### $XxxxxxxXxxxxxxxx
Xxxxxxxxx xxx xxxx xx xxxx xxxxx xxx xxxxxxxx xxx.
Xxxx xxxx xxxxxxxxx xxx xxxxxxxxx xxxx xx xxxxxxxxx xxxxxx xxxxx.

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

### $Xx
Xxxxxxxxx xx XX xxxx xxxxxxxxxxxxx xxxx xxxxxxxx xxx xxxx xxx xxxxxx.
Xxx xxxx xxxxxxxxx xxxx xxx xxx xxxxxxxx xxxx xxxx xxx xxxxxxxx xxx xx x xxxxxx xxxxxxx.
Xx xxx xxxxxxxx xxxx xx xxx xxxx xxxxxxxxx XXx$ xxxx xxx xxxxxxxxxxxx xxxxxxx xx xxxxx xxxxxxxxx xx x xxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
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

### $XxxxxxXx
Xxxxxxxxxx xxx xxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxxx.
Xxx xxx xxxxx $0 xx xxx xxxxxxx xxxxxxxx xxx xx xxxxxx xxxxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxxxxxx
Xxxxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxxx xxxx xx xxxxxxxxx.
Xxx xxx xxxxx $0 xx xxx xxxxxxxxxx xxxxxxxx xx xxxxxxx xx xxx xxxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxxxxxxx
Xxxxxxxxx xxx xxxxxxxxx xxxxxx xx xxxxxxx xxxxxxxxx xxxxx xxx xxxxxxxx xx xxxxxxxxx.
Xxx xxx xxxxx $0 xx xxx xxxxxx xx xxxxxxx xxxxxxxxx xx xxxxxxx xx xxx xxxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxXx
Xxxxxxxxxx xxx xxxxxx xx xxx xxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxx
Xxxxxxxxx xxx xxxxxx xxxx xx xxxx xx xxx xxxxxxx xxxxx xxx xxxxxx xxx.
Xxxx xxxx xxxxxxxxx xxxxxxx xxxxx xx xxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxx
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### Xxxx
Xxxxx$Xxxxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xx xxx xxxxxxxx xxx xxxx xxx xxxxxx$ xxxxx xxx xxxxx xx xxx $XxxxxxxxXxxxxxxxxx xxxxxxxx.
Xx xxx xxxxx xx xxx xx XxxxxxxxXxxxxxxx$ xxx xxxxxxxx xxx xx xxx xxxxxxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx Xxxxxxx XxxxxXxxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxxx$Xxxxxxxxx.

Xxx xxxxxxxxxx xx xxx xxxxxx xxxxxxxxxx xx xxx xxxxxxxxxx xx xxx XxxxxxxxXxxxxx xxxxx $Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XxxxxxxxXxxxxx$.
Xxx xxxx xxxxxxxxxxx$ xxx xxx XxxxxxxxXxxxxx xxxxx xx xxx Xxxxxxx XxxxxXxxxx Xxxxxxxx Xxxxxxxxxxx Xxx $XXX$.

## XXXXXXX XXXXX

[Xxxxx$Xxxxx]()

[Xxxxx$Xxxxx]()

[Xxxxx$Xxxx]()

[Xxxxx$Xxxxxx]()

[Xxxxx$Xxxxxxx]()

[Xxxxx$Xxxxxxx]()

