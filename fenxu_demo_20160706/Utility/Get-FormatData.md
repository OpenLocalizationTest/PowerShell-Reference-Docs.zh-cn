---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293969
schema: 2.0.0
---

# Get-FormatData
## XXXXXXXX
Xxxx xxx xxxxxxxxxx xxxx xx xxx xxxxxxx xxxxxxx.

## XXXXXX

```
Get-FormatData [[-TypeName] <String[]>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$XxxxxxXxxx xxxxxx xxxx xxx xxxxxxxxxx xxxx xx xxx xxxxxxx xxxxxxx.

Xxx xxxxxxxxxx xxxx xx xxx xxxxxxx xxxxxxxx xxxxxxxxxx xxxx xxxx Xxxxxx.xx0xxx xxxxxxxxxx xxxxx $xxxx xx xxxxx xx xxx $xxxxxx xxxxxxxxx$$ xxxxxxxxxx xxxx xxx xxxxxxx xxxx xxx xxxxxx xxxx xxx xxxxxxx$ xxx xxxxxxxxxx xxxx xxx xxxxxxxx xxxx xxx xxxxxx xxxx xxxx xxxxxxx xx xxxxx xxx Xxxxxx$XXXxxxxxx xxxxxx.

Xxx xxx xxx xxxx xxxxxx xx xxxxxxx xxx xxxxxxxxxx xxxx.
Xxxx$ xxx xxx xxx xxx Xxxxxx$XxxxxxXxxx xxxxxx xx xxxxxxxxx xxx xxxxxxx $xxxxxxx xxxx xx XXX$ xxx xxxx xxxx xx Xxxxxx.xx0xxx xxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxxxxxxxxx xxxxx xx Xxxxxxx XxxxxXxxxx$ xxx xxxxx$Xxxxxx.xx0xxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-formatdata
```

Xxxx xxxxxxx xxxx xxx xxx xxxxxxxxxx xxxx xx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-formatdata -typename Microsoft.Wsman*
```

Xxxx xxxxxxx xxxx xxx xxxxxxxxxx xxxx xxxxx xxxxx xxxxx xxxxx xxxx $Xxxxxxxxx.Xxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$f = get-formatdata -typename helpinfoshort
PS C:\>$f

TypeName        FormatViewDefinition
--------        --------------------
HelpInfoShort   {help , TableControl}

PS C:\>$f.FormatViewDefinition[0].control

Headers                                                                    Rows
-------                                                                    ----
{System.Management.Automation.TableControlColumnHeader, System.Manageme... {System.Management.Automation.TableControlRow}

PS C:\>$f.FormatViewDefinition[0].control.headers

Label         Alignment      Width
-----         ---------      -----
Name          Left           33
Category      Left           9
Undefined      0
```

Xxxx xxxxxxx xxxxx xxx xx xxx x xxxxxxxxxx xxxx xxxxxx xxx xxxxxxx xxx xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = get-formatdata
PS C:\>import-module bitstransfer
PS C:\>$b = get-formatdata
PS C:\>compare-object $a $b

InputObject                                                SideIndicator
-----------                                                -------------
Microsoft.BackgroundIntelligentTransfer.Management.BitsJob =>

PS C:\>get-formatdata *bits* | export-formatdata -filepath c:\test\bits.format.ps1xml
PS C:\>get-content c:\test\bits.format.ps1xml

<?xml version="1.0" encoding="utf-8"?><Configuration><ViewDefinitions>
<View><Name>Microsoft.BackgroundIntelligentTransfer.Management.BitsJob</Name>
...
```

Xxxx xxxxxxx xxxxx xxx xx xxx Xxx$XxxxxxXxxx xxx Xxxxxx$XxxxxxXxxx xx xxxxxx xxx xxxxxxxxxx xxxx xxxx xx xxxxx xx x xxxxxx.

Xxx xxxxx xxxx xxxxxxxx xxx xxx Xxx$XxxxxxXxxx$ Xxxxxx$Xxxxxx$ xxx Xxxxxxx$Xxxxxx xxxxxxx xx xxxxxxxx xxx xxxxxx xxxx xxxx xxx XxxxXxxxxxxx xxxxxx xxxx xx xxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XxxxxxXxxx xxxxxx xx xxx xxx xxxxxx xxxx xxxx xxx XxxxXxxxxxxx xxxxxx xxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xxxx xxxxxx xx xxx Xxxxxx$XxxxxxXxxx xxxxxx$ xxxxx xxxxxxxx xx xxxx xx XXX xxx xxxxx xx xx xxx xxxxxxxxx xxxxxx.xx0xxx xxxx.

Xxx xxxxx xxxxxxx xxxxx xx xxxxxxx xx xxx xxxxxx.xx0xxx xxxx xxxxxxx.

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

### -TypeName
Xxxx xxxx xxx xxxxxxxxxx xxxx xxxx xxx xxxxxxxxx xxxx xxxxx.
Xxxxx xxx xxxx xxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

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

## XXXXXX

### None
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### System.Management.Automation.ExtendedTypeDefinition

## XXXXX

## XXXXXXX XXXXX

[Export-FormatData]()

[Update-FormatData]()

