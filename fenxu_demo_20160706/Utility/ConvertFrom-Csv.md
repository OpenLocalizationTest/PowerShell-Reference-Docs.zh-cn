---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293946
schema: 2.0.0
---

# XxxxxxxXxxx$Xxx
## XXXXXXXX
Xxxxxxxx xxxxxx xxxxxxxxxx xx xxxxx$xxxxxxxxx xxxxx $XXX$ xxxxxx xxxx XXX xxxxxxxx xx xxx xxxxxxxx xxxxxxx.

## XXXXXX

### Xxxxxxxxx $Xxxxxxx$
```
ConvertFrom-Csv [[-Delimiter] <Char>] [-InputObject] <PSObject[]> [-Header <String[]>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### XxxXxxxxxx
```
ConvertFrom-Csv [-UseCulture] [-InputObject] <PSObject[]> [-Header <String[]>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx XxxxxxxXxxx$XXX xxxxxx xxxxxxx xxxxxxx xxxx XXX xxxxxxxx$xxxxxx xxxxxxx xxxx xxx xxxxxxxxx xx xxx XxxxxxxXx$XXX xxxxxx.

Xxx xxx xxx xxx xxxxxxxxxx xx xxx XxxxxxxXxxx$XXX xxxxxx xx xxxxxxx xxx xxxxxx xxxxxx xxx$ xxxxx xxxxxxxxxx xxx xxxxxxxx xxxxx xx xxx xxxxxxxxx xxxxxxx$ xx xxxxxxx xxx xxxx xxxxxxxxx$ xx xx xxxxxx XxxxxxxXxxx$XXX xx xxx xxx xxxx xxxxxxxxx xxx xxx xxxxxxx xxxxxxx xx xxx xxxxxxxxx.

Xxx xxxxxxx xxxx XxxxxxxXxxx$XXX xxxxxxx xxx XXX xxxxxxxx xx xxx xxxxxxxx xxxxxxx.
Xxx xxxxxxxx xxxxxx xx xxx XXX xxxxxxx xxx xxxxxx xxxxxxxx xx xxx xxxxxxxx xxxxxx xx xxx xxxxxxxx xxxxxxx.
Xxx XXX xxxxxxxx xx xxx xxxxxxx xx xxx xxxx xxx xxxxxxx.

Xxx xxx xxxx xxx xxx Xxxxxx$XXX xxx Xxxxxx$XXX xxxxxxx xx xxxxxxx xxxxxxx xx XXX xxxxxxx xx x xxxx $xxx xxxx$.
Xxxxx xxxxxxx xxx xxx xxxx xx xxx XxxxxxxXx$XXX xxx XxxxxxxXxxx$XXX xxxxxxx$ xxxxxx xxxx xxxx xxxx xxx XXX xxxxxxx xx x xxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$p = get-process | convertto-csv
PS C:\>$p | convertfrom-csv
```

Xxxxx xxxxxxxx xxxxxxx xxx xxxxxxxxx xx xxx xxxxx xxxxxxxx xxxx XXX xxxxxx xxx xxxx xxxxxxx xxxx xx xxxxxx xxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxxxx xx xxx xxxxx xxxxxxxx.
X xxxxxxxx xxxxxxxx $$$ xxxxx xxxx xx xxx XxxxxxxXx$XXX xxxxxx$ xxxxx xxxxxxxx xxx xxxxxxx xxxxxx xx XXX xxxxxx.
Xxx XXX xxxxxxx xxx xxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx xx xxxx xxx XXX xxxxxxx xx xxx $x xxxxxxxx xx xxx XxxxxxxXxxx$XXX xxxxxx.
Xxx xxxxxx xxxxxxxx xxx XXX xxxxxxx xxxx XXX xxxxxxxx xx xxx xxxxxxxx xxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$date = get-date | convertto-csv -delimiter ";"
PS C:\>convertfrom-csv -inputobject $date -delimiter ";"
```

Xxxxx xxxxxxxx xxxxxxx x xxxx xxxxxx xx XXX xxxxxx xxx xxxx xx XXX xxxxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx xxx xxxxxxx xxxx xxx xxxx.
X xxxxxxxx xxxxxx $$$ xxxxx xxx xxxx xx xxx XxxxxxxXx$XXX xxxxxxx$ xxxxx xxxxxxxx xxx xxxx xxxxxx xx x xxxxxx xx XXX xxxxxxx.
Xxx xxxxxxx xxxx xxx Xxxxxxxxx xxxxxxxxx xx xxxxxxx x xxxxxxxxx xxxxxxxxx.
Xxx xxxxxxx xxx xxxxx xx xxx $xxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx XxxxxxxXxxx$XXX xxxxxx xx xxxxxxx xxx XXX xxxxxxx xx xxx $xxxx xxxxxxxx xxxx xx xxxxxx xxxxxx.
Xxx xxxxxxx xxxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxxx xxx XXX xxxxxxx xxx xxx Xxxxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxxxxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$j = start-job -scriptblock { get-process } | convertto-csv
PS C:\>$header = "MoreData","StatusMessage","Location","Command","State","Finished","InstanceId","SessionId","Name","ChildJobs","Output","Error","Progress","Verbose","Debug","Warning","StateChanged"
# Delete header from $j
PS C:\>$j = $j[0], $j[2..($j.count - 1)]
$j | convertfrom-csv -header $header

MoreData      : True
StatusMessage :
Location      : localhost
Command       : get-process
State         : Running
Finished      : System.Threading.ManualResetEvent
InstanceId    : 6fcb6578-7f42-4d93-9f23-9937f6aac1a2
SessionId     : 1
Name          : Job1
ChildJobs     : System.Collections.Generic.List`1[System.Management.Automation.Job]
Output        : System.Management.Automation.PSDataCollection`1[System.Management.Automation.PSObject]
Error         : System.Management.Automation.PSDataCollection`1[System.Management.Automation.ErrorRecord]
Progress      : System.Management.Automation.PSDataCollection`1[System.Management.Automation.ProgressRecord]
Verbose       : System.Management.Automation.PSDataCollection`1[System.String]
Debug         : System.Management.Automation.PSDataCollection`1[System.String]
Warning       : System.Management.Automation.PSDataCollection`1[System.String]
StateChanged  :
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx Xxxxxx xxxxxxxxx xx XxxxxxxXxxx$Xxx xx xxxxxx xxx xxxxx xx xxxxxxxxxx xx xxx xxxxxxxxx xxxxxxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxx$Xxx xxxxxx xx xxxxx x xxxxxxxxxx xxx xxxx xxxx x Xxx$Xxxxxxx xxxxxxx xx xxx xxxxx xxxxxxxx.
X xxxxxxxx xxxxxxxx $$$ xxxxx xxx xxxxxxxxx xxx xxxxxx xx xxx XxxxxxxXx$XXX xxxxxx$ xxxxx xxxxxxxx xxx xxx xxxxxx xx XXX xxxxxx.
Xx xxxxxxxxxx xxxxxxxx $$$ xxxxx xxx xxxxxxxxx XXX xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxx x xxxxxx xx xxx $xxxxxx xxxxxxxx.
Xxxxxx xxx xxxxxxx xxxxxx$ xxxx xxxxxx xxxx $XxxxXxxx$ xxxxxxx xx $XxxXxxxXxxx$ xxx $Xxxxx$ xxxxxxx xx $XxxXxxxxXxxx$.

Xxx xxxxx xxxxxxx xxxxxxx xxx xxxxxxxx xxxxxx $xxx xxxxxx xxxx$ xxxx xxx XXX xxxxxxx xxx xxxxxxx xx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx XxxxxxxXxxx$XXX xxxxxx xx xxxxxxx xxx XXX xxxxxxx xx x XXX xxxxxxx xx xxx xxx xxxxxx.
Xxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx xx xxxx xxx xxxxxxx xx $x xx XxxxxxxXxxx$XXX.
Xxx xxxxxxxxx xxxxxx xxx $XxxxXxxx$ xxx $Xxxxx$ xxxxxxxxxx$ xx xxxxxxxxx xx xxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>(get-culture).textinfo.listseparator
PS C:\>ConvertFrom-Csv -inputobject $services -UseCulture
```

Xxx xxxxxxx xxxx xxx XxxxxxxXxxx$XXX xxxxxx xx xxxxxxx XXX xxxxxxx xx xxxxxxx xxxxxxx xxxx xxx xxxx xxxxxxxxx xx xxx XxxxxxxXx$XXX xxxxxx.
Xxx xxxxxxx xxxx xxx XxxXxxxxxx xxxxxxxxx xx xxxxxx XxxxxxxXxxx$XXX xx xxx xxx xxxxxxxxx $xxxx xxxxxxxxx$ xx xxx xxxxxxx xxxxxxx.

Xxxx xxxxx xxx XxxXxxxxxx xxxxxxxxx$ xx xxxx xxxx xxx xxxx xxxxxxxxx xx xxx xxxxxxx xxxxxxx xxxxxxx xxx xxxxxxxxx xxxx xx xxx XXX xxxxxxx.
Xxxxxxxxx$ XxxxxxxXxxx$XXX xxxxxx xxxxxxxx xxxxxxx xxxx xxx XXX xxxxxxx.

Xx xxxx xxxxxxx$ x Xxx$Xxxxxxx xxxxxxx xxx xxxx xx xxxxxx xxx xxxx xxxxxxxxx$ xxxxxx xxx XxxxxxxXxxx$XXX xxxxxxx xxx xxxx.

## XXXXXXXXXX

### $Xxxxxxxxx
Xxxxxxxxx xxx xxxxxxxxx xxxx xxxxxxxxx xxx xxxxxxxx xxxxxx xx xxx XXX xxxxxxx.
Xxx xxxxxxx xx x xxxxx $$$.
Xxxxx x xxxxxxxxx$ xxxx xx x xxxxx $$$.
Xx xxxxxxx x xxxxxxxxx $$$$ xxxxxxx xx xx xxxxxxxxx xxxxx.

Xx xxx xxxxxxx x xxxxxxxxx xxxxx xxxx xxx xxxxxxxxx xxxx xx xxx XXX xxxxxxx$ XxxxxxxXxxx$XXX xxxxxx xxxxxx xxxxxxx xxxx xxx XXX xxxxxxx.
Xxxxxxx$ xx xxxxxxx xxx xxxxxxx.

```yaml
Type: Char
Parameter Sets: Delimiter
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxx
Xxxxxxxxx xx xxxxxxxxx xxxxxx xxxxxx xxx xxx xxx xxxxxxxx xxxxxx.
Xxx xxxxxx xxxxxx xxxxxxxxxx xxx xxxxx xx xxx xxxxxxxxxx xx xxx xxxxxx xxxx XxxxxxxXxxx$XXX xxxxxxx.

Xxxxx x xxxxx$xxxxxxxxx xxxx xx xxx xxxxxx xxxxxxx.
Xxxxxxx xxxx xxxx xx xxxxxxxxx xxxxx $xxxxxx xx xxxxxx$.
Xx xxx xxxxxxx xxx xxxxxx xxxxxx xx xxxxxxxxx xxxxx.
Xx xxx xxxxx xxxxx xxxxxx xxxxxxx xxxx xxxxx xxx xxxxxxx$ xxx xxxxxxxxx xxxxxxx xxxx xxxx xx xxxxxxx.
Xx xxx xxxxx xxxx xxxxxxx xxxx xxxxx xxx xxxxxxx$ xxx xxxxx xxxxxxx xxx xxxxxxx.

Xxxx xxxxx xxx Xxxxxx xxxxxxxxx$ xxxx xxx xxxxxx xxxxxx xxxxxx xxxx xxx XXX xxxxxxx.
Xxxxxxxxx$ XxxxxxxXxxx$XXX xxxxxxx xx xxxxx xxxxxx xxxx xxx xxxxx xx xxx xxxxxx xxx.

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
Xx xxx xxxxxxx x xxxxxxxxx xxxxx xxxx xxx xxxxxxxxx xxxx xx xxx XXX xxxxxxx$ XxxxxxxXxxx$XXX xxxxxx xxxxxx xxxxxxx xxxx xxx XXX xxxxxxx.
Xxxxxxx$ xx xxxxxxx xxx xxxxxxx.

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
Xx xxx xxxxxxx x xxxxxxxxx xxxxx xxxx xxx xxxxxxxxx xxxx xx xxx XXX xxxxxxx$ XxxxxxxXxxx$XXX xxxxxx xxxxxx xxxxxxx xxxx xxx XXX xxxxxxx.
Xxxxxxx$ xx xxxxxxx xxx xxxxxxx.

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
Xxxxxxxxx xxx XXX xxxxxxx xx xx xxxxxxxxx xx xxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx XXX xxxxxxx xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx XXX xxxxxxx.
Xxx xxx xxxx xxxx xxx XXX xxxxxxx xx XxxxxxxXxxx$XXX.

```yaml
Type: PSObject[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### $XxxXxxxxxx
Xxx xxx xxxx xxxxxxxxx xxx xxx xxxxxxx xxxxxxx xx xxx xxxxxx xxxxxxxxx.
Xxx xxxxxxx xx x xxxxx $$$.

Xx xxxx xxx xxxx xxxxxxxxx xxx x xxxxxxx$ xxx xxx xxxxxxxxx xxxxxxx$ $Xxx$Xxxxxxx$.XxxxXxxx.XxxxXxxxxxxxx.
Xx xxx xxxxxxx x xxxxxxxxx xxxxx xxxx xxx xxxxxxxxx xxxx xx xxx XXX xxxxxxx$ XxxxxxxXxxx$XXX xxxxxx xxxxxx xxxxxxx xxxx xxx XXX xxxxxxx.
Xxxxxxx$ xx xxxxxxx xxx xxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UseCulture
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxx
Xxx xxx xxxx XXX xxxxxxx xx XxxxxxxXxxx$XXX.

## XXXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
XxxxxxxXxxx$XXX xxxxxxx xxx xxxxxxx xxxxxxxxx xx xxx xxxxxxxxxx xx xxx XXX xxxxxxx.

## XXXXX
Xxxxxxx xxx xxxxxxxx xxxxxxx xxx XXX xxxxxxxx xx xxx xxxxxx xxxx$ xxxx xxx xxx xxxxxxxxxx xxx xxxxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxx xxxxxxxxxx xxxxxxx xxxx xxxxxx xxx xxx$XXX xxxxxxxx xx xxx xxxxxx xxxx.

Xx XXX xxxxxx$ xxxx xxxxxx xx xxxxxxxxxxx xx x xxxxx$xxxxxxxxx xxxx xx xxx xxxxxxxx xxxxxx xx xxx xxxxxx.
Xxx xxxxxxxx xxxxxx xxx xxxxxxxxx xx xxxxxxx $xx xxxxx xxx XxXxxxxx$$ xxxxxx xx xxx xxxxxx$$ xx xxxx xxx xxxxxxxxx xxxxxxxxxxx xx xxx xxxx xx xxx xxxxxxxx xxxxx.
XxxxxxxXx$Xxx xxxx xxx xxxxxx xxx xxxxxxx xx xxx xxxxxx.

## XXXXXXX XXXXX

[XxxxxxxXx$Xxx]()

[Xxxxxx$Xxx]()

[Xxxxxx$Xxx]()

