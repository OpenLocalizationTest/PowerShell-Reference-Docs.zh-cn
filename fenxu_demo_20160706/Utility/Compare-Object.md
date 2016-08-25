---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293945
schema: 2.0.0
---

# Compare-Object
## XXXXXXXX
Xxxxxxxx xxx xxxx xx xxxxxxx.

## XXXXXX

```
Compare-Object [-ReferenceObject] <PSObject[]> [-DifferenceObject] <PSObject[]> [-SyncWindow <Int32>]
 [-Property <Object[]>] [-ExcludeDifferent] [-IncludeEqual] [-PassThru] [-Culture <String>] [-CaseSensitive]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxxx$Xxxxxx xxxxxx xxxxxxxx xxx xxxx xx xxxxxxx.
Xxx xxx xx xxxxxxx xx xxx $xxxxxxxxx xxx$$ xxx xxx xxxxx xxx xx xxx $xxxxxxxxxx xxx.$

Xxx xxxxxx xx xxx xxxxxxxxxx xxxxxxxxx xxxxxxx x xxxxxxxx xxxxx xxxxxxxx xxxx xx xxx xxxxxx xxxx xxx xxxxxxxxx xxx $xxxxxxxxx xx xxx $$$ xxxxxx$$ xxxx xx xxx xxxxxx xxxx xxx xxxxxxxxxx xxx $xxxxxxxxx xx xxx $$$ xxxxxx$ xx$ xx xxx XxxxxxxXxxxx xxxxxxxxx xx xxxxxxxxx$ xx xxxx xxxxxxx $xxxxxxxxx xx xxx $$ xxxxxx$.

XXXX$  Xx xxx xxxxxxxxx xxx xx xxx xxxxxxxxxx xxx xx xxxx $$xxxx$$ Xxxxxxx$Xxxxxx xxxxxxxxx x xxxxxxxxxxx xxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>compare-object -referenceobject $(get-content C:\test\testfile1.txt) -differenceobject $(get-content C:\test\testfile2.txt)
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxx xx xxx xxxx xxxxx.
Xx xxxxxxxx xxxx xxx xxxxx xxxx xxxxxx xx xxx xxxx xx xx xxx xxxxx xxxx$ xxx xxxxx xxxx xxxxxx xx xxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>compare-object -referenceobject $(get-content C:\Test\testfile1.txt) -differenceobject $(get-content C:\Test\testfile2.txt) -includeequal
```

Xxxx xxxxxxx xxxxxxxx xxxx xxxx xx xxxxxxx xx xxx xxxx xxxxx.
Xx xxxxxxxx xxx xxxxx xx xxxxxxx xxxx xxxx xxxxx$ xxxxxxxxxx xxxxxxx xxxx xxxx xxxxxxx xx xxxx Xxxxxxxx0.xxx xx Xxxxxxxx0.xxx xx xxxxxxx xxxx xxxx xxxxxxx xx xxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$processes_before = get-process
PS C:\>notepad
PS C:\>$processes_after  = get-process
PS C:\>compare-object -referenceobject $processes_before -differenceobject $processes_after
```

Xxxxx xxxxxxxx xxxxxxx xxx xxxx xx xxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxxxx xx xxx xxxxxxxx.
Xx xxxxxx xxxx xx xxx $xxxxxxxxx$xxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxx Xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xxxxx xxx xxxxxx xxx xxxxxxxxx xxxxxxxxx xx xxx $xxxxxxxxx$xxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxxx$Xxxxxx xxxxxx xx xxxxxxx xxx xxx xxxx xx xxxxxxx xxxxxxx.
Xx xxxxxxxxxxx xxxxxxxxxxx xxxxxxx xxxx$ xxxxx xxxxxxx xxx xxx xxxxxxxx xx Xxxxxxx.

## XXXXXXXXXX

### -CaseSensitive
Xxxxxxxxx xxxx xxxxxxxxxxx xxxxxx xx xxxx$xxxxxxxxx.

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
Xxxxxxxxx xxx xxxxxxx xx xxx xxx xxxxxxxxxxx.

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

### -DifferenceObject
Xxxxxxxxx xxx xxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxxxxxx xxxxxxx.

```yaml
Type: PSObject[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ExcludeDifferent
Xxxxxxxx xxxx xxx xxxxxxxxxxxxxxx xx xxxxxxxx xxxxxxx xxxx xxx xxxxx.

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

### -IncludeEqual
Xxxxxxxx xxxxxxxxxxxxxxx xx xxxxxxxx xxxxxxx xxxx xxx xxxxx.
Xx xxxxxxx$ xxxx xxxxxxxxxxxxxxx xxxx xxxxxx xxxxxxx xxx xxxxxxxxx xxx xxxxxxxxxx xxxxxxx xxx xxxxxxxxx.

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

### -PassThru
Xxxxxx xxx xxxxxxx xxxx xxxxxxxx xx xxx xxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

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
Xxxxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxxxx xxx xxxxxxxxxx xxxxxxx xx xxxxxxx.

```yaml
Type: Object[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReferenceObject
Xxxxxxx xxxx xx x xxxxxxxxx xxx xxxxxxxxxx.

```yaml
Type: PSObject[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SyncWindow
Xxxxxxxxx xxx xxxxxx xx xxxxxxxx xxxxxxx xxxx Xxxxxxx$Xxxxxx xxxxxxxx xxxxx xxxxxxx xxx xx xxxxx xx x xxxxxxxxxx xx xxxxxxx.
Xxxxxxx$Xxxxxx xxxxxxxx xxxxxxxx xxxxxxx xxxx xx xxxxx$x xxxx xxx xxxxxx xx xxx xxxx xxxxxxxx xx x xxxxxxxxxx.
Xxx xxxxxxx xxxxx xx $$Xxx00$$$$XxxXxxxx$ xxxxx xxxxx xxxx Xxxxxxx$Xxxxxx xxxxxxxx xxx xxxxxx xxxxxx xxxxxxxxxx.

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

## XXXXXX

### System.Management.Automation.PSObject
Xxx xxx xxxx x XxxxxxxxxxXxxxxx xxxxxx xx Xxxxxxx$Xxxxxx.

## XXXXXXX

### None, or the objects that are different
Xxxx xxx xxx xxx XxxxXxxx xxxxxxxxx$ Xxxxxxx$Xxxxxx xxxxxxx xxx xxxxxxx xxxx xxxxxxxx.
Xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX

## XXXXXXX XXXXX

[ForEach-Object]()

[Group-Object]()

[Measure-Object]()

[New-Object]()

[Select-Object]()

[Sort-Object]()

[Tee-Object]()

[Where-Object]()

