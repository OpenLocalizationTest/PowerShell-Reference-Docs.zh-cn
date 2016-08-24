---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294008
schema: 2.0.0
---

# Xxxxxx$Xxxxxx
## XXXXXXXX
Xxxxx xxxx xx xxxxxxx xxx xxxxx.

## XXXXXX

### Xxxx $Xxxxxxx$
```
Select-String [-Pattern] <String[]> [-Path] <String[]> [-SimpleMatch] [-CaseSensitive] [-Quiet] [-List]
 [-Include <String[]>] [-Exclude <String[]>] [-NotMatch] [-AllMatches] [-Encoding <String>]
 [-Context <Int32[]>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### Xxxxxx
```
Select-String -InputObject <PSObject> [-Pattern] <String[]> [-SimpleMatch] [-CaseSensitive] [-Quiet] [-List]
 [-Include <String[]>] [-Exclude <String[]>] [-NotMatch] [-AllMatches] [-Encoding <String>]
 [-Context <Int32[]>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### XxxxxxxXxxx
```
Select-String [-Pattern] <String[]> -LiteralPath <String[]> [-SimpleMatch] [-CaseSensitive] [-Quiet] [-List]
 [-Include <String[]>] [-Exclude <String[]>] [-NotMatch] [-AllMatches] [-Encoding <String>]
 [-Context <Int32[]>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxxxxx xxxxxx xxxxxxxx xxx xxxx xxx xxxx xxxxxxxx xx xxxxx xxxxxxx xxx xxxxx.
Xxx xxx xxx xx xxxx Xxxx xx XXXX xxx Xxxxxxx xx Xxxxxxx.
Xxx xxx xxxx $Xxxxxx$Xxxxxx$ xx xxx xxxxx$ $xxx$.

Xxxxxx$Xxxxxx xx xxxxx xx xxxxx xx xxxx.
Xx xxxxxxx$ Xxxxxx$Xxxxxx xxxxx xxx xxxxx xxxxx xx xxxx xxxx xxx$ xxx xxxx xxxxx$ xx xxxxxxxx xxx xxxx xxxx$ xxxx xxxxxx$ xxx xxx xxxx xx xxx xxxx xxxxxxxxxx xxx xxxxx.
Xxxxxxx$ xxx xxx xxxxxx xx xx xxxxxx xxxxxxxx xxxxxxx xxx xxxx$ xxxxxxx xxxx xxxxxx xxx xxxxx xxx xxxxx$ xx xxxxxxx xxxx x Xxxxxxx xxxxx $xxxx xx xxxxx$ xxxx xxxxxxxxx xxxxxxx x xxxxx xx xxxxx.

Xxxxxx$Xxxxxx xxxx xxxxxxx xxxxxxxxxx xxxxxxxx$ xxx xx xxx xxxx xxxxxxx x xxxxxx xxxxx xxxx xxxxxxxx xxx xxxxx xxx xxx xxxx xxxx xxx xxxxxxx.

Xxxxxx$Xxxxxx xxx xxxxxxx xxx xx xxx xxxx xxxxxxx xx xxxx xxxxx xxx xxxxx xxxxx xx xxxx xxxxx xxxx.
Xx xxx xxxx xxxxxxx xxx xxxx xxxx xxxx xxx xxxxx xxx xxxxxxxxx xxxxxxx.
Xxx xxx xxxx xxxxxxx xxxx Xxxxxx$Xxxxxx xxxxxx xxxxxx x xxxxxxxxxx xxxxxxxxx xxxxxxxx$ xxxx xx xxxx xxx xxx xxxxxxxxx xxxxx xx Xxxxxxx xxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>"Hello","HELLO" | select-string -pattern "HELLO" -casesensitive
```

Xxxx xxxxxxx xxxxxxxx x xxxx$xxxxxxxxx xxxxx xx xxx xxxx xxxx xxx xxxxx xx xxx Xxxxxx$Xxxxxx xxxxxxx.

Xx x xxxxxx$ Xxxxxx$Xxxxxx xxxxx xxxx $XXXXX$$ xxxxxxx $Xxxxx$ xxxx xxx xxxxx.

Xxxxxxx xxxx xx xxx xxxxxx xxxxxxx xx xxxxxxx xx x xxxx$ xxxxxxx xxx XxxxXxxxxxxxx xxxxxxxxx$ Xxxxxx$Xxxxxx xxxxx xxxxxxxxx xxxx xx xxx xxxxxxx xx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>select-string -path *.xml -pattern "the the"
```

Xxxx xxxxxxx xxxxxxxx xxxxxxx xxx xxxxx xxxx xxx .xxx xxxx xxxx xxxxxxxxx xx xxx xxxxxxx xxxxxxxxx xxx xxxxxxxx xxx xxxxx xx xxxxx xxxxx xxxx xxxxxxx xxx xxxxxx $xxx xxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>select-string -path $pshome\en-US\*.txt -pattern "@"
```

Xxxx xxxxxxx xxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxxx Xxxx xxxxx $xxxxx$$.xxx$ xxx xxxxxxxxxxx xxxxx xxx xxx xx xxx xx xxxx $$$.

Xx xxxxxxxx xxx xxxx$ xxxx xxxxxxx xxxx xxx xxxxx xx xxx $xxxxxx xxxxxxxxx xxxxxxxx$ xxxxx xxxxxx xxx xxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxxxxx xxxxxxxxx.
Xx xxxx xxxxxxx$ xxx xxxxxxx xxxxxxxx xxx xx$XX xxxxxxxxxxxx$ xxxxx xxxxxxxx xxx Xxxxxxx $XX$ xxxxxxxx Xxxx xxxxx xxx Xxxxxxx XxxxxXxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>function search-help
{
   $pshelp = "$pshome\es\about_*.txt", "$pshome\en-US\*dll-help.xml"
   select-string -path $pshelp -pattern $args[0]
}
```

Xxxx xxxxxx xxxxxxxx xxxx xxx Xxxxxx$Xxxxxx xxxxxx xx xxxxxx xxx Xxxxxxx XxxxxXxxxx Xxxx xxxxx xxx x xxxxxxxxxx xxxxxx.
Xx xxxx xxxxxxx$ xxx xxxxxxxx xxxxxxxx xxx $xx$XX$ xxxxxxxxxxxx xxx Xxxxxxx$Xxxxxx Xxxxxx xxxxxxxx xxxxx.

Xx xxx xxx xxxxxxxx xx xxxx x xxxxxx$ xxxx xx $xxxxxxx$$ xxxx xxxxxx$xxxx xxxxxxx.

Xx xxx xxxx xxxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxx$ xxxxxx xxx xxxx xx xxxxx xx xxx Xxxxxxx XxxxxXxxxx Xxxx xxxxx xx xxxx xxxxxx$ xxx xxxx xxxxx xxx xxxxxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$events = get-eventlog -logname application -newest 100
PS C:\>$events | select-string -inputobject {$_.message} -pattern "failed"
```

Xxxx xxxxxxx xxxxxxxx xxx xxx xxxxxx $xxxxxx$ xx xxx 000 xxxxxx xxxxxx xx xxx Xxxxxxxxxxx xxx xx Xxxxx Xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XxxxxXxx xxxxxx xx xxx xxx 000 xxxx xxxxxx xxxxxx xxxx xxx Xxxxxxxxxxx xxxxx xxx.
Xxxx xx xxxxxx xxx xxxxxx xx xxx $xxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xx xxx $xxxxxx xxxxxxxx xx Xxxxxx$Xxxxxx.
Xx xxxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxxxxx xxx xxxxx xxxx xxx $xxxxxx xxxxxxxx.
Xxx xxxxx xx xxx XxxxxXxxxxx xxxxxxxxx xx xxx Xxxxxxx xxxxxxxx xx xxxx xxxxxx xx xx xxxxxxx xxxxxxx xxx xxxxxxxx.
Xxx xxxxxxx xxxxxx xx xxxxxxxxxxx xx xxx $$ xxxxxx.

Xx xxxx xxxxx xxxxxxx xx xxx xxxxxxxx$ Xxxxxx$Xxxxxx xxxxxxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xxx xxx $xxxxxx$ xxxxxx$ xxx xxxx xxxxxxxx xxx xxxxx xxxx xxxxxxx x xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem c:\windows\system32\*.txt -recurse | select-string -pattern "Microsoft" -casesensitive
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxx xx xxx xxxxxxxxxxxxxx xx X$$Xxxxxxx$Xxxxxx00 xxxx xxx .xxx xxxx xxxx xxxxxxxxx xxx xxxxxxxx xxx xxx xxxxxx $Xxxxxxxxx$.
Xxx XxxxXxxxxxxxx xxxxxxxxx xxxxxxxxx xxxx xxx $X$ xx $Xxxxxxxxx$ xxxx xx xxxxxxxxxxx xxx xxxx xxx xxxx xx xxx xxxxxxxxxx xxxx xx xxxxxxxxx xxx Xxxxxx$Xxxxxx xx xxxx x xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>select-string -path process.txt -pattern idle, svchost -notmatch
```

Xxxx xxxxxxx xxxxx xxxxx xx xxxx xx xxx Xxxxxxx.xxx xxxx xxxx xx xxx xxxxxxx xxx xxxxx $xxxx$ xx $xxxxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$f = select-string -path audit.log -pattern "logon failed" -context 2, 3
PS C:\>$f.count
PS C:\>($f)[0].context | format-list
```

Xxx xxxxx xxxxxxx xxxxxxxx xxx Xxxxx.Xxx xxxx xxx xxx xxxxxx $xxxxx xxxxxx.$ Xx xxxx xxx Xxxxxxx xxxxxxxxx xx xxxxxxx 0 xxxxx xxxxxx xxx xxxxx xxx 0 xxxxx xxxxx xxx xxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxx xxxxxxxx xx xxxxxx xxxxxx xx xxxxxxx xxx xxxxxx xx xxxxxxx xxxxx$ xx xxxx xxxx$ 0.

Xxx xxxxx xxxxxxx xxxxxxxx xxx xxxxx xxxxxx xx xxx Xxxxxxx xxxxxxxx xx xxx xxxxx XxxxxXxxx xxxxxx.
Xx xxxx xxxxx xxxxxxxx xx xxxxxxxx xxx xxxxx xxxxx $xxxxx 0 xx x xxxx$xxxxx xxxxx$$ xxx xx xxxx xxx X$Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.Xxxxxx$Xxxx xxxxxx xx xxxxxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx x xxxx.

Xxx xxxxxx xxxxxxxx xx xxx XxxxxXxxx xxxxxxx$ xxx xxx xxxx xxxxx xxxxxxxx.
Xxx xxxxxxx xxxxx xxx xxxxxx xx xxx Xxxxxxx xxxxxxxx xx xxx XxxxxXxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>
$a = get-childitem $pshome\en-us\about*.help.txt | select-string -pattern transcript
PS C:\>$b = get-childitem $pshome\en-us\about*.help.txt | select-string -pattern transcript -allmatches
PS C:\>$a
C:\Windows\system32\WindowsPowerShell\v1.0\en-us\about_Pssnapins.help.txt:39:       Start-Transcript and Stop-Transcript.
PS C:\>$b
C:\Windows\system32\WindowsPowerShell\v1.0\en-us\about_Pssnapins.help.txt:39:       Start-Transcript and Stop-Transcript.

PS C:\>> $a.matches
Groups   : {Transcript}
Success  : True
Captures : {Transcript}
Index    : 13
Length   : 10
Value    : Transcript
PS C:\>$b.matches
Groups   : {Transcript}
Success  : True
Captures : {Transcript}
Index    : 13
Length   : 10
Value    : Transcript
Groups   : {Transcript}
Success  : True
Captures : {Transcript}
Index    : 33
Length   : 10
Value    : Transcript
```

Xxxx xxxxxxx xxxxxxxxxxxx xxx xxxxxx xx xxx XxxXxxxxxx xxxxxxxxx xx Xxxxxx$Xxxxxx.
XxxXxxxxxx xxxxx xxx xxxxxxx xxxxxxx xx x xxxx$ xxxxxxx xx xxxx xxxxxxx xxx xxxxx xxxxx xx xxxx xxxx.

Xxx xxxxx xxxxxxx xx xxx xxxxxxx xxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxxx Xxxx xxxxx $$xxxxx$ Xxxx$ xxx xxxxxxxxx xx xxx xxxx $xxxxxxxxxx$.
Xxx xxxxxx xx xxx xxxxx xxxxxxx xx xxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xx xxxxxxxxx$ xxxxxx xxxx xx xxxx xxx XxxXxxxxxx xxxxxxxxx.
Xxx xxxxxx xx xxx xxxxxx xxxxxxx xx xxxxx xx xxx $x xxxxxxxx.

Xxxx xxx xxxxxxx xxx xxxxx xx xxx xxxxxxxxx$ xxx xxxxxxx xxxxxxx xx xxxxxxxxx$ xx xxxxx xx xxx xxxxxxx xxxxxx.

Xxxxxxx$ xxx xxxxx xxx xxxxx xxxxxxxx xxxxxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx xxxx xxxxxx.
Xxx Xxxxxxx xxxxxxxx xx xxx xxxxx xxxxxxx xxxxxxxx xxxx xxx xxxxx $xxxx xx$ xxx Xxxxxx.Xxxx.XxxxxxxXxxxxxxxxxx.Xxxxx xxxxxx$$ xxxxxxx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxx xxxxxxx xxxxxxxx xxxxxxx xxx xxxx xx xxx xxxxxxx xx xxx xxxx.

## XXXXXXXXXX

### $XxxXxxxxxx
Xxxxxxxx xxx xxxx xxxx xxx xxxxx xx xxxx xxxx xx xxxx.
Xxxxxxx xxxx xxxxxxxxx$ Xxxxxx$Xxxxxx xxxxx xxxx xxx xxxxx xxxxx xx xxxx xxxx xx xxxx.

Xxxx Xxxxxx$Xxxxxx xxxxx xxxx xxxx xxx xxxxx xx x xxxx xx xxxx$ xx xxxxx xxxxx xxxx xxx XxxxxXxxx xxxxxx xxx xxx xxxx$ xxx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxx xxxxxxxx xxx xx xxx xxxxxxx.

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

### $XxxxXxxxxxxxx
Xxxxx xxxxxxx xxxx$xxxxxxxxx.
Xx xxxxxxx$ xxxxxxx xxx xxx xxxx$xxxxxxxxx.

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

### $Xxxxxxx
Xxxxxxxx xxx xxxxxxxxx xxxxxx xx xxxxx xxxxxx xxx xxxxx xxx xxxx xxxx xxx xxxxx.
Xxxx xxxxxx xxx xx xxxx xxx xxxxx xx xxxxxxx.

Xx xxx xxxxx xxx xxxxxx xx xxx xxxxx xx xxxx xxxxxxxxx$ xxxx xxxxxx xxxxxxxxxx xxx xxxxxx xx xxxxx xxxxxxxx xxxxxx xxx xxxxx xxx xxxxx.
Xx xxx xxxxx xxx xxxxxxx xx xxx xxxxx$ xxx xxxxx xxxxxx xxxxxxxxxx xxx xxxxxx xx xxxxx xxxxxx xxx xxxxx xxx xxx xxxxxx xxxxxx xxxxxxxxxx xxx xxxxxx xx xxxxx xxxxx xxx xxxxx.

Xx xxx xxxxxxx xxxxxxx$ xxxxx xxxx x xxxxx xxx xxxxxxxxx xx x xxxxx xxxxx xxxxxxx $XXXXX 00$ xx xxx xxxxx xxxxxx xx xxx xxxxxxx.
Xxxxxxxx xxxxx xxx xxx xxxxxxx.

Xxxx xxxxxxxxx xxxx xxx xxxxxx xxx xxxxxx xx xxxxxxx xxxxxxxxx xx Xxxxxx$Xxxxxx.
Xxxxxx$Xxxxxx xxxxxxxxx xxx XxxxxXxxx $Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.XxxxxXxxx$ xxxxxx xxx xxxx xxxxx.
Xxx xxxxxxx xx xxxxxx xx xx xxxxx xx xxxxxxx xx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxx.

Xxxx xxx xxxx xxx xxxxxx xx x Xxxxxx$Xxxxxx xxxxxxx xx xxxxxxx Xxxxxx$Xxxxxx xxxxxxx$ xxx xxxxxxxxx xxxxxxx xxxxxxxx xxxx xxx xxxx xx xxx xxxxxxx xxxx $xxx xxxxx xx xxx Xxxx xxxxxxxx xx xxx XxxxxXxxx xxxxxx$$ xxx xxx xxxx xx xxx xxxxxxx xxxxx.
Xx x xxxxxx$ xxx Xxxxxxx xxxxxxxxx xx xxx xxxxx xx xxx xxxxxxxxx Xxxxxx$Xxxxxx xxxxxxx.

Xxxx xxx xxxxxxx xxxxxxxx x xxxxx$ xxx XxxxxXxxx xxxxxx xxx xxxx xxxxx xxxxxxxx xxx xx xxx xxxxxxx xxxxx$ xxx xxx xxxxxxxxxxx xxxxx xxxxxx xxxx xxxx xx xxx xxxxxxx.

```yaml
Type: Int32[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxxxxxx xxxxxxxx xxxx Xxxxxx$Xxxxxx xxxxxx xxxxxx xxxx xxxxxxxxx xxx xxxx.
Xxx xxxxxxx xx XXX0.

Xxxxx xxxxxx xxx $XXX0$$ $XXX0$$ $XXX00$$ $XXXXX$$ $Xxxxxxx$$ $XxxXxxxxxXxxxxxx$$ $Xxxxxxx$$ xxx $XXX$.
$Xxxxxxx$ xx xxx xxxxxxxx xx xxx xxxxxx$x xxxxxxx XXXX xxxx xxxx.
$XXX$ xx xxx xxxxxxx xxxxxxxx xxxxxxxxx xxxxxxxxxxxx xxxx xxxx xxxxxxxxxx xxx xxx xxxxxxxxx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: unicode, utf7, utf8, utf32, ascii, bigendianunicode, default, oem

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxx
Xxxxxxx xxx xxxxxxxxx xxxxx.
Xxx xxxxx xx xxxx xxxxxxxxx xxxxxxxxx xxx Xxxx xxxxxxxxx.
Xxxxx x xxxx xxxxxxx xx xxxxxxx$ xxxx xx $$.xxx$.
Xxxxxxxxx xxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxx
Xxxxxxx xxxx xxx xxxxxxxxx xxxxx.
Xxx xxxxx xx xxxx xxxxxxxxx xxxxxxxxx xxx Xxxx xxxxxxxxx.
Xxxxx x xxxx xxxxxxx xx xxxxxxx$ xxxx xx $$.xxx$.
Xxxxxxxxx xxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxxxXxxxxx
Xxxx Xxxxxx$Xxxxxx xxxxx xxxx xxxx xxx xxxxx xx x xxxx xx xxxx$ xx xxxxx xxxxx xxxx xxx XxxxxXxxx xxxxxx xxx xxx xxxx$ xxx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxx xxxxxxxx xxx xx xxx xxxxxxx.

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
Xxxx Xxxxxx$Xxxxxx xxxxx xxxx xxxx xxx xxxxx xx x xxxx xx xxxx$ xx xxxxx xxxxx xxxx xxx XxxxxXxxx xxxxxx xxx xxx xxxx$ xxx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxx xxxxxxxx xxx xx xxx xxxxxxx.

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

### $XxxxxXxxxxx
Xxxxxxxxx xxx xxxx xx xx xxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxx$ xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxx.

Xxxxx xxx XxxxxXxxxxx xxxxxxxxx xx xxx xxx xxxx xx xxxxxx xxxxxxx xx Xxxxxx$Xxxxxx.
Xxx xxxxxxxxxxx xxx xx xxxxxxx$

$$ Xxxx xxx xxxx xxxx xxxx xxx xxxxxx $x $xxxxxxxxxx$$ xx Xxxxxx$Xxxxxx$ Xxxxxx$Xxxxxx xxxxxxxx xxx xxx xxxxxxxxx xxxx xx xxxx xxxxxx xxx xxxxxxx xxxx xxxxxx xxxx xxxxxxxx xxx xxxxxx xxxx.
$$ Xxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxx x xxxxxxxxxx xx xxxxxxx$ Xxxxxx$Xxxxxx xxxxxx xxx xxxxxxxxxx xx x xxxxxx xxxxxxxx xxxxxx xxx xxxxxxx xxx xxxxxxx xx x xxxx xx xx xxxxx xxx xxxxxx xxxx xx xxx xxxxxx.

```yaml
Type: PSObject
Parameter Sets: Object
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxx xxxx xxx xxxxx xxxxx xx xxxx xxxxx xxxx.
Xx xxxxxxx$ Xxxxxx$Xxxxxx xxxxxxx x XxxxxXxxx xxxxxx xxx xxxx xxxxx xx xxxxx.

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

### $XxxXxxxx
Xxxxx xxxx xxxx xxxx xxx xxxxx xxx xxxxxxxxx xxxxxxx.

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

### $Xxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxx xx xx xxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.
Xxx xxxxxxx xxxxxxxx xx xxx xxxxx xxxxxxxxx.

Xxxxxxx xxxxx xx xxx xxxxxxxxx$ xxxx xx $xxx0.xxx$$ $$.xxx$$ xx $$.$$.
Xx xxx xxxxxxx xxxx x xxxxxxxxx$ xxx xxxxxxx xxxxx.

```yaml
Type: String[]
Parameter Sets: File
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxx
Xxxxxxxxx xxx xxxx xx xxxx.
Xxxx x xxxxxx xx xxxxxxx xxxxxxxxxx.
Xx xxx xxxx x xxxxxx$ xxx xxx XxxxxxXxxxx xxxxxxxxx.

Xx xxxxx xxxxx xxxxxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxxxxxxxx.

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

### $Xxxxx
Xxxxxxx x Xxxxxxx xxxxx $xxxx xx xxxxx$$ xxxxxxx xx x XxxxxXxxx xxxxxx.
Xxx xxxxx xx $xxxx$ xx xxx xxxxxxx xx xxxxx$ xxxxxxxxx$ xxx xxxxx xx $xxxxx$.

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

### $XxxxxxXxxxx
Xxxx x xxxxxx xxxxx xxxxxx xxxx x xxxxxxx xxxxxxxxxx xxxxx.
Xx x xxxxxx xxxxx$ Xxxxxx$Xxxxxx xxxxxxxx xxx xxxxx xxx xxx xxxx xx xxx Xxxxxxx xxxxxxxxx.
Xx xxxx xxx xxxxxxxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxxx xx x xxxxxxx xxxxxxxxxx xxxxxxxxx.

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

### $XxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxx xx xx xxxxxxxx.
Xxxxxx Xxxx$ xxx xxxxx xx xxx XxxxxxxXxxx xxxxxxxxx xx xxxx xxxxxxx xx xx xx xxxxx.
Xx xxxxxxxxxx xxx xxxxxxxxxxx xx xxxxxxxxx.
Xx xxx xxxx xxxxxxxx xxxxxx xxxxxxxxxx$ xxxxxxx xx xx xxxxxx xxxxxxxxx xxxxx.
Xxxxxx xxxxxxxxx xxxxx xxxx Xxxxxxx XxxxxXxxxx xxx xx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: LiteralFile
Aliases: PSPath

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxx xxxx xxx xxxxxx xxxx xxx x XxXxxxxx xxxxxx xx Xxxxxx$Xxxxxx.

## XXXXXXX

### Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.XxxxxXxxx xx Xxxxxx.Xxxxxxx
Xx xxxxxxx$ xxx xxxxxx xx x xxx xx XxxxxXxxx xxxxxxx$ xxx xxx xxxx xxxxx xxxxx.
Xx xxx xxx xxx Xxxxx xxxxxxxxx$ xxx xxxxxx xx x Xxxxxxx xxxxx xxxxxxxxxx xxxxxxx xxx xxxxxxx xxx xxxxx.

## XXXXX
Xxxxxx$Xxxxxx xx xxxx xxx Xxxx xxxxxxx xx XXXX xxx xxx XxxxXxx xxxxxxx xx Xxxxxxx.

Xxx $xxx$ xxxxx xxx xxx Xxxxxx$Xxxxxx xxxxxx xxx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

Xx xxx Xxxxxx$Xxxxxx$ xxxx xxx xxxx xxxx xxx xxxx xx xxxx xx xxx xxxxx xx xxx Xxxxxxx xxxxxxxxx.

Xx xxxxxxx xxx xxxx xx xx xxxxxxxx$ xx xxx xxxxxxxxx$

$$ Xxxx xxx xxxx xx x xxxxxx xxxxxx$ xxx xxxx xxxx xx xx Xxxxxx$Xxxxxx.
$$ Xxxxx x xxxx xxxxxx xx x xxxxxxxx$ xxx xxxx xxxxxxx xxx xxxxxxxx xx xxx xxxxx xx xxx XxxxxXxxxxx xxxxxxxxx.
$$ Xx xxx xxxx xx xxxxxx xx xxxxx$ xxx xxx Xxxx xxxxxxxxx xx xxxxxxx xxx xxxx xx xxx xxxxx.

Xx xxxxxxx$ Xxxxxx$Xxxxxx xxxxxxxxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxxx xx x xxxxxxx xxxxxxxxxx.
$Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxxxxxxxx.$ Xxxxxxx$ xxx xxx xxx xxx XxxxxxXxxxx xxxxxxxxx xx xxxxxxxx xxx xxxxxxx xxxxxxxxxx xxxxxxxx.
Xxx XxxxxxXxxxx xxxxxxxxx xxxxx xxxxxxxxx xx xxx xxxxx xx xxx Xxxxxxx xxxxxxxxx xx xxx xxxxx.

Xxx xxxxxxx xxxxxx xx Xxxxxx$Xxxxxx xx x XxxxxXxxx xxxxxx$ xxxxx xxxxxxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxx.
Xxx xxxxxxxxxxx xx xxx xxxxxx xx xxxxxx xxxx xxx xxx xxxxxxxxx xxx xxxx xx xxxxx$ xxxxxxx XxxxxXxxx xxxxxxx xxxx xxxxxxxxxx xxxx xx Xxxxxxxx xxx Xxxx.
Xxxx xxx xxxxx xx xxx xxxx xxx xxxx$ xxx xxxxx xx xxxxx xxxxxxxxxx xx $XxxxxXxxxxx$.

Xx xxx xx xxx xxxx xxx xxxxxxxxxxx xx xxx XxxxxXxxx xxxxxx$ xxx xxx Xxxxx xxxxxxxxx$ xxxxx xxxxxxx x Xxxxxxx xxxxx $xxxx xx xxxxx$ xx xxxxxxxx xxxxxxx xx xxxxx x xxxxx$ xxxxxxx xx x XxxxxXxxx xxxxxx.

Xxxx xxxxxxxx xxxxxxx$ Xxxxxx$Xxxxxx xxxx xxx xxxxxxx xxxxxxx xxxx xx xxx xxx xxx xxxxxx.
Xx xxxx xxx xxxxxxx xxxxxxx$ xxx xxx X$Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.Xxx$Xxxxxxx xxxxxx.

Xx xxxx xxx xxxxxxxxxx xx x XxxxxXxxx xxxxxx$ xxxx xxx xxxxxxxxx$

xxxxxx$xxxxxx $xxxx xxxx.xxx $xxxxxxx $xxxx$ $ xxx$xxxxxx $ xxxxxx$xxxx $xxxxxxxx $

## XXXXXXX XXXXX

[xxxxx$Xxxxxxxxxx$Xxxxxxxxx]()

[xxxxx$Xxxxxxx$Xxxxxxxxxxx]()

