---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293962
schema: 2.0.0
---

# Format-Table
## XXXXXXXX
Xxxxxxx xxx xxxxxx xx x xxxxx.

## XXXXXX

```
Format-Table [-AutoSize] [-HideTableHeaders] [-Wrap] [[-Property] <Object[]>] [-GroupBy <Object>]
 [-View <String>] [-ShowError] [-DisplayError] [-Force] [-Expand <String>] [-InputObject <PSObject>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxxxx xxxxxx xxxxxxx xxx xxxxxx xx x xxxxxxx xx x xxxxx xxxx xxx xxxxxxxx xxxxxxxxxx xx xxx xxxxxx xx xxxx xxxxxx.
Xxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxx xxxxxx xxx xxxxxxxxxx xxxx xxx xxxxxxxxx xx xxxx xxxxxx$ xxx xxx xxx xxx xxx Xxxxxxxx xxxxxxxxx xx xxxxxx xxx xxxxxxxxxx xxxx xxx xxxx xx xxx.

Xxx xxx xxxx xxx x xxxx xxxxx xx xxx xxxxxxxxxx xxxxxxxxxx xx xx xxxxxx xxxxxx xxxxxxxxxx xx xxx xx xxxxxxx xxx xxxxxx xxxxxxxx xx xxx xxxxx.
Xx xxx x xxxxxxxxxx xxxxxxxx$ xxx xxx Xxxxxxxx xx XxxxxXx xxxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-pssnapin | format-table -auto
```

Xxxx xxxxxxx xxxxxxx xxxxxxxxxxx xxxxx Xxxxxxx XxxxxXxxxx xxxx$xxx xx x xxxxx.
Xx xxxxxxx$ xxxx xxx xxxxxxxxx xx x xxxx.
Xxx Xxx$XXXxxxxx xxxxxx xxxx xxxxxxx xxxxxxxxxxxx xxx xxxx$xxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxxx xxx xxxxxx xx xxx Xxxxxx$Xxxxx xxxxxxx.
Xxxxxx$Xxxxx xxxxxxx xxx xxxxxxx xx x xxxxx.
Xxx Xxxxxxxx xxxxxxxxx xxxxxxx xxx xxxxxx xxxxxx xx xxxxxxxx xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | sort-object -property basepriority | format-table -groupby basepriority -wrap
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xx xxxxxx xxxx xxx xxxx xxxx xxxxxxxx.

Xxx Xxx$Xxxxxxx xxxxxx xxxx xxxxxxx xxxxxxxxxxxx xxxx xxxxxxx xx xxx xxxxxxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxxx xxx xxxxxx xx xxx Xxxx$Xxxxxx xxxxxx$ xxxxx xxxxx xxx xxxxxxx xx xxxxx xx xxxxx xxxx xxxxxxxx.

Xxxxxxx xxxxxxxx xxxxxxxx xxxxxx xxx xxxxxxx xx xxx Xxxxxx$Xxxxx xxxxxx.
Xxx XxxxxXx xxxxxxxxx xxxxxxxx xxx xxxx xxxxx xxx xxxxxxxxx xxxx xxxxxx xxxxx xx xxx xxxxx xx xxxxx XxxxXxxxxxxx xxxxxxxx.
Xxx Xxxx xxxxxxxxx xxxxxxx xxxx xxxx xx xxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | sort-object starttime | format-table -view starttime
```

Xxxx xxxxxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xx xxxxx xxxxx xx xxx xxxxx xxxx xx xxx xxxxxxx.
Xx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxxxxxx xxxxxxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxx xxx xxxxxx xx Xxx$Xxxxxxx xx xxx Xxxx$Xxxxxx xxxxxx$ xxxxx xxxxx xx xxxxx xx xxx XxxxxXxxx xxxxxxxx.
Xxxxxxx xxxxxxxx xxxxxxxx xxxxx xxx xxxxxx xxxxxxx xx Xxxxxx$Xxxxx.

Xxx Xxxx xxxxxxxxx xx xxxx xx xxxxxx xxx XxxxxXxxx xxxx xxxx xx xxxxxxx xx xxx XxxXxxXxxxx.xxxxxx.xx0xxx xxxxxxxxxx xxxx xxx Xxxxxx.Xxxxxxxxxxx.Xxxxxxx xxxxxxx$ xxxx xx xxxxx xxxxxxxx xx Xxx$Xxxxxxx.
Xxxx xxxx xxxxxxxx xxx XxxxxXxxx xx xxx xxxxxxx xx x xxxxx xxxx xxx xxxx xxxxxx xxx xxxxxxxxx xx xxxxx xxxx.

Xxx XxxXxxXxxxx.xxxxxx.xx0xxx xxxxxxxxxx xxxx xxxx xxxxxxxx x Xxxxxxxx xxxx xxx xxxxxxxxx$ xxx xxx xxx xxxxxx xxxx xxx xxxxxx.xx0xxx xxxxx xxxx xxxxxxxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-service | format-table -property Name, DependentServices
```

Xxxx xxxxxxx xxxxxxxx xxx xx xxx xxxxxxxx xx xxx xxxxxxxx xx x xxxxx xxxx xxx xxxxxxx$ Xxxx xxx XxxxxxxxxXxxxxxxx.
Xxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xx xxx xxxxxxxx xx xxx xxxxxxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxx xxx xxxxxxx xx xxx Xxxxxx$Xxxxx xxxxxx$ xxxxx xxxxxxx xxx xxxxxx xx x xxxxx.
Xxx Xxxxxxxx xxxxxxxxx xxxxxxxxx xxx xxxxxxxxxx xxxx xxxxxx xx xxx xxxxx xx xxxxxxx.
Xxx xxxx xx xxx Xxxxxxxx xxxxxxxxx xx xxxxxxxx$ xx xxx xxx xxxx xx $$xxxxxx$xxxxx xxxx$ xxxxxxxxxxxxxxxxx$$.

Xxxxxxxx xxx XxxxxxxxxXxxxxxxx xxx xxxx xxx xx xxx xxxxxxxxxx xx xxxxxxx xxxxxxx.
Xx xxxx xxx xx xxx xxxxxxxxxx$ xxxx $xxx$xxxxxxx $ xxx$xxxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process notepad | format-table ProcessName, @{Label="TotalRunningTime"; Expression={(get-date) - $_.StartTime}}
```

Xxxx xxxxxxx xxxxx xxx xx xxx x xxxxxxxxxx xxxxxxxx xx x xxxxx.
Xxx xxxxxxx xxxxxxxx x xxxxx xxxx xxx xxxxxxx xxxx xxx xxxxx xxxxxxx xxxx xx xxx Xxxxxxx xxxxxxxxx xx xxx xxxxx xxxxxxxx.
Xxx xxxxx xxxxxxx xxxx xx xxxxxxxxxx xx xxxxxxxxxxx xxx xxxxx xxxx xx xxxx xxxxxxx xxxx xxx xxxxxxx xxxx.

Xxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxxxx xxxxx $Xxxxxxx$ xx xxx xxxxx xxxxxxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxx xxx xxxxxxx xx Xxxxxx$Xxxxx$ xxxxx xxxxxxxx x xxxxx xxxx xxx xxxxxxx$ XxxxxxxXxxx$ x xxxxxxxx xxxxxxxx xx xxxxxxxxx$ xxx XxxxxXxxxxxxXxxx$ x xxxxxxxxxx xxxxxxxx.

Xxx XxxxxXxxxxxxXxxx xxxxxxxx xx xxxxxxxxx xx x xxxx xxxxx xxxx xxx xxxx$ Xxxxx xxx Xxxxxxxxxx.
Xxx xxxx xx xxx xxxxxxxx xx xxxxxxxx xx xxx Xxxxx xxx.
Xxx xxxxxxxxxxx xx xxxxxxxx xx xxx Xxxxxxxxxx xxx.
Xxx xxxxxxxxxx xxxx xxx XxxxxXxxx xxxxxxxx xx xxxx xxxxxxx xxxxxx xxx xxxxxxxxx xx xxxx xxx xxxxxx xx x Xxx$Xxxx xxxxxxx$ xxxxx xxxx xxx xxxxxxx xxxx $xxx xxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$processes = get-wmiobject -ComputerName Server01 win32_process -filter "name='notepad.exe'"
PS C:\>$processes | format-table ProcessName, @{ Label = "Total  Running Time"; Expression={(get-date) - $_.ConvertToDateTime($_.CreationDate)}}
```

Xxxxx xxxxxxxx xxx xxxxxxx xx xxx xxxxxxxx xxxxxxx$ xxxxxx xxxx xxxxx xxxxxxxx xxx xxx Xxx$XxxXxxxxx xxxxxx xxx xxx Xxx00$Xxxxxxx xxxxx xx xxxxxxx xxxxxxxxxxx xxxxx Xxxxxxx xxxxxxxxx xx x xxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XxxXxxxxx xxxxxx xx xxx xxxxxxxxx xx xxx Xxxxxxx Xxxxxxxxxx Xxxxxxxxxxxxxxx $XXX$ Xxx00$Xxxxxxx xxxxx xxxx xxxxxxxxx xxx xx xxx xxxxxxxxx xx xxx Xxxxxx00 xxxxxxxx xxxx xxx xxxxx Xxxxxxx.xxx.
Xxx xxxxxxx xxxxxx xxx xxxxxxx xxxxxxxxxxx xx xxx $xxxxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xxxxxxxxxxx xx xxx $xxxxxxxxx xxxxxxxx xx xxx Xxxxxx$Xxxxx xxxxxx$ xxxxx xxxxxxxx xxx XxxxxxxXxxx xx xxxx xxxxxxx xxxxx xxxx x xxx xxxxxxxxxx xxxxxxxx.

Xxx xxxxxxx xxxxxxx xxx xxxx xx xxx xxx xxxxxxxxxx xxxxxxxx$ Xxxxx Xxxxxxx Xxxx$ xx xxx Xxxxx xxx.
Xxx xxxxxx xxxxx xxxx xx xxxxxxxx xx xxx Xxxxxxxxxx xxx xxxxxxxxxx xxx xxxx xxx xxxxxxx xxx xxxx xxxxxxx xx xxxxxxxxxxx xxx xxxxxxxx xxxx xx xxx xxxxxxx xxxx xxx xxxxxxx xxxx.
Xxx Xxx$Xxxx xxxxxx xxxx xxx xxxxxxx xxxx.
Xxx XxxxxxxXxXxxxXxxx xxxxxx xxxxxxxx xxx XxxxxxxxXxxx xxxxxxxx xx xxx Xxx00$Xxxxxxx xxxxxx xxxx x XXX XXX$XXXXXXXX xxxxxx xx x Xxxxxxxxx .XXX Xxxxxxxxx XxxxXxxx xxxxxx xxxx xxx xx xxxxxxxx xxxx xxx xxxxxx xx Xxx$Xxxx.
Xxxx$ xxx xxxxxxxxx xxxxxxxx xxxx xx xxxxxxxxxx xxxx xxx xxxxxxx xxxx.
Xxx xxxxxx xx xxx xxxxx xx Xxxxx Xxxxxxx Xxxx.

## XXXXXXXXXX

### -AutoSize
Xxxxxxx xxx xxxxxx xxxx xxx xxxxxx xx xxxxxxx xxxxx xx xxx xxxxx xx xxx xxxx.
Xx xxxxxxx$ xxx xxxxxx xxxx xxx xxxxxx xxx xxxxxxxxxx xx xxx xxxx.

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

### -DisplayError
Xxxxxxxx xxxxxx xx xxx xxxxxxx xxxx.
Xxxx xxxxxxxxx xx xxxxxx xxxx$ xxx xxx xx xxxx xx x xxxxxxxxx xxx xxxx xxx xxx xxxxxxxxxx xxxxxxxxxxx xx x Xxxxxx$Xxxxx xxxxxxx$ xxx xxx xxxxxxxxxxx xx xxx xxxxxx xx xx xxxxxxx.
Xxx xxxxxxxxx xxxxx xx xxxxxxx xx xxx xxxxxxx xx xxxxxx xxx XxxxxxxXxxxx xxxxxxxxx xxxx xx xxxxxxxxxx.

XX $$ Xxx$Xxxx $ Xxxxxx$Xxxxx XxxXxXxxx$$ $$ $ $xxxx $ $XxxxXxxxx XxxXxXxxx  $$ $ $xxxx
--------- ------------
Xxxxxxxxx $XXX

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

### -Expand
Xxxxxxx xxx xxxxxxxxxx xxxxxx$ xx xxxx xx xxx xxxxxxx xx xxx xxxxxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx xx xxxxxx xxxxxxx xxxx xxxxxxx xxx XXxxxxxxxxx $Xxxxxx.Xxxxxxxxxxx$ xxxxxxxxx.
Xxx xxxxxxx xxxxx xx XxxxXxxx.

Xxxxx xxxxxx xxx$

$$ XxxxXxxx$ Xxxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxx xx xxx xxxxxxxxxx.
$$ XxxxXxxx$ Xxxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxxxxx xxxxxx.
$$ Xxxx$ Xxxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxxxxx xxxxxx xxx xxx xxxxxxxxxx xx xxxxxxx xx xxx xxxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: CoreOnly, EnumOnly, Both

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Xxxxxxx xxx xxxxxx xx xxxxxxx xxx xx xxx xxxxx xxxxxxxxxxx.
Xxx xxxx xxx XxxxxxxXxxxx xx XxxxXxxxx xxxxxxxxxx.
Xx xxxxxxx$ xxxx xx xxxxx xxxxxx xx xxxxxxx xx xxx xxxxx xx xxxxxxx xxxxxxx$ xxxx xxxx xx xxx xxxxx xxxxxxxxxxx xx xxxxxxxxx.

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

### -GroupBy
Xxxxxxxx xxxxxx xxxxxx xx xxxxxxxx xxxxxx xxxxx xx x xxxxxxxx xxxxx.
Xxx xxxxxxx$ xxx xxx xxx XxxxxXx xx xxxx xxxxxxxx xx xxxxxxxx xxxxxx xxxxx xx xxxxx xxxxxx.

Xxxxx xx xxxxxxxxxx xx x xxxxxxxx xx xxx xxxxxx.
Xxx xxxxxx xxxx xx xxxxxx xxxxxx xxx xxxx xx xx Xxxxxx$Xxxxx.

Xxx xxxxx xx xxx XxxxxXx xxxxxxxxx xxx xx x xxx xxxxxxxxxx xxxxxxxx.
Xx xxxxxx x xxxxxxxxxx$ xxxxxxxx$ xxx x xxxx xxxxx.
Xxxxx xxxx xxx$

$$ Xxxx $xx Xxxxx$ $$xxxxxx$$$$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxx xxxxx$$$$$ XxxxxxXxxxxx $$xxxxxx\>

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HideTableHeaders
Xxxxx xxx xxxxxx xxxxxxxx xxxx xxx xxxxx.

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
Xxxxxxxxx xxx xxxxxxx xx xx xxxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx$ xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.

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

### -Property
Xxxxxxxxx xxx xxxxxx xxxxxxxxxx xxxx xxxxxx xx xxx xxxxxxx xxx xxx xxxxx xx xxxxx xxxx xxxxxx.
Xxxx xxx xx xxxx xxxxxxxx xxxxx $xxxxxxxxx xx xxxxxx$$ xx xxx x xxxx xxxxx xx xxxxxxx x xxxxxxxxxx xxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

Xx xxx xxxx xxxx xxxxxxxxx$ xxx xxxxxxxxxx xxxx xxxxxx xx xxx xxxxxxx xxxxxx xx xxx xxxxxx xxxxx xxxxxxxxx.
Xxx xxxxxxxxx xxxx $$Xxxxxxxx$$ xx xxxxxxxx.
Xxx xxxxxx xxx xxx Xxxxxxxx xxx Xxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

Xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx xxx xx x xxx xxxxxxxxxx xxxxxxxx.
Xx xxxxxx x xxxxxxxxxx$ xxxxxxxx$ xxx x xxxx xxxxx.
Xxxxx xxxx xxx$

$$ Xxxx $xx Xxxxx$ $$xxxxxx$$$$$ Xxxxxxxxxx $$xxxxxx$$ xx $$xxxxxx xxxxx$$$$$ XxxxxxXxxxxx $$xxxxxx$$$$$ Xxxxx $$xxx00$$$$$ Xxxxxxxxx  $xxxxx xxx xx $Xxxx$$ $Xxxxxx$$ xx $Xxxxx$$

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

### -ShowError
Xxxxx xxxxxx xxxxxxx xxx xxxxxxxx.
Xxxx xxxxxxxxx xx xxxxxx xxxx$ xxx xxx xx xxxx xx x xxxxxxxxx xxx xxxx xxx xxx xxxxxxxxxx xxxxxxxxxxx xx x Xxxxxx$Xxxxx xxxxxxx$ xxx xxx xxxxxxxxxxx xx xxx xxxxxx xx xx xxxxxxx.
Xxx xxxxxxxxx xxxxx xx xxxxxxx xx xxx xxxxxxx xx xxxxxx xxx XxxxXxxxx xxxxxxxxx xxxx xx xxxxxxxxxx.

XX $$ Xxx$Xxxx $ Xxxxxx$Xxxxx XxxXxXxxx$$ $$ $ $xxxx $ $XxxxXxxxx XxxXxXxxx  $$ $ $xxxx
--------- ------------
Xxxxxxxxx

Xxxxxx xx xxxxxxxx xxxxxxxxxx $ $$ $ $xxxx $.
$ XxxxxxxxXxxx          $ XxxxxxxXxxxxxxx$ $00$00$0000 0$00$00 XX$XXXxxxxx$ $$$$$ XxxxxxxXxxxxxxxx $ XxxxxXxxxxxxxxXxxxxXx $ xxxXxxxxxxxxxXxxxx

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

### -View
Xxxxxxxxx xxx xxxx xx xx xxxxxxxxx xxxxx xxxxxx xx $xxxx.$ Xxx xxxxxx xxx xxx Xxxxxxxx xxx Xxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

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

### -Wrap
Xxxxxxxx xxxx xxxx xxxxxxx xxx xxxxxx xxxxx xx xxx xxxx xxxx.
Xx xxxxxxx$ xxxx xxxx xxxxxxx xxx xxxxxx xxxxx xx xxxxxxxxx.

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
Xxx xxx xxxx xxx xxxxxx xx Xxxxxx$Xxxxx.

## XXXXXXX

### Microsoft.PowerShell.Commands.Internal.Format
Xxxxxx$Xxxxx xxxxxxx xxxxxx xxxxxxx xxxx xxxxxxxxx xxx xxxxx.

## XXXXX
Xxx XxxxxXx xxxxxxxxx xxxxxxx xxxx xxx xxxxxxx xxx xxxxxx.
Xxxxxx xxxxx Xxxxxx$Xxxxx xx xxxxx xxx xxxxxxx$ xxx xxx Xxxx$Xxxxxx xxxxxx xx xxxx xxxx.

Xxx Xxxx xxxxxxxxx xxxx xxx xxxxxxx xx xxxxxxxxx xxxxxx xxx xxx xxxxx.
Xxx xxx xxx xxx xxxxx xxxxxxx xx xxx $.xxxxxx.XX0XXX xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxx xx xxx xxx xxxxxx xxxx xxx xxxxx xx xxx XX0XXX xxxxx xxx xxxx xxx xxx XXxxxxx$XxxxxxXxxx xxxxxx xx xxxxxxx xxxx xx Xxxxxxx XxxxxXxxxx.

Xxx xxxxxxxxx xxxxx xxx xxx Xxxx xxxxxxxxx xxxx xxx xxx xxxxx xxxxxx.
Xx xx xxxx xxx$ xxx xxxxxxx xxxxx.
Xx xxx xxxxxxxxx xxxx xx x xxxx$ xxx xxx Xxxxxx$Xxxx xxxxxx.
Xx xxx xxxxxxxxx xxxx xx xxxxxxx x xxxx xxx x xxxxx$ xxx xxx X$Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.Xxxxxx$Xxxxxx xxxxxx.

## XXXXXXX XXXXX

[Format-Custom]()

[Format-List]()

[Format-Wide]()

