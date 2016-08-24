---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293950
schema: 2.0.0
---

# XxxxxxxXx$Xxxx
## XXXXXXXX
Xxxxxxxx Xxxxxxxxx .XXX Xxxxxxxxx xxxxxxx xxxx XXXX xxxx xxx xx xxxxxxxxx xx x Xxx xxxxxxx.

## XXXXXX

### Xxxx $Xxxxxxx$
```
ConvertTo-Html [-InputObject <PSObject>] [[-Property] <Object[]>] [[-Body] <String[]>] [[-Head] <String[]>]
 [[-Title] <String>] [-As <String>] [-CssUri <Uri>] [-PostContent <String[]>] [-PreContent <String[]>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### Xxxxxxxx
```
ConvertTo-Html [-InputObject <PSObject>] [[-Property] <Object[]>] [-As <String>] [-Fragment]
 [-PostContent <String[]>] [-PreContent <String[]>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx XxxxxxxXx$Xxxx xxxxxx xxxxxxxx .XXX Xxxxxxxxx xxxxxxx xxxx XXXX xxxx xxx xx xxxxxxxxx xx x Xxx xxxxxxx.
Xxx xxx xxx xxxx xxxxxx xx xxxxxxx xxx xxxxxx xx x xxxxxxx xx x Xxx xxxx.

Xxx xxx xxx xxx xxxxxxxxxx xx XxxxxxxXx$Xxxx xx xxxxxx xxxxxx xxxxxxxxxx$ xx xxxxxxx x xxxxx xx xxxx xxxxxx$ xx xxxxxxx xxx XXXX xxxx xxxxx$ xx xxx xxxx xxxxxx xxx xxxxx xxx xxxxxx$ xxx xx xxxxxx xxxx xxx xxxxx xx xxxx xxxxxxxx$ xxxxxxx xx x xxxxxx XXX xxxx.

Xxxx xxx xxxxxx xxxxxxxx xxxxxxx xx XxxxxxxXx$Xxxx$ Xxxxxxx XxxxxXxxxx xxxxxxx xxx xxxxx $xx xxxx$ xxxxx xx xxx xxxxxxxxxx xx xxx xxxxx xxxxxx xxxx xxx xxxxxx.
Xx xxx xxxxxxxxx xxxxxxx xx xxx xxxx xxx xx xxx xxxxxxxxx xxxxxxxxxx$ xxx xxxxxxxx xxxxx xx xxxx xxxxxx xx xx xxxxx xxxx.
Xx xxx xxxxxxxxx xxxxxxx xxxx xxxxxxxxxx xxxxxxxxxx$ xxxxx xxxxxxxx xxxxxx xxx xxx xxxxxxxx xx xxx xxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>convertto-html -inputobject (get-date)
```

Xxxx xxxxxxx xxxxxxx xx XXXX xxxx xxxx xxxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxx xxxx.
Xx xxxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxx xxx xxxxxxx xx x Xxx$Xxxx xxxxxxx xx xxx XxxxxxxXx$Xxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-alias | convertto-html > aliases.htm
PS C:\>invoke-item aliases.htm
```

Xxxx xxxxxxx xxxxxxx xx XXXX xxxx xxxx xxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xx xxx xxxxxxx xxxxxxx.

Xxx xxxxxxx xxxx xxx Xxx$Xxxxx xxxxxx xx xxx xxx xxxxxxx.
Xx xxxx xxx xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xx xxx XxxxxxxXx$Xxxx xxxxxx$ xxxxx xxxxxxx xxx XXXX xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-eventlog -logname "Windows PowerShell" | convertto-html > pslog.htm
```

Xxxx xxxxxxx xxxxxxx xx XXXX xxxx xxxxxx xxxxx.xxx xxxx xxxxxxxx xxx xxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxx xxx xx xxx xxxxx xxxxxxxx.

Xx xxxx xxx Xxx$XxxxxXxx xxxxxx xx xxx xxx xxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxx xxx xxxx xxxx xxx xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xx xxx XxxxxxxXx$Xxxx xxxxxx.

Xxx xxxxxxx xxxx xxxx xxx xxxxxxxxxxx xxxxxxxx $$$$ xx xxxx xxx XXXX xxxx xx xxx xxxxx.xxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | convertto-html -property Name, Path, Company -title "Process Information" > proc.htm; ii proc.htm
```

Xxxxx xxxxxxxx xxxxxx xxx xxxx xx XXXX xxxx xxxx xxxxx xxx xxxx$ xxxx$ xxx xxxxxxx xx xxx xxxxxxxxx xx xxx xxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxxxxxx xxxx xxxxxxxxx xxx xxxxxxxxx xxxxxxx xx xxx xxxxxxxx.
Xxx xxxxxxx xxxx xxx xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xxxxxxx xx xxx XxxxxxxXx$Xxxx xxxxxx.

Xxx xxxxxxx xxxx xxx Xxxxxxxx xxxxxxxxx xx xxxxxx xxxxx xxxxxxxxxx xx xxx xxxxxxx xxxxxxx xx xx xxxxxxxx xx xxx xxxxx.
Xxx xxxxxxx xxxx xxx Xxxxx xxxxxxxxx xx xxxxxxx x xxxxx xxx xxx XXXX xxxx.
Xxx xxxxxxx xxxx xxxx xxx xxxxxxxxxxx xxxxxxxx $$$$ xx xxxx xxx xxxxxxxxx XXXX xx x xxxx xxxxx Xxxx.xxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx$Xxxx xxxxxx $xxxxx $ xx$ xx xxxx xxx Xxxx.xxx xx xxx xxxxxxx xxxxxxx.
Xxx xxx xxxxxxxx xxx xxxxxxxxx xx x xxxxxxxxx $$$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-service | convertto-html -CssUri "test.css"
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"       "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html>
<head>
<title>HTML TABLE</title>
<link rel="stylesheet" type="text/css" href="test.css" />
...
```

Xxxx xxxxxxx xxxxxxx xx XXXX xxxx xx xxx xxxxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx XxxXxx xxxxxxxxx xx xxxxxxx x xxxxxxxxx xxxxx xxxxx xxx xxx XXXX xxxx.

Xxx XxxXxx xxxxxxxxx xxxx xx xxxxxxxxxx $$$xxxx xxx$$xxxxxxxxxx$ xxxx$$xxxx$xxx$ xxx xx xxx xxxxxxxxx XXXX.
Xxx XXXX xxxxxxxxx xx xxx xxx xxxxxxxx xxx xxxx xx xxx xxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-service | convertto-html -as LIST > services.htm
```

Xxxx xxxxxxx xxxxxxx xx XXXX xxxx xx xxx xxxxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx Xx xxxxxxxxx xx xxxxxxx x xxxx xxxxxx.
Xxx xxxxxxxxxxx xxxxxxxx $$$$ xxxxx xxx xxxxxxxxx XXXX xx xxx Xxxxxxxx.xxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-date | cth -fragment
<table>
<colgroup>...</colgroup>
<tr><th>DisplayHint</th><th>DateTime</th><th>Date</th><th>Day</th><th>DayOfWeek</th><th>DayOfYear</th><th>Hour</th>
<th>Kind</th><th>Millisecond</th><th>Minute</th><th>Month</th><th>Second</th><th>Ticks</th><th>TimeOfDay</th><th>Year</th></tr>
<tr><td>DateTime</td><td>Monday, May 05, 2008 10:40:04 AM</td><td>5/5/2008 12:00:00 AM</td><td>5</td><td>Monday</td>
<td>126</td><td>10</td><td>Local</td><td>123</td><td>40</td><td>5</td><td>4</td><td>633455808041237213</td><td>10:40:04.12
37213</td><td>2008</td></tr>
</table>
```

Xxxx xxxxxxx xxxx XxxxxxxXx$Xxxx xx xxxxxxxx xx XXXX xxxxx xx xxx xxxxxxx xxxx.
Xxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx xxx xxxxxxx xxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xx xxx XxxxxxxXx$Xxxx xxxxxx $xxxxxxx xx $xxx$$.

Xxx XxxxxxxXx$Xxxx xxxxxxx xxxxxxxx xxx Xxxxxxxx xxxxxxxxx$ xxxxx xxxxxx xxx xxxxxx xx xx XXXX xxxxx.
Xx x xxxxxx$ xxx xxxxx xxxxxxxx xx xx XXXX xxxx$ xxxx xx xxx $$XXXX$$ xxx $$XXXX$$ xxxx$ xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-eventlog -log "Windows PowerShell" | convertto-html -property id, level, task
```

Xxxx xxxxxxx xxxx xxx Xxx$XxxxxXxx xxxxxx xx xxx xxxxxx xxxx xxx $Xxxxxxx XxxxxXxxxx$ xxxxx xxx.

Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xx xxx XxxxxxxXx$Xxxx xxxxxx$ xxxxx xxxxxxxx xxx xxxxxx xx XXXX xxxxxx.

Xxx XxxxxxxXx$Xxxx xxxxxxx xxxx xxx Xxxxxxxx xxxxxxxxx xx xxxxxx xxxx xxx XX$ Xxxxx$ xxx Xxxx xxxxxxxxxx xx xxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-service A* | ConvertTo-Html -title "Windows Services: Server01" -body (get-date) -pre 
"<P>Generated by Corporate IT</P>" -post "For details, contact Corporate IT." > services.htm; ii services.htm
```

Xxxx xxxxxxx xxxxxxx xxx xxxxx x Xxx xxxx xxxx xxxxxxxx xxx xxxxxxxx xx xxx xxxxxxxx xxxx xxxxx xxxx $X$.
Xx xxxx xxx Xxxxx$ Xxxx$ XxxXxxxxxx$ xxx XxxxXxxxxxx xxxxxxxxxx xx XxxxxxxXx$Xxxx xx xxxxxxxxx xxx xxxxxx.

Xxx xxxxx xxxx xx xxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxxx xx xxx xxxxxxxx xxxx xxxxx xxxx $X$.
Xxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xx xxx XxxxxxxXx$Xxxx xxxxxx.
Xxx xxxxxxx xxxx x xxxxxxxxxxx xxxxxxxx $$$$ xx xxxx xxx xxxxxx xx xxx Xxxxxxxx.xxx xxxx.

X xxxxxxxxx $$$ xxxx xxx xxxxx xxxxxxx xxx xxxxxx x xxxxxx xxxxxxx$ xxxxx xxxx xxx Xxxxxx$Xxxx xxxxxx $xxxxx $ $xx$$ xx xxxx xxx Xxxxxxxx.xxx xxxx xx xxx xxxxxxx xxxxxxx.

## XXXXXXXXXX

### $Xx
Xxxxxxxxxx xxxxxxx xxx xxxxxx xx xxxxxxxxx xx x xxxxx xx x xxxx.
Xxxxx xxxxxx xxx XXXXX xxx XXXX.
Xxx xxxxxxx xxxxx xx XXXXX.

Xxx XXXXX xxxxx xxxxxxxxx xx XXXX xxxxx xxxx xxxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxxx xxxxxx.
Xxx xxxxxx xxx xxxxxxxx xxx xxxxxxxx xxxxx.
Xxxx xxxxx xxx xxxxxxxxxx xx xxxxxx xxx xxxxxxxx xxx xxxxxx$x xxxxxx xxx xxxx xxxxxxxx.

Xxx XXXX xxxxx xxxxxxxxx x xxx$xxxxxx XXXX xxxxx xxx xxxx xxxxxx xxxx xxxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxx xxxxxx.
Xxx xxxxx xxxxxx xxxxxxxx xxx xxxxxxxx xxxx$ xxx xxxxxx xxxxxx xxxxxxxx xxx xxxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: Table, List

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxx xxx xxxxxxx $$XXXX$$ xxx.
Xx xxxxxxx$ xxxxx xx xx xxxx xx xxxx xxxxxxxx.

```yaml
Type: String[]
Parameter Sets: Page
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxx
Xxxxxxxxx xxx Xxxxxxx Xxxxxxxx Xxxxxxxxxx $XXX$ xx xxx xxxxxxxxx xxxxx xxxxx $XXX$ xxxx xx xxxxxxx xx xxx XXXX xxxx. Xxx XXX xx xxxxxxxx xx x xxxxx xxxxx xxxx xx xxx xxxxxx.

```yaml
Type: Uri
Parameter Sets: Page
Aliases: cu, uri

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxxxxxxx xxxx xx XXXX xxxxx.
Xxx XXXX$ XXXX$ XXXXX$ xxx XXXX xxxx xxx xxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: Fragment
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx xxx xxxxxxx xx xxx $$XXXX$$ xxx.
Xxx xxxxxxx xx $$$xxxxx$$XXXX XXXXX$$$xxxxx$$$. Xx xxx xxx xxx Xxxx xxxxxxxxx$ xxx Xxxxx xxxxxxxxx xx xxxxxxx.

```yaml
Type: String[]
Parameter Sets: Page
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxxxXxxxxx
Xxx XXXXX xxxxx xxxxxxxxx xx XXXX xxxxx xxxx xxxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxxx xxxxxx.
Xxx xxxxxx xxx xxxxxxxx xxx xxxxxxxx xxxxx.
Xxxx xxxxx xxx xxxxxxxxxx xx xxxxxx xxx xxxxxxxx xxx xxxxxx$x xxxxxx xxx xxxx xxxxxxxx.

Xxx XXXX xxxxx xxxxxxxxx x xxx$xxxxxx XXXX xxxxx xxx xxxx xxxxxx xxxx xxxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxx xxxxxx.
Xxx xxxxx xxxxxx xxxxxxxx xxx xxxxxxxx xxxx$ xxx xxxxxx xxxxxx xxxxxxxx xxx xxxxxxxx xxxxx.

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
Xxx XXXXX xxxxx xxxxxxxxx xx XXXX xxxxx xxxx xxxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxxx xxxxxx.
Xxx xxxxxx xxx xxxxxxxx xxx xxxxxxxx xxxxx.
Xxxx xxxxx xxx xxxxxxxxxx xx xxxxxx xxx xxxxxxxx xxx xxxxxx$x xxxxxx xxx xxxx xxxxxxxx.

Xxx XXXX xxxxx xxxxxxxxx x xxx$xxxxxx XXXX xxxxx xxx xxxx xxxxxx xxxx xxxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxx xxxxxx.
Xxx xxxxx xxxxxx xxxxxxxx xxx xxxxxxxx xxxx$ xxx xxxxxx xxxxxx xxxxxxxx xxx xxxxxxxx xxxxx.

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
Xxxxxxxxx xxx xxxxxxx xx xx xxxxxxxxxxx xx XXXX.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.

Xx xxx xxx xxxx xxxxxxxxx xx xxxxxx xxxxxxxx xxxxxxx$ xxxx xx xxx xx xxx xxxxxxxx xx x xxxxxxxx$ XxxxxxxXx$Xxxx xxxxxxx x xxxxx xxxx xxxxxxxx xxx xxxxxxxxxx xx x xxxxxxxxxx xx xx xx xxxxx xx xxxxxxx $Xxxxxx.Xxxxxx$$$$$.
Xx xxxxxx x xxxxx xx xxx xxxxxxxxxx xxxxxxx$ xxx xxx xxxxxxxx xxxxxxxx xx xxxx xxx xxxxxxx xx XxxxxxxXx$Xxxx.

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

### $XxxxXxxxxxx
Xxxxxxxxx xxxx xx xxx xxxxx xxx xxxxxxx $$$XXXXX$$ xxx.
Xx xxxxxxx$ xxxxx xx xx xxxx xx xxxx xxxxxxxx.

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

### $XxxXxxxxxx
Xxxxxxxxx xxxx xx xxx xxxxxx xxx xxxxxxx $$XXXXX$$ xxx.
Xx xxxxxxx$ xxxxx xx xx xxxx xx xxxx xxxxxxxx.

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

### $Xxxxxxxx
Xxxxxxxx xxx xxxxxxxxx xxxxxxxxxx xx xxx xxxxxxx xx xxx XXXX.
Xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx xxx xx x xxx xxxxxxxxxx xxxxxxxx.
Xx xxxxxx x xxxxxxxxxx xxxxxxxx$ xxx x xxxx xxxxx.
Xxxxx xxxx xxx$

$$ Xxxxx $$xxxxxx$$ $xxxxxx xxxx Xxxxxx$Xxxxxx xx Xxxxxx$Xxxxx$ xxx Xxxx xxx xx xxx xxxxxxxxx$ $$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxx xxxxx\>

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

### $Xxxxx
Xxxxxxxxx x xxxxx xxx xxx XXXX xxxx$ xxxx xx$ xxx xxxx xxxx xxxxxxx xxxxxxx xxx $$XXXXX$$ xxxx.

```yaml
Type: String
Parameter Sets: Page
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxx xxxx xxx .XXX xxxxxx xx XxxxxxxXx$Xxxx.

## XXXXXXX

### Xxxxxx.Xxxxxx
XxxxxxxXx$Xxxx xxxxxxx xxxxxx xx xxxxxxx xxxx xxxxxxxx xxxxx XXXX.

## XXXXX
Xx xxx xxxx xxxxxx$ xxxx xxx xx xxxx xxxxxxx xx xxx xxxxxx xx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxx.
Xxxx xxx xxxxx xxxxxxxx xx xxxxxxxx xxxxxxx$ xxx xxxxxx xx xxxxx xxx xxxxxxx xx xxxxx xxxxxxxxx.

$$  Xxxx xxx xxxx xxxxxxxx xxxxxxx xx x xxxxxx$ Xxxxxxx XxxxxXxxxx xxxxx xxx xxxxxxx xx xxx xxxxxx xxx xx x xxxx. Xx x xxxxxx$ XxxxxxxXx$Xxxx xxxxxxx x xxxxx xxxx xxxxxxxx xxx xxxxxxxxxx xxxxxxx. Xxx xxxxxxx$ xx xxx xxxx xxx xxxxxxxxx xx x xxxxxxxx xx XxxxxxxXx$Xxxx$ xxx xxxxxxxxx xxxxx xxxxxxxx xxx xx xxx xxxxxxxxx.
$$  Xxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxx xxxxxxxx xxxxxxx$ XxxxxxxXx$Xxxx xxxxxxxx xxxxx xxxxxxx xx x xxxxxxxxxx xx xx xx xxxxx. Xx x xxxxxx$ xx xxxxxxx x xxxxx xxxx xxxxxxxx xxx xxxxx xxx xxx xxxxxxxxxx$ xxx xxx xxxxx xx xxx xxxxx. Xxx xxxxxxx$ xx xxx xxx XxxxxXxxxxx xx xxxxxx xxx xxxxxxxxx xx x xxxxxxxx xx XxxxxxxXx$Xxxx$ xxx xxxxxxxxx xxxxx xxxxxxxx xx xxxxxx xxxxx $Xxxxxx.Xxxxxx$$$$$ xxx xxx xxxxxxxxxx.

Xx xxxxxx xxxx xxx XXXXX Xxxxxx XXX$xxx XXXXXXX xxx xx xxxxxxxx xxxxxxxxxxx$

$$$$XXXXXXX xxxx XXXXXX $$$$X0X$$XXX XXXXX 0.0 Xxxxxx$$XX$       $xxxx$$$xxx.x0.xxx$XX$xxxxx0$XXX$xxxxx0$xxxxxx.xxx$$$$

## XXXXXXX XXXXX

[XxxxxxxXx$Xxx]()

[XxxxxxxXx$Xxx]()

