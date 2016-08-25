---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293999
schema: 2.0.0
---

# Out-String
## XXXXXXXX
Xxxxx xxxxxxx xx xxx xxxx xx x xxxxxx xx xxxxxxx.

## XXXXXX

```
Out-String [-Stream] [-Width <Int32>] [-InputObject <PSObject>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxx xxxxxx xxxxxxxx xxx xxxxxxx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx xxxx xx xxxxx xx xxxxxxx.
Xx xxxxxxx$ Xxx$Xxxxxx xxxxxxxxxxx xxx xxxxxxx xxx xxxxxxx xxxx xx x xxxxxx xxxxxx$ xxx xxx xxx xxx xxx xxxxxx xxxxxxxxx xx xxxxxx Xxx$Xxxxxx xx xxxxxx xxx xxxxxx xx x xxxx.
Xxxx xxxxxx xxxx xxx xxxxxx xxx xxxxxxxxxx xxxxxx xxxxxx xx xxx xxxxx xx xxxxxxxxxxx xxxxxx xxxx xxxxxx xxxxxxxxxxxx xx xxxx xxxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-content C:\test1\testfile2.txt | out-string
```

Xxxx xxxxxxx xxxxx xxx xxxxxxx xx xxx Xxxxxxxx0.xxx xxxx xx xxx xxxxxxx xx x xxxxxx xxxxxx.
Xx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxx xx xxx xxxx.
Xxx xxxxxxxx xxxxxxxx $$$ xxxxx xxx xxxxxxx xx Xxx$Xxxxxx$ xxxxx xxxxx xxx xxxxxxx xx xxx xxxxxxx xx x xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command uses the Get-Culture cmdlet to get the regional settings. The pipeline operator (|) sends the result to the Select-Object cmdlet, which selects all properties (*) of the culture object that Get-Culture returned. The command then stores the results in the $c variable.
PS C:\>$c = Get-Culture | Select-Object *

The second command uses the Out-String cmdlet to convert the CultureInfo object to a series of strings (one string for each property). It uses the InputObject parameter to pass the $c variable to Out-String. The Width parameter is set to 100 characters per line to prevent truncation.
PS C:\>Out-String -InputObject $c -Width 100
```

Xxxxx xxxxxxxx xxx xxx xxxxxxxx xxxxxxxx xxx xxx xxxxxxx xxxx xxx xxxxxxx xxx xxxx xx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-alias | out-string -stream | select-string "Get-Command"
```

Xxxx xxxxxxx xxxxxxxxxxxx xxx xxxxxxxxxx xxxxxxx xxxxxxx xxxx xxxxxxx xxx xxxxxxx xxxx xxxxxxx.
Xxx xxxxxxx xxxxxxxx xxxxxxx xxxx xxxxxxx xxx xxxxxx $Xxx$Xxxxxxx$.
Xx xxxx xxx Xxx$Xxxxx xxxxxx xx xxx x xxx xx XxxxxXxxx xxxxxxx $xxx xxx xxxx xxxxx xx xxx xxxxxxx xxxxxxx$.

Xxx xxxxxxxx xxxxxxxx $$$ xxxxx xxx xxxxxx xx xxx Xxx$Xxxxx xxxxxx xx xxx Xxx$Xxxxxx xxxxxx$ xxxxx xxxxxxxx xxx xxxxxxx xx x xxxxxx xx xxxxxxx.
Xx xxxx xxx Xxxxxx xxxxxxxxx xx Xxx$Xxxxxx xx xxxx xxxx xxxxxx xxxxxxxxxxxx$ xxxxxxx xx xxxxxxxxxxxxx xxxx xxxx x xxxxxx xxxxxx.
Xxxxxxx xxxxxxxx xxxxxxxx xxxxx xxx xxxxxxx xx xxx Xxxxxx$Xxxxxx xxxxxx$ xxxxx xxxxxxx xxx xxxxxxx xxxx xxxxxxx $Xxx$Xxxxxxx$ xxxxxxxx xx xxx xxxxxx.

Xx xxx xxxx xxx Xxxxxx xxxxxxxxx$ xxx xxxxxxx xxxxxxxx xxx xx xxx xxxxxxx$ xxxxxxx Xxxxxx$Xxxxxx xxxxx $Xxx$Xxxxxxx$ xx xxx xxxxxx xxxxxx xxxx Xxx$Xxxxxx xxxxxxx$ xxx xxx xxxxxxxxx xxxxxxxx xxx xxxxxx xx x xxxxx.

## XXXXXXXXXX

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
Xxxxxxxxx xxx xxxxxxx xx xx xxxxxxx xx x xxxxxx.
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

### -Stream
Xxxxx xxx xxxxxxx xxx xxxx xxxxxx xxxxxxxxxx.
Xx xxxxxxx$ xxx xxxxxxx xxx xxxx xxxxxx xxx xxxxxxxxxxx xxx xxxx xx x xxxxxx xxxxxx.

Xx xxx xxx Xxxxxx xxxxxxxxx$ xxxx $$Xxxxxx$ xx xxx xxxxx$ $xxx$.

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

### -Width
Xxxxxxxxx xxx xxxxxx xx xxxxxxxxxx xx xxxx xxxx xx xxxxxx.
Xxx xxxxxxxxxx xxxxxxxxxx xxx xxxxxxxxx$ xxx xxxxxxx.
Xx xxx xxxx xxxx xxxxxxxxx$ xxx xxxxx xx xxxxxxxxxx xx xxx xxxxxxxxxxxxxxx xx xxx xxxx xxxxxxx.
Xxx xxxxxxx xxxxx xxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xx 00 $xxxxxxxxxx$.

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
Xxx xxx xxxx xxxxxxx xx Xxx$Xxxxxx.

## XXXXXXX

### System.String
Xxx$Xxxxxx xxxxxxx xxx xxxxxx xxxx xx xxxxxxx xxxx xxx xxxxx xxxxxx.

## XXXXX
Xxx xxxxxxx xxxx xxxxxxx xxx Xxx xxxx $xxx Xxx xxxxxxx$ xx xxx xxxxxx xxxxxxx$ xxxx xxxx xxxxxx xxxx xxx xxxx xxxx xx xxx xxxxxxxxx xxxxxxx xxxxxxxxxxx.
Xx xxx xxxx xx xxxxxxxxxxx xxxxxx xx xx Xxx xxxxxx$ xxx xxxxxx xxxxx xx xx x xxxxxxxxxx xxxxxx xxxxxx xxxxxxxxx xx.

Xxx Xxx xxxxxxx xx xxx xxxx xxxxxxxxxx xxxx xxxx  xxxxx xx xxxx xxxxx.
Xx xxxx xxxx xx xx Xxx xxxxxx$ xxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xx x Xxxxxxx XxxxxXxxxx xxxxxxx xx xxx xxxxxx.
Xxx xxx xxxx xxxxx xxxx xx x xxxxxxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxx xxx xxxx xx xxx xxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxx xxxxxxxx.

## XXXXXXX XXXXX

[Out-Default]()

[Out-File]()

[Out-Host]()

[Out-Null]()

[Out-Printer]()

