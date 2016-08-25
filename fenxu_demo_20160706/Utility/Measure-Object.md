---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293990
schema: 2.0.0
---

# Measure-Object
## XXXXXXXX
Xxxxxxxxxx xxx xxxxxxx xxxxxxxxxx xx xxxxxxx$ xxx xxx xxxxxxxxxx$ xxxxx$ xxx xxxxx xx xxxxxx xxxxxxx$ xxxx xx xxxxx xx xxxx.

## XXXXXX

### GenericMeasure (Default)
```
Measure-Object [-InputObject <PSObject>] [[-Property] <String[]>] [-Sum] [-Average] [-Maximum] [-Minimum]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### TextMeasure
```
Measure-Object [-InputObject <PSObject>] [[-Property] <String[]>] [-Line] [-Word] [-Character]
 [-IgnoreWhiteSpace] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxxx$Xxxxxx xxxxxx xxxxxxxxxx xxx xxxxxxxx xxxxxx xx xxxxxxx xxxxx xx xxxxxx.
Xxxxxxx$Xxxxxx xxxxxxxx xxxxx xxxxx xx xxxxxxxxxxxx$ xxxxxxxxx xx xxx xxxxxxxxxx xx xxx xxxxxxx.

Xxx Xxxxxxx$Xxxxxx xxxxxx xxxxxxxx xxxxxxxxxxxx xx xxx xxxxxxxx xxxxxx xx xxxxxxx.
Xx xxx xxxxx xxxxxxx xxx xxxxxxxxx xxx xxxxxxx$ xxxxxxx$ xxx$ xxx xxxxxxx xx xxx xxxxxxx xxxxxx.
Xxx xxxx xxxxxxx$ xx xxx xxxxx xxx xxxxxxxxx xxx xxxxxx xx xxxxx$ xxxxx$ xxx xxxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem | measure-object
```

Xxxx xxxxxxx xxxxxx xxx xxxxx xxx xxxxxxx xx xxx xxxxxxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem | measure-object -property length -minimum -maximum -average
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxx$ xxxxxxx$ xxx xxx xx xxx xxxxx xx xxx xxxxx xx xxx xxxxxxx xxxxxxxxx$ xxx xxx xxxxxxx xxxx xx x xxxx xx xxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-content C:\test.txt | measure-object -character -line -word
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxx xx xxxxxxxxxx$ xxxxx$ xxx xxxxx xx xxx Xxxx.xxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | measure-object -property workingset -minimum -maximum -average
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxx$ xxxxxxx$ xxx xxxxxxx xxxxx xx xxx xxxxxxx xxxx xx xxx xxxxxxxxx xx xxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>import-csv d:\test\serviceyrs.csv | measure-object -property years -minimum -maximum -average
```

Xxxx xxxxxxx xxxxxxxxxx xxx xxxxxxx xxxxx xx xxxxxxx xx xxx xxxxxxxxx xx x xxxxxxx.

Xxx XxxxxxxXxx.xxx xxxx xx x XXX xxxx xxxx xxxxxxxx xxx xxxxxxxx xxxxxx xxx xxxxx xx xxxxxxx xx xxxx xxxxxxxx.
Xxx xxxxx xxx xx xxx xxxxx xx x xxxxxx xxx xx $XxxXx$ Xxxxx$.

Xxxx xxx xxx Xxxxxx$Xxx xx xxxxxx xxx xxxx$ xxx xxxxxx xx x XXXxxxxxXxxxxx xxxx xxxx xxxxxxxxxx xx XxxXx xxx Xxxxx.
Xxx xxx xxx Xxxxxxx$Xxxxxx xx xxxxxxxxx xxx xxxxxx xx xxxxx xxxxxxxxxx$ xxxx xxxx xxx xxxxx xxxxxxxx xx xx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem | measure-object -property psiscontainer -max -sum -min -average

Count    : 126
Average  : 0.0634920634920635
Sum      : 8
Maximum  : 1
Minimum  : 0
Property : PSIsContainer
```

Xxxx xxxxxxx xxxxxxxxxxxx xxx Xxxxxxx$Xxxxxx xxx xxxxxxx Xxxxxxx xxxxxx.
Xx xxxx xxxx$ xx xxxx xxx XXXxXxxxxxxxx Xxxxxxx xxxxxxxx xx xxxxxxx xxx xxxxxxxxx xx xxxxxxx $xx. xxxxx$ xx xxx xxxxxxx xxxxxxxxx.

## XXXXXXXXXX

### -Average
Xxxxxxxx xxx xxxxxxx xxxxx xx xxx xxxxxxxxx xxxxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: GenericMeasure
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Character
Xxxxxx xxx xxxxxx xx xxxxxxxxxx xx xxx xxxxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: TextMeasure
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IgnoreWhiteSpace
Xxxxxxx xxxxx xxxxx xx xxxx xxxxxx xxx xxxxxxxxx xxxxxx.
Xx xxxxxxx$ xxxxx xxxxx xx xxx xxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: TextMeasure
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
Xxxxxxxxx xxx xxxxxxx xx xx xxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx$ xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.

Xxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xxxx Xxxxxxx$Xxxxxx$ xxxxxxx xx xxxxxx xxxxxxx xxxxxxx xx Xxxxxxx$Xxxxxx$ xxx XxxxxXxxxxx xxxxx$xxxx xx xxx xxxxx xx x xxxxxxxxxx xxxx xx xxx xxxxxx xx x xxxxxxx$ xxxx xx $XxxxxXxxxxx $Xxx$Xxxxxxx$$xx xxxxxxx xx x xxxxxx xxxxxx.
Xxxxxxx XxxxxXxxxxx xxxxxx xxxxxx xxxxxxxxxx xxxxxxxxxx xxxx xx xxxxx xx xxxxxxxxxx xx xxxxxxx$ xx xx xxxxxxxxxxx xxxx xx xxx xxx Xxxxxxx$Xxxxxx xx xxxxxxx x xxxxxxxxxx xx xxxxxxx xxx xxxxx xxxxxxx xxxx xxxx xxxxxxxx xxxxxx xx xxxxxxx xxxxxxxxxx$ xxx xxx Xxxxxxx$Xxxxxx xx xxx xxxxxxxx$ xx xxxxx xx xxx xxxxxxxx xx xxxx xxxxx.

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

### -Line
Xxxxxx xxx xxxxxx xx xxxxx xx xxx xxxxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: TextMeasure
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Maximum
Xxxxxxxx xxx xxxxxxx xxxxx xx xxx xxxxxxxxx xxxxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: GenericMeasure
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Minimum
Xxxxxxxx xxx xxxxxxx xxxxx xx xxx xxxxxxxxx xxxxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: GenericMeasure
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Property
Xxxxxxxxx xxx xx xxxx xxxxxxx xxxxxxxxxx xx xxxxxxx.
Xxx xxxxxxx xx xxx Xxxxx $Xxxxxx$ xxxxxxxx xx xxx xxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Sum
Xxxxxxxx xxx xxx xx xxx xxxxxx xx xxx xxxxxxxxx xxxxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: GenericMeasure
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Word
Xxxxxx xxx xxxxxx xx xxxxx xx xxx xxxxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: TextMeasure
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.Management.Automation.PSObject
Xxx xxx xxxx xxxxxxx xx Xxxxxxx$Xxxxxx.

## XXXXXXX

### Microsoft.PowerShell.Commands.GenericMeasureInfo, Microsoft.PowerShell.Commands.TextMeasureInfo, Microsoft.PowerShell.Commands.GenericObjectMeasureInfo
Xx xxx xxx xxx Xxxx xxxxxxxxx$ Xxxxxxx$Xxxxxx xxxxxxx x XxxxXxxxxxxXxxx xxxxxx.
Xxxxxxxxx$ xx xxxxxxx x XxxxxxxXxxxxxxXxxx xxxxxx.

## XXXXX

## XXXXXXX XXXXX

[Compare-Object]()

[ForEach-Object]()

[Group-Object]()

[New-Object]()

[Select-Object]()

[Sort-Object]()

[Tee-Object]()

[Where-Object]()

