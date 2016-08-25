---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293998
schema: 2.0.0
---

# Out-Printer
## XXXXXXXX
Xxxxx xxxxxx xx x xxxxxxx.

## XXXXXX

```
Out-Printer [[-Name] <String>] [-InputObject <PSObject>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxxx xxxxxx xxxxx xxxxxx xx xxx xxxxxxx xxxxxxx xx xx xx xxxxxxxxx xxxxxxx$ xx xxx xx xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-content $pshome\about_signing.help.txt | Out-Printer
```

Xxxx xxxxxxx xxxxxx xxx xxxxxxx xx xxx xxxxx$Xxxxxxx Xxxx xxxxx xx xxx xxxxxxx xxxxxxx.
Xxxx xxxxxxx xxxxx xxx xxx xx xxxxx x xxxx$ xxxx xxxxxx Xxx$Xxxxxxx xxxx xxx xxxx x Xxxx xxxxxxxxx.

Xxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxxx xx xxx Xxxx xxxxx.
Xxx xxxx xxxxxxxx $xxxxxx$ x xxxxx$xx xxxxxxxx xxxx xxxxxx xxx xxxxxxxxxxxx xxxxxxxxx xxx Xxxxxxx XxxxxXxxxx.
X xxxxxxxx xxxxxxxx $$$ xxxxxx xxx xxxxxxx xx Xxx$Xxxxxxx$ xxxxx xxxxx xx xx xxx xxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>"Hello, World" | out-printer -name "\\Server01\Prt-6B Color"
```

Xxxx xxxxxxx xxxxxx $Xxxxx$ Xxxxx$ xx xxx $Xxx$0X Xxxxx$ xxxxxxx xx Xxxxxx00.
Xxxx xxxxxxx xxxx xxx Xxxx xxxxxxxxx xx xxxxxxx xxx xxxxxxxxx xxxxxxx.
Xxxxxxx xxx xxxxxxxxx xxxx xx xxxxxxxx$ xxx xxx xxxx xx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$h = get-help -full get-wmiobject
PS C:\>out-printer -inputobject $h
```

Xxxxx xxxxxxxx xxxxx xxx xxxx xxxxxxx xx xxx Xxxx xxxxx xxx Xxx$XxxXxxxxx.
Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx xxx xxxx xxxxxxx xx xxx Xxxx xxxxx xxx Xxx$XxxXxxxxx xxx xxxxxx xx xx xxx $x xxxxxxxx.
Xxx xxxxxx xxxxxxx xxxxx xxx xxxxxxx xx xxx xxxxxxx xxxxxxx.
Xx xxxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxx xxx xxxxx xx xxx $x xxxxxxxx xx Xxx$Xxxxxxx.

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
Xxxxxxxxx xxx xxxxxxx xx xx xxxx xx xxx xxxxxxx.
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

### -Name
Xxxxxxxxx xxx  xxxxxxxxx xxxxxxx.
Xxx xxxxxxxxx xxxx $$Xxxx$$ xx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: PrinterName

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.Management.Automation.PSObject
Xxx xxx xxxx xxx xxxxxx xx Xxx$Xxxxxxx.

## XXXXXXX

### None
Xxx$Xxxxxxx xxxx xxx xxxxxx xxx xxxxxxx.

## XXXXX
Xxx xxx xxxx xxxxx xx Xxx$Xxxxxxx xx xxx xxxxx$xx xxxxx$ $xx$.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx.

Xxx xxxxxxx xxxx xxxxxxx xxx Xxx xxxx $xxx Xxx xxxxxxx$ xx xxx xxxxxx xxxxxxx$ xxxx xxxx xxxxxx xxxx xxx xxxx xxxx xx xxx xxxxxxxxx xxxxxxx xxxxxxxxxxx.
Xx xxx xxxx xx xxxxxxxxxxx xxxxxx xx xx Xxx xxxxxx$ xxx xxxxxx xxxxx xx xx x xxxxxxxxxx xxxxxx xxxxxx xxxxxxxxx xx.

Xxx Xxx xxxxxxx xx xxx xxxx xxxxxxxxxx xxx xxxxx xx xxxx xxxxx.
Xx xxxx xxxx xx xx Xxx xxxxxx$ xxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xx x Xxxxxxx XxxxxXxxxx xxxxxxx xx xxx xxxxxx.
Xxx xxx xxxx xxxxx xxxx xx x xxxxxxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxx xxx xxxx xx xxx xxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxx xxxxxxxx.

Xxx$Xxxxxxx xxxxx xxxx$ xxx xx xxxx xxx xxxx xxx xxxxxx xxxxxxx.
Xx xxx xxxx xxx xxxxxx xx Xxx$Xxxxxxx xx Xxx$Xxxxxx$ Xxx$Xxxxxx xxxxxxx xxxx xx xxxxxxx xxxx xxxx xxxxxxxxx.

## XXXXXXX XXXXX

[Out-Default]()

[Out-File]()

[Out-Host]()

[Out-Null]()

[Out-String]()

